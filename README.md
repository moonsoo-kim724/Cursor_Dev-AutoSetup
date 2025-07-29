# 🚀 Cursor 개발 자동화 환경 

> **완전 자동화된 개발 환경**: Python, Git, WSL, AI 도구까지 원클릭으로 설정!

## 📋 프로젝트 개요

이 프로젝트는 개발자를 위한 완전 자동화된 개발 환경 설정 도구입니다. 새로운 컴퓨터에서 개발 환경을 몇 분 만에 구축할 수 있으며, 다양한 AI 도구와 통합되어 있습니다.

## ✨ 주요 기능

### 🔧 자동 설치 도구
- **Python 3.10**: 가상환경 자동 설정
- **Git & GitHub CLI**: 자동 설정 및 인증
- **WSL Ubuntu 24.04**: 리눅스 환경 구축
- **Node.js & npm**: 웹 개발 환경

### ⚡ Cursor 완전 자동화
- 키보드 단축키 설정
- 프로젝트 자동 모니터링
- 가상환경 자동 설정
- Git 자동 커밋 & 푸시

### 🤖 AI 도구 통합
- **Vooster AI**: 작업 우선순위 자동 분석
- **MCP 서버**: Model Context Protocol 설정
- **Claude 자동화**: WSL 환경에서 Claude 실행

## 🔥 빠른 시작 (원클릭 설치)

### 1. PowerShell 관리자 실행
```powershell
# Windows + X → A (관리자 PowerShell)
```

### 2. 저장소 클론
```powershell
git clone https://github.com/moonsoo-kim724/cursor-automation-setup.git
cd cursor-automation-setup
```

### 3. 원클릭 설치 실행
```powershell
# 실행 정책 변경
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process

# 자동 설치 실행
.\quick-install.ps1
```

### 4. 완료! 🎉
- 모든 개발 도구가 자동으로 설치됩니다
- Cursor 설정이 자동으로 적용됩니다
- 프로젝트 템플릿이 준비됩니다

## 📁 프로젝트 구조

```
cursor-automation-setup/
├── 📁 scripts/                 # 자동화 스크립트
│   ├── install-automation.ps1  # 전체 환경 설정
│   ├── setup-mcp-servers.ps1   # MCP 서버 설정
│   ├── project-monitor.ps1     # 프로젝트 모니터링
│   └── vooster-ai-automation.ps1 # Vooster AI 자동화
├── 📁 settings/                # VS Code/Cursor 설정
│   ├── settings.json           # 에디터 설정
│   ├── keybindings.json        # 키보드 단축키
│   ├── tasks.json              # 작업 설정
│   ├── extensions.json         # 확장 프로그램
│   └── mcp-config.json         # MCP 설정
├── 📁 templates/               # 프로젝트 템플릿
│   └── nextjs-shadcn-template/ # Next.js + Shadcn/UI 템플릿
├── 📁 rules/                   # 개발 규칙 및 가이드
│   ├── global-rules.md         # 전체 개발 규칙
│   ├── web-stack-2025.md       # 웹 기술 스택 가이드
│   └── Taskmaster-ai-mcp.json  # AI 도구 설정
├── 📁 wsl-setup/               # WSL 설정
│   └── claude-auto-start.sh    # Claude 자동 시작
├── 📁 src/                     # 현재 활성 프로젝트 (ysk-ai-landingpage)
└── quick-install.ps1           # 원클릭 설치 스크립트
```

## ⌨️ 키보드 단축키

| 단축키 | 기능 |
|--------|------|
| `Ctrl+Alt+S` | 📊 프로젝트 상태 확인 |
| `Ctrl+Alt+V` | 🐍 Python 가상환경 활성화 |
| `Ctrl+Alt+G` | 📝 Git 자동 커밋 & 푸시 |
| `Ctrl+Alt+N` | 📦 Node.js 의존성 설치 |
| `Ctrl+Alt+U` | 📋 requirements.txt 업데이트 |
| `Ctrl+Alt+C` | 🤖 Claude 터미널 실행 |
| `Ctrl+Alt+Shift+V` | 🎯 Vooster AI 작업 관리 |
| `Ctrl+Alt+R` | 🔄 모든 서비스 재시작 |

## 🎯 사용 방법

### 새 프로젝트 시작
1. 원하는 템플릿을 새 프로젝트 폴더에 복사
2. Cursor에서 해당 폴더 열기
3. 자동으로 모든 설정 적용!

### Python 프로젝트
- 가상환경 자동 생성 및 활성화
- requirements.txt 자동 관리
- 개발 도구 자동 설정

### 웹 프로젝트
- Next.js + TypeScript + Tailwind CSS 자동 설정
- 필수 패키지 자동 설치
- 모던 UI 컴포넌트 구조

### Git 자동화
- 자동 `git init`
- 자동 `.gitignore` 생성
- 자동 GitHub 저장소 생성 및 연결

## 🤖 AI 도구 활용

### Vooster AI 작업 관리
- 작업 우선순위 자동 분석
- 기술 스택별 자동 실행
- 연속 작업 자동 처리

### MCP 서버 연결
- Model Context Protocol 지원
- 다양한 AI 도구 통합
- 자동 설정 및 연결

### WSL Claude 자동화
```bash
# WSL에서 사용 가능한 명령어
claude-start    # Claude 시작
claude-status   # 상태 확인
claude-restart  # 재시작
```

## 🔧 문제 해결

### 설정이 적용되지 않을 때
```powershell
# 설정 재적용
.\scripts\install-automation.ps1
```

### GitHub 인증 문제
```powershell
# GitHub CLI 로그인
gh auth login
```

### Python 가상환경 문제
```powershell
# 가상환경 수동 생성
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### WSL 문제
```powershell
# WSL 재시작
wsl --shutdown
wsl
```

## 🎊 설치 후 확인

### 필수 도구 설치 확인
```powershell
python --version    # Python 3.10.x
git --version       # git version 2.x
gh --version        # gh version 2.x
wsl --version       # WSL 버전 확인
```

### 개발 환경 확인
- `Ctrl+Alt+S` 프로젝트 상태 확인 작동
- 자동 완성 및 IntelliSense 작동
- 터미널 통합 작동

## 📞 지원 및 업데이트

### 자동 업데이트
```powershell
# 설정 폴더에서 실행
git pull origin main
.\quick-install.ps1
```

### 개별 구성 요소 업데이트
각 폴더의 README.md 파일을 참조하여 개별 설정이 가능합니다:

- **📁 scripts/**: 자동화 스크립트 관리
- **📁 settings/**: VS Code/Cursor 설정 관리
- **📁 templates/**: 프로젝트 템플릿 관리
- **📁 rules/**: 개발 규칙 및 가이드라인 관리

## 🏆 주요 특징

🔥 **완전 자동화**: 클릭 한 번으로 모든 설정 완료  
🎯 **스마트 감지**: 프로젝트 타입 자동 인식  
⚡ **빠른 실행**: 키보드 단축키로 즉시 실행  
🤖 **AI 통합**: 다양한 AI 도구 자동 연결  
🔄 **지속적 동기화**: 모든 PC에서 동일한 환경  

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 있습니다.

## 🤝 기여하기

1. 이 저장소를 포크합니다
2. 기능 브랜치를 생성합니다 (`git checkout -b feature/amazing-feature`)
3. 변경사항을 커밋합니다 (`git commit -m 'Add amazing feature'`)
4. 브랜치에 푸시합니다 (`git push origin feature/amazing-feature`)
5. Pull Request를 생성합니다

---

**🚀 이제 모든 PC에서 동일한 최적화된 개발 환경을 사용하세요!**

# 연수김안과의원 AI 기반 디지털 마케팅 랜딩페이지

> 30년의 신뢰, AI로 미래를 열다

## 📋 프로젝트 개요

연수김안과의원의 SEO/AEO 최적화 랜딩페이지 및 AI 기반 디지털 마케팅 플랫폼입니다. 30년 수술 전문 노하우와 최신 AI 기술을 결합하여 환자 중심의 디지털 헬스케어 경험을 제공합니다.

## ✨ 주요 기능

### 🎯 핵심 기능
- **AI 챗봇 상담**: GPT 기반 다국어(한/영/중) 의료 상담
- **스마트 예약 시스템**: Typebot 스타일 조건분기 설문 → 즉시 예약
- **CRM 자동화**: 카카오채널, SMS, 이메일 자동 발송
- **리뷰 관리**: UGC 수집 및 SEO 최적화
- **다국어 지원**: 외국인 환자를 위한 글로벌 서비스

### 🔧 기술적 특징
- **SEO/AEO 최적화**: 구조화된 데이터, 음성검색 대응
- **성능 최적화**: 2초 이내 로딩, PWA 지원
- **모바일 우선**: 반응형 디자인, 터치 최적화
- **보안 강화**: 의료정보 보호, GDPR 준수

## 🛠 기술 스택

### Frontend
- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS 3.4
- **UI Components**: shadcn/ui
- **Icons**: Lucide React

### Backend & Database
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth
- **Edge Functions**: Vercel Edge Functions
- **API**: tRPC (타입 안전한 API)

### AI & Integration
- **AI**: OpenAI GPT-4o, Google Gemini
- **Messaging**: Kakao BizMessage, CoolSMS
- **Analytics**: Google Analytics 4
- **SEO**: Next.js Metadata API

### Infrastructure
- **Hosting**: Vercel (Primary), Netlify (Backup)
- **CDN**: Vercel Edge Network
- **CI/CD**: GitHub Actions
- **Monitoring**: Vercel Analytics

## 🚀 시작하기

### 시스템 요구사항
- Node.js 16.8+ 
- npm 또는 yarn
- Git

### 설치 방법

1. **저장소 클론**
   ```bash
   git clone https://github.com/moonsoo-kim724/ysk-AI-LandingPage.git
   cd ysk-ai-landingpage
   ```

2. **의존성 설치**
   ```bash
   npm install
   # 또는
   yarn install
   ```

3. **환경 변수 설정**
   ```bash
   cp .env.example .env.local
   ```
   
   `.env.local` 파일에 다음 환경 변수를 설정하세요:
   ```env
   # Supabase
   NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
   SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
   
   # OpenAI
   OPENAI_API_KEY=your_openai_api_key
   
   # Kakao
   KAKAO_API_KEY=your_kakao_api_key
   
   # SMS
   COOLSMS_API_KEY=your_coolsms_api_key
   COOLSMS_API_SECRET=your_coolsms_secret
   ```

4. **개발 서버 실행**
   ```bash
   npm run dev
   # 또는
   yarn dev
   ```

5. **브라우저에서 확인**
   http://localhost:3000 에서 확인할 수 있습니다.

## 📁 프로젝트 구조

```
ysk-ai-landingpage/
├── src/
│   ├── app/                 # Next.js App Router
│   │   ├── (dashboard)/     # 관리자 대시보드
│   │   ├── api/            # API 라우트
│   │   ├── globals.css     # 글로벌 스타일
│   │   ├── layout.tsx      # 루트 레이아웃
│   │   └── page.tsx        # 메인 페이지
│   ├── components/         # 재사용 가능한 컴포넌트
│   │   ├── ui/            # shadcn/ui 컴포넌트
│   │   ├── forms/         # 폼 컴포넌트
│   │   ├── chat/          # 챗봇 컴포넌트
│   │   └── layout/        # 레이아웃 컴포넌트
│   ├── lib/               # 유틸리티 및 설정
│   │   ├── supabase.ts    # Supabase 클라이언트
│   │   ├── utils.ts       # 공통 유틸리티
│   │   └── validators.ts  # 폼 검증
│   ├── hooks/             # 커스텀 React 훅
│   ├── types/             # TypeScript 타입 정의
│   └── styles/            # 추가 스타일 파일
├── public/                # 정적 파일
├── docs/                  # 프로젝트 문서
└── .github/              # GitHub 설정
    └── workflows/        # CI/CD 워크플로우
```

## 🔄 개발 워크플로우

### 브랜치 전략
- `main`: 프로덕션 브랜치
- `develop`: 개발 브랜치
- `feature/*`: 기능 개발 브랜치
- `bugfix/*`: 버그 수정 브랜치
- `hotfix/*`: 긴급 수정 브랜치

### 코드 품질
```bash
# 린팅
npm run lint

# 포맷팅
npm run format

# 타입 체크
npm run type-check

# 빌드 테스트
npm run build
```

## 📊 성능 목표

- **로딩 속도**: FCP ≤ 1.5초, TTI ≤ 3초
- **SEO 점수**: Lighthouse 90+
- **접근성**: WCAG 2.1 AA 준수
- **모바일 성능**: PageSpeed Insights 90+
- **서버 가용성**: 99.9% SLA

## 🔒 보안 & 규정 준수

- **의료정보보호**: 개인정보 암호화 (AES-256)
- **통신 보안**: HTTPS 강제, CSP 헤더
- **규정 준수**: 의료광고법, 개인정보보호법, GDPR
- **API 보안**: Rate Limiting, CORS 설정

## 🌐 다국어 지원

| 언어 | 코드 | 상태 |
|------|------|------|
| 한국어 | ko | ✅ 완료 |
| English | en | 🚧 진행중 |
| 中文 | zh | 📋 계획됨 |

## 📈 분석 & 모니터링

- **사용자 분석**: Google Analytics 4
- **성능 모니터링**: Vercel Analytics
- **에러 추적**: Sentry (계획됨)
- **A/B 테스트**: Vercel Edge Config

## 🤝 기여하기

1. 이 저장소를 포크합니다
2. 기능 브랜치를 생성합니다 (`git checkout -b feature/amazing-feature`)
3. 변경사항을 커밋합니다 (`git commit -m 'Add amazing feature'`)
4. 브랜치에 푸시합니다 (`git push origin feature/amazing-feature`)
5. Pull Request를 생성합니다

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 있습니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

## 📞 연락처

- **개발팀**: development@ysk-eye.com
- **프로젝트 매니저**: pm@ysk-eye.com
- **이슈 리포트**: [GitHub Issues](https://github.com/moonsoo-kim724/ysk-AI-LandingPage/issues)

## 🙏 감사의 말

이 프로젝트는 다음 오픈소스 프로젝트들의 도움을 받았습니다:
- [Next.js](https://nextjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [shadcn/ui](https://ui.shadcn.com/)
- [Supabase](https://supabase.com/)

---

**연수김안과의원** | 30년의 신뢰, AI로 미래를 열다
