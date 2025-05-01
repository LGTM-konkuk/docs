# API Specification

이 문서는 LGTM-konkuk 코드 리뷰 플랫폼의 API 명세서를 포함하고 있습니다.

## 기능 정의

이 API는 코드 리뷰 시스템에서 사용되는 기능들을 제공합니다. 주요 기능은 다음과 같습니다:

- **사용자 관리**: 사용자 등록, 정보 수정, 조회
- **리뷰 관리**: 코드 리뷰 요청, 코드 리뷰 진행, 리뷰 피드백
- **알림 시스템**: 리뷰 상태에 대한 알림 전송
- **프로젝트 관리**: 코드 리뷰가 진행될 프로젝트 생성 및 관리

## API 엔드포인트

### 1. 사용자 관리

#### **POST /users**
새로운 사용자를 등록합니다.

- **Request body**:
  ```json
  {
    "username": "john_doe",
    "email": "john@example.com",
    "password": "password123"
  }

- **Response**:
  ```json
  {
    "id": 1,
    "username": "john_doe",
    "email": "john@example.com"
  }
  ```
