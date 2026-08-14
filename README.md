# POE 보따리

**POE 보따리(POE BOTTARI)**는 Path of Exile을 플레이하면서 필요한 Path of Building, 거래 검색, 아이템 비교, 제작 실험, 게임 단축키와 사이트 번역을 한곳에서 연결하는 Windows 데스크톱 도구입니다.

> 비공식 커뮤니티 프로젝트이며 Grinding Gear Games가 제작하거나 보증한 프로그램이 아닙니다.

![POE 보따리 메인 화면](assets/product/0.1.5/desktop-overview.png)

## 무엇을 할 수 있나요?

- **PoB1·PoB2 관리**: PoB1 안정판과 3.29 미리보기, PoB2를 보따리 안에서 실행하고 연결 상태를 관리합니다.
- **게임 단축키**: `/hideout`, `/exit`, `/dnd` 같은 채팅 명령과 지도 필터·정보 검색을 원하는 키에 연결합니다.
- **아이템 가격 검색**: 게임에서 복사한 아이템을 분석해 공식 거래소 표본과 가격 범위를 확인합니다.
- **PoB 성능 비교**: 거래소 아이템을 현재 빌드에 적용했을 때 DPS·EHP가 어떻게 달라지는지 확인합니다.
- **제작 시뮬레이션**: 화폐, 에센스, 화석, 수확, 야수, 영향력, 작업대 등 PoE1 제작 방법을 단계별로 실험합니다.
- **사이트 번역**: poe.ninja, Craft of Exile, PoE Planner, pobb.in, Wealthy Exile, FilterBlade, poe.re/poe2.re를 선택한 언어로 기기 안에서 번역합니다.
- **안전한 업데이트**: 서명된 버전 정보와 SHA-256을 확인하고, 앱/Native Host 변경 시에는 전체 설치 파일을 사용합니다.

## 제품 화면

### 게임 단축키

![게임 단축키 설정](assets/product/0.1.5/game-shortcuts.png)

### 제작 시뮬레이터

![POE1 제작 시뮬레이터](assets/product/0.1.5/crafting-workbench.png)

### Chrome 확장프로그램과 가격 검색

<p>
  <img src="assets/product/0.1.5/chrome-extension.png" alt="Chrome 확장프로그램 설정" width="340">
  <img src="assets/product/0.1.5/trade-price-search.png" alt="아이템 가격 검색 결과" width="620">
</p>

## 다운로드

- Windows 설치 파일: [GitHub 릴리스 목록](https://github.com/seeyouworks/POE-BOTTARI-Releases/releases)
- Chrome 확장프로그램: [Chrome Web Store 항목](https://chromewebstore.google.com/detail/hdgedfadfonijbdlnonhhapamhnhebil)

이 저장소에는 제품 소스 코드가 아니라 공식 설치 파일, 체크섬, 릴리스 안내, 개인정보처리방침과 지원 문서만 게시합니다.

## 설치

1. 최신 릴리스의 Assets에서 `.exe` 설치 파일과 같은 이름의 `.sha256` 파일을 내려받습니다.
2. 필요하면 PowerShell에서 무결성을 확인합니다.

   ```powershell
   Get-FileHash .\POE-BOTTARI-Setup-community-0.1.5.exe -Algorithm SHA256
   ```

3. 설치 파일을 실행하고 POE 보따리를 시작합니다.
4. 앱의 `최신받기`는 서명된 새 버전과 설치 파일 해시를 확인해 내려받지만, 설치 실행과 교체는 사용자가 직접 진행합니다.

현재 community 설치 파일은 Authenticode 코드 서명이 없어 Windows에서 `알 수 없는 게시자` 또는 평판 경고가 표시될 수 있습니다. 반드시 이 공식 저장소에서만 내려받으세요.

## 데이터와 권한

사이트 번역은 외부 번역 서비스나 광고·분석 서버로 페이지 내용을 보내지 않고 기기 안에서 처리합니다. 거래 기능을 명시적으로 실행할 때만 선택한 아이템 원문과 현재 거래 URL이 로컬에 설치된 POE 보따리 앱으로 전달됩니다.

자세한 내용은 [개인정보처리방침](PRIVACY.md)을 확인하세요.

## 지원

재현 가능한 오류와 릴리스 문의는 [GitHub Issues](https://github.com/seeyouworks/POE-BOTTARI-Releases/issues)에 남겨주세요. 계정 비밀번호, 쿠키, POESESSID, OAuth 토큰, 비공개 빌드 파일은 첨부하지 마세요.

---

## English

POE BOTTARI is an unofficial Windows companion for Path of Exile. It manages PoB1/PoB2 workflows, game shortcuts, trade-item price and build-impact checks, PoE1 crafting experiments, and on-device translation for supported community sites.

Download the latest Windows installer from [GitHub Releases](https://github.com/seeyouworks/POE-BOTTARI-Releases/releases). The community installer is currently unsigned, and the app verifies signed update metadata and installer SHA-256 without automatically executing the downloaded file.
