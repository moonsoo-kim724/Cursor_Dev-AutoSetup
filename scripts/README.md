# 자동화 스크립트

이 폴더는 개발 환경 설정과 자동화를 위한 PowerShell 스크립트들을 포함합니다.

## 📁 스크립트 목록

### 🔧 환경 설정
- **`install-automation.ps1`**: Cursor 자동화 환경 전체 설정
- **`setup-mcp-servers.ps1`**: MCP 서버 설정 및 구성

### 📊 모니터링
- **`project-monitor.ps1`**: 프로젝트 상태 및 파일 변경 모니터링

### 🤖 AI 통합
- **`vooster-ai-automation.ps1`**: Vooster AI 자동화 스크립트

## 🚀 사용 방법

### 전체 환경 설정
```powershell
# 관리자 권한으로 PowerShell 실행
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
.\scripts\install-automation.ps1
```

### 개별 스크립트 실행
```powershell
# MCP 서버 설정
.\scripts\setup-mcp-servers.ps1

# 프로젝트 모니터링 시작
.\scripts\project-monitor.ps1

# Vooster AI 자동화
.\scripts\vooster-ai-automation.ps1
```

## ⚠️ 주의사항

1. **관리자 권한**: 일부 스크립트는 관리자 권한이 필요합니다
2. **실행 정책**: PowerShell 실행 정책을 적절히 설정해야 합니다
3. **종속성**: 일부 스크립트는 특정 프로그램이 설치되어 있어야 합니다

## 🔍 문제 해결

### PowerShell 실행 정책 오류
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

### 스크립트 실행 권한 오류
```powershell
# 관리자 권한으로 PowerShell 실행 후 재시도
``` 