# 🌊 명조 체크리스트 (Wuthering Waves Checklist)

명조: 워더링 웨이브의 일일/주간/월간 숙제를 관리하는 데스크톱 앱입니다.

## ✨ 기능

- **일일 숙제** — 활약도 100, 플레이트 소모, 일반 의뢰, 방송국, 광석, 낚시, 에코런, 모네 파밍
- **주간 숙제** — 군가의 중주, 수많은 문의 환상, 강화 흡수, 방송국, 상점, 채집
- **월간 컨텐츠** — 역경의 탑 심경구역, 바닷속 폐허, 매트릭스 더블 폰스
- **리셋 타이머** — 일일/주간/월간 리셋까지 남은 시간 실시간 표시
- **팁 시스템** — 각 항목별 공략 팁 제공
- **메모 기능** — 항목별 개인 메모 저장
- **카운터** — 군가의 중주 3회, 강화 흡수 15회 등 횟수 추적

## 📥 다운로드

[Releases](../../releases) 페이지에서 최신 `.exe` 파일을 다운받아 실행하세요.

- **설치형**: `명조 체크리스트 Setup x.x.x.exe` — 설치 후 사용
- **포터블**: `WW-Checklist-Portable.exe` — 설치 없이 바로 실행

## 🛠️ 직접 빌드하기

### 준비물
- [Node.js](https://nodejs.org) v18 이상 (LTS 권장)

### 빌드 방법

```bash
# 1. 저장소 클론
git clone https://github.com/YOUR_USERNAME/ww-checklist.git
cd ww-checklist

# 2. 의존성 설치
npm install

# 3. 개발 모드 실행 (테스트)
npm start

# 4. .exe 빌드
npm run dist
```

빌드 완료 후 `dist/` 폴더에 `.exe` 파일이 생성됩니다.

### 다른 OS 빌드

```bash
npm run dist:mac    # macOS
npm run dist:linux  # Linux
```

## 🔄 자동 빌드 (GitHub Actions)

태그를 push하면 자동으로 `.exe`가 빌드되어 Release에 올라갑니다.

```bash
git tag v1.0.0
git push origin v1.0.0
```

## 📁 프로젝트 구조

```
ww-checklist/
├── .github/
│   └── workflows/
│       └── build.yml          # GitHub Actions 자동 빌드
├── build/
│   └── icon.png               # 앱 아이콘 (256x256)
├── src/
│   ├── main.js                # Electron 메인 프로세스
│   └── index.html             # 앱 UI (HTML/CSS/JS)
├── package.json               # 프로젝트 설정
└── README.md
```

## 📋 향후 추가 예정

- [ ] 별의 소리 가계부
- [ ] 패키지 효율 계산기
- [ ] 자동 리셋 (시간 도래 시 체크 초기화)

## 📄 라이선스

MIT License
