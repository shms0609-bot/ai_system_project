# 🏠 SafeHome AI - 대학생을 위한 전세 사기 예방 서비스

**SafeHome AI**는 사회초년생과 대학생들이 복잡한 임대차 계약서를 사진 찍어 올리면, AI가 독소 조항과 위험 요소를 분석하여 알기 쉽게 설명해 주는 서비스입니다.

---

## 🛠️ 필수 설치 프로그램 (Prerequisites)

이 프로젝트를 실행하기 위해 아래 프로그램들이 먼저 설치되어 있어야 합니다.

### 1. Git
- **용도**: 프로젝트 코드를 내려받고 관리합니다.
- **다운로드**: [git-scm.com](https://git-scm.com/downloads)

### 2. Python 
- **용도**: 백엔드(FastAPI) 서버를 구동합니다.
- **다운로드**: [python.org](https://www.python.org/downloads/)
- **주의**: 설치 시 **'Add Python to PATH'** 옵션을 반드시 체크해 주세요.

### 3. Node.js 
- **용도**: 프론트엔드(React) 개발 환경을 구동합니다.
- **다운로드**: [nodejs.org](https://nodejs.org/ko) (LTS 버전을 권장합니다)

---

## 🚀 시작하기 (Installation & Setup)

### 1. 저장소 복제 (Clone)
터미널을 열고 아래 명령어를 입력하여 코드를 가져옵니다.
```bash
git clone https://github.com/shms0609-bot/ai_system_project
cd ai_system_project

2. 백엔드 설정 (Backend Setup)

cd backend
# 1. 가상환경 생성 및 활성화
python -m venv venv
# Windows의 경우:
.\venv\Scripts\activate
# Mac/Linux의 경우: source venv/bin/activate

# 2. 필요한 패키지 설치
pip install -r requirements.txt

# 3. 환경 변수 설정
# backend 폴더 안에 .env 파일을 생성하고 아래 내용을 입력하세요.
# GEMINI_API_KEY=발급받은_본인의_API_키


3. 프론트엔드 설정 (Frontend Setup)
cd ../frontend
# 1. 패키지 설치
npm install

터미널 1: 백엔드 서버 실행
cd backend
.\venv\Scripts\activate
uvicorn main:app --reload

터미널 2: 프론트엔드 서버 실행
cd frontend
npm run dev
