name: "🛠️ 기능 개발 요청"
description: "새로운 기능을 개발하기 위한 이슈"
title: "[Feature] "
labels: ["feature", "development"]
assignees:
  - your-github-username

body:
  - type: markdown
    attributes:
      value: "## 🔧 작업 개요\n기능 개발의 주요 목표를 간략하게 설명하세요."

  - type: textarea
    id: overview
    attributes:
      label: "작업 개요"
      description: "이슈의 핵심 목표를 간단하게 정리하세요."
      placeholder: "예: Kakao API와 PostGIS를 활용한 지도 기능 개발"

  - type: markdown
    attributes:
      value: "## 📋 상세 설명\n이 기능이 어떤 역할을 하는지 구체적으로 설명하세요."

  - type: textarea
    id: description
    attributes:
      label: "상세 설명"
      description: "구현할 기능의 세부 내용을 작성하세요."
      placeholder: "예: 사용자의 현재 위치를 가져와 주변 소셜다이닝 이벤트를 필터링합니다."

  - type: markdown
    attributes:
      value: "## 📝 작업 내용\n이 기능을 구현하기 위해 수행해야 할 작업 목록을 작성하세요."

  - type: checkboxes
    id: tasks
    attributes:
      label: "작업 목록"
      description: "이 기능을 완성하기 위해 필요한 세부 작업을 작성하세요."
      options:
        - label: "기능 기획 및 설계"
        - label: "API 연동 및 데이터 처리"
        - label: "프론트엔드 UI 구현"
        - label: "백엔드 로직 개발"
        - label: "테스트 및 디버깅"
        - label: "최종 배포"

  - type: markdown
    attributes:
      value: "## 📸 참고 자료\n이 기능을 개발하는 데 참고할 자료(문서, API 명세서 등)를 정리하세요."

  - type: textarea
    id: references
    attributes:
      label: "참고 자료"
      description: "관련 API 문서, DB ERD, 디자인 문서 등의 링크를 추가하세요."
      placeholder: "예: [Kakao 지도 API 문서](https://developers.kakao.com/docs/latest/ko/local/dev-guide)"

  - type: markdown
    attributes:
      value: "## 🚀 진행 상황\n현재 진행 상태를 체크박스로 관리하세요."

  - type: checkboxes
    id: progress
    attributes:
      label: "진행 상황"
      description: "각 항목이 완료될 때 체크하세요."
      options:
        - label: "🛠️ 개발 시작"
        - label: "🚀 기본 기능 구현 완료"
        - label: "🔧 테스트 및 디버깅"
        - label: "✅ 기능 완성 및 배포"
