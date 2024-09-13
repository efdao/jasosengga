# 자소서 챗봇 (Self-Introduction Chatbot)

이 프로젝트는 Django를 기반으로 한 챗봇으로, 사용자가 입력한 정보를 바탕으로 회사 맞춤형 자기소개서를 생성해주는 시스템입니다. 회사 분석 데이터베이스를 이용하여 특정 회사에 맞춘 자기소개서를 작성할 수 있도록 도와줍니다.

## 주요 기능

- **회사 맞춤 자기소개서 생성**: 사용자가 선택한 회사에 맞춰 적합한 자기소개서를 생성합니다.
- **회사 데이터베이스 기반 분석**: 회사의 요구 사항과 특성에 맞춰 자기소개서를 작성할 수 있도록 회사 데이터를 분석합니다.
- **사용자 인터랙션 챗봇**: 자연어 처리(NLP)를 통해 사용자와의 대화를 통해 정보를 수집하고 자기소개서를 작성합니다.

## 기술 스택

- **백엔드**: Django (Python)
- **프론트엔드**: HTML, CSS, JavaScript
- **데이터베이스**: SQLite (개발 단계)
- **API 사용**: OpenAI API (NLP 모델 사용)

## 설치 및 실행 방법

```bash
# 1. 프로젝트 클론 및 디렉토리 이동
git clone https://github.com/efdao/jasoseongga.git
cd jasoseongga

# 2. 가상 환경 생성 및 활성화 (선택 사항)
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows

# 3. 패키지 설치
pip install -r requirements.txt

# 4. .env 파일 생성 및 환경 변수 설정
echo "OPENAI_API_KEY=your_openai_api_key" > teamproject/.env
echo "DATABASE_URL=your_database_url" >> teamproject/.env

# 5. 데이터베이스 마이그레이션
python manage.py migrate

# 6. 서버 실행
python manage.py runserver

# 7. 브라우저에서 http://127.0.0.1:8000 접속
```

## 사용 방법

1. 웹페이지에 접속하여 사용자 정보를 입력합니다.
2. 원하는 회사와 관련된 정보를 입력한 후, "자기소개서 생성" 버튼을 클릭합니다.
3. 챗봇이 대화 형식으로 질문을 하고, 사용자는 이에 맞게 대답합니다.
4. 수집된 정보를 바탕으로 회사 맞춤형 자기소개서가 생성됩니다.
