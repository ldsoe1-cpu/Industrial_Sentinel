# Industrial Sentinel - Professional GIS Analysis Engine (v1.0) 🛰️

**Industrial Sentinel**은 화학 사고 예방 및 산업 단지 조사를 위한 GIS 기반의 고정밀 자동화 분석 플랫폼입니다. 카카오 로컬 API와 Playwright 자동화 엔진을 결합하여, 특정 사업장 주변 1~2km 반경 내의 모든 산업 시설을 전수 조사하고 법적 증빙 자료를 자동으로 수집합니다.

---

## 🚀 주요 기능 (Key Features)

### 1. 📍 전문가용 GIS 시각화 (Expert GIS Visualization)
- **나노 도트 시스템**: 지형지물 분석을 방해하지 않는 5px/8px 크기의 초정밀 도트 마커와 플로팅 라벨 시스템을 적용했습니다.
- **듀얼 맵 동기화**: 실시간 분석 지도와 하이브리드 항공 사진 분석 탭이 완벽히 동기화되어 다각도 분석이 가능합니다.
- **중심 사업장 강조**: 검색 대상(Hero)과 주변 시설(Neighbors)을 색상(파란색/주황색)과 크기로 명확히 구분합니다.

### 2. 🤖 2단계 자동 조사 엔진 (2-Phase Investigation)
- **Phase 1 (Scan)**: 카카오 로컬 API를 활용하여 5개 산업 핵심 키워드 기반의 전수 조사를 수행합니다.
- **Phase 2 (Capture)**: **Playwright** 엔진이 상업용 상세 페이지에 자동 접속하여 증빙 스크린샷을 채득하고 데이터를 마이닝합니다.

### 3. 📊 다각도 분석 보고 (Multi-Dimensional Reporting)
- **증빙 갤러리**: 자동 수집된 모든 사업장의 상세 페이지 캡처본을 카드 형태로 즉시 시각화합니다.
- **엑셀 리포트**: 수집된 종업원 수, 생산품, 원내/외 판정 등의 데이터를 포함한 전문 리포트를 즉시 다운로드할 수 있습니다.

---

## 🛠️ 기술 스택 (Tech Stack)

- **Backend**: Python, Flask, Pandas
- **Frontend**: Tailwind CSS, Kakao Map SDK, JavaScript (ES6+)
- **Automation**: Playwright (Headless Browser Engine)
- **API**: Kakao Local API, Kakao Geo-coding API

---

## ⚙️ 설치 및 실행 (Installation & Setup)

프로젝트를 로컬 환경에서 실행하려면 아래의 단계를 따라주세요.

### 1. 필수 라이브러리 설치
```bash
pip install -r requirements.txt
```

### 2. 브라우저 엔진 설치 (Playwright)
```bash
playwright install chromium
```

### 3. 환경 변수 설정
`.env` 파일을 프로젝트 루트 디렉토리에 생성하고 아래의 API 키를 입력하세요.
```env
KAKAO_JS_KEY=YOUR_KAKAO_JS_KEY
KAKAO_REST_KEY=YOUR_KAKAO_REST_KEY
```

### 4. 서버 시작
```bash
python app.py
```
접속 주소: `http://127.0.0.1:5000`

---

## 📜 라이선스 및 저작권 (License)
본 프로젝트는 산업 안전 및 사고 예방을 목적으로 제작되었습니다. 무단 복제 및 상업적 재배포 시 깃허브 소유자(`ldsoe1-cpu`)와의 협의가 필요합니다.

---

**Developed with by Jenny - Your AI Coding Assistant**
