# 자기소개 챗봇 (Jasoseongga)

이 프로젝트는 Django를 기반으로 한 **자기소개 챗봇**으로, 사용자가 다양한 질문을 통해 자기소개를 할 수 있도록 도와줍니다.
특히, 웹 크롤링을 통해 만들어진 **기업 분석 DB**를 활용하여 특정 기업에 특화된 자기소개서를 작성하는 데 도움을 줍니다. 학교 캡스톤 디자인 과제의 일환으로 개발되었습니다.

## 주요 기능
- 질문에 따른 자기소개 답변 제공
- 대화형 자기소개 지원
- **기업 분석 DB**를 활용한 기업 맞춤형 자기소개서 작성 지원
- 사용자 정보 저장 및 관리

## 기술 스택
- **Backend:** Django
- **Frontend:** HTML, CSS, JavaScript
- **Database:** SQLite (개발용)

## 설치 및 실행

1. 레포지토리 클론:
    ```bash
    git clone https://github.com/efdao/jasoseongga.git
    cd jasoseongga
    ```

2. 가상환경 생성 및 패키지 설치:
    ```bash
    python -m venv venv
    source venv/bin/activate  # MacOS/Linux
    venv\Scripts\activate     # Windows
    pip install -r requirements.txt
    ```

3. 마이그레이션 및 서버 실행:
    ```bash
    python manage.py migrate
    python manage.py runserver
    ```

4. 브라우저에서 `http://localhost:8000`로 접속하여 확인

## 프로젝트 구조
