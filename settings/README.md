# VS Code 설정 파일

이 폴더는 VS Code와 Cursor IDE의 설정 파일들을 포함합니다.

## 📁 설정 파일 목록

### 🎨 에디터 설정
- **`settings.json`**: VS Code/Cursor 기본 설정
- **`keybindings.json`**: 사용자 정의 키보드 단축키

### 🔧 개발 환경
- **`tasks.json`**: 자동화 작업 및 빌드 태스크
- **`extensions.json`**: 권장 확장 프로그램 목록

### 🤖 AI 통합
- **`mcp-config.json`**: MCP (Model Context Protocol) 서버 설정

## 🚀 사용 방법

### 자동 적용
```powershell
# 설정 파일들을 VS Code/Cursor 설정 디렉토리에 복사
.\scripts\install-automation.ps1
```

### 수동 적용
1. VS Code/Cursor 설정 디렉토리 열기:
   - Windows: `%APPDATA%\Code\User\`
   - macOS: `~/Library/Application Support/Code/User/`
   - Linux: `~/.config/Code/User/`

2. 해당 폴더의 파일들을 설정 디렉토리에 복사

### 백업 및 복원
```powershell
# 현재 설정 백업
copy "%APPDATA%\Code\User\settings.json" ".\settings\settings.backup.json"

# 설정 복원
copy ".\settings\settings.json" "%APPDATA%\Code\User\settings.json"
```

## ⚙️ 주요 설정 내용

### 코딩 스타일
- 자동 포맷팅: Prettier
- 린팅: ESLint
- 탭 크기: 2칸
- 자동 저장: 활성화

### AI 도구
- GitHub Copilot 최적화
- MCP 서버 연결
- 자동 완성 개선

### 워크플로우
- 자동 태스크 실행
- 핫 리로드 설정
- 디버깅 구성

## 🔄 업데이트

설정 파일들은 정기적으로 업데이트됩니다. 최신 버전을 유지하려면:
```powershell
git pull origin main
.\scripts\install-automation.ps1
``` 