# 나의 서재 — PWA 배포 가이드

## 파일 구성
```
bookapp/
├── index.html      ← 앱 본체
├── manifest.json   ← PWA 설정
├── sw.js           ← 오프라인 지원
├── icon-192.png    ← 앱 아이콘 (직접 추가)
├── icon-512.png    ← 앱 아이콘 (직접 추가)
└── README.md
```

---

## 🚀 GitHub Pages로 배포하기 (무료, 5분)

### 1단계 — GitHub 가입
https://github.com 에서 무료 계정 만들기

### 2단계 — 새 저장소 만들기
1. 우측 상단 `+` → **New repository**
2. Repository name: `bookapp` (또는 원하는 이름)
3. **Public** 선택
4. **Create repository** 클릭

### 3단계 — 파일 업로드
1. 저장소 페이지에서 **Add file → Upload files** 클릭
2. `index.html`, `manifest.json`, `sw.js` 세 파일을 드래그해서 올리기
3. **Commit changes** 클릭

### 4단계 — GitHub Pages 활성화
1. 저장소 상단 **Settings** 탭 클릭
2. 왼쪽 메뉴 **Pages** 클릭
3. Source: **Deploy from a branch**
4. Branch: **main** → `/ (root)` 선택 → **Save**
5. 1~2분 기다리면 배포 완료!

### 5단계 — 앱 주소 확인
`https://[내GitHub아이디].github.io/bookapp/`

---

## 📱 아이폰 홈 화면에 추가하기

1. iPhone의 **Safari**로 위 주소 접속
2. 하단 **공유 버튼** (네모+화살표) 탭
3. **"홈 화면에 추가"** 탭
4. 이름 확인 후 **추가** 탭
5. 홈 화면에 앱 아이콘이 생성됨 ✅

> ⚠️ Chrome이 아닌 **Safari**에서만 홈 화면 추가가 가능합니다.

---

## 🎨 앱 아이콘 만들기 (선택)

icon-192.png, icon-512.png 파일이 없으면 기본 아이콘이 사용됩니다.
직접 만들고 싶다면:
- https://www.canva.com 에서 192×192, 512×512 크기로 제작
- 또는 https://favicon.io 에서 텍스트로 간단하게 생성

---

## 💾 데이터 저장
- 모든 데이터는 **기기의 로컬 저장소**에 저장됩니다
- 앱을 삭제하면 데이터도 삭제되니 주의하세요
- 중요한 데이터는 주기적으로 백업하는 것을 권장합니다
