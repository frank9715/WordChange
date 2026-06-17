# 영어 문장 연습기 (English Sentence Practice)

주제별로 자연스러운 영어 문장을 만들고, 단어를 바꿔 가며 반복 연습하는 웹 앱입니다.
설치형 PWA(Progressive Web App)로 동작하여 모바일/데스크톱에서 오프라인으로도 사용할 수 있습니다.

## 주요 기능

- 주제별 영어 문장 연습
- 문장 속 단어를 바꿔 가며 패턴 학습
- PWA 지원 (홈 화면 설치 · 오프라인 캐시)

## 실행 방법

별도의 빌드 과정 없이 정적 파일로 동작합니다.

```bash
# 간단한 로컬 서버 실행 예시
python3 -m http.server 8000
```

브라우저에서 `http://localhost:8000/english-practice.html` 로 접속하세요.

> PWA(서비스 워커·설치) 기능은 `file://` 직접 열기에서는 제한될 수 있으므로 로컬 서버 또는 정적 호스팅 환경에서 실행하는 것을 권장합니다.

## 구성 파일

| 파일 | 설명 |
|---|---|
| `english-practice.html` | 앱 본체 (HTML/CSS/JS 단일 파일) |
| `manifest.webmanifest` | PWA 매니페스트 |
| `sw.js` | 서비스 워커 (오프라인 캐시) |
| `icon-192.png`, `icon-512.png` | 앱 아이콘 |
