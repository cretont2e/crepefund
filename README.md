# WordPress to Vercel 마이그레이션 가이드

이 프로젝트는 WordPress 사이트를 Vercel로 배포하기 위한 설정을 포함하고 있습니다.

## 배포 상태

- 도메인: crepe.fund
- 상태: 배포 진행 중

## 사전 요구사항

1. [Vercel CLI](https://vercel.com/download) 설치
2. [Git](https://git-scm.com/) 설치
3. [Vercel 계정](https://vercel.com/signup)
4. [GitHub 계정](https://github.com/join)

## 배포 단계

1. GitHub 저장소 생성:
   - GitHub에서 새 저장소 생성 [github.com/new](https://github.com/new)
   - 저장소 이름 설정 (예: my-wordpress-site)
   - 저장소를 공개 또는 비공개로 설정

2. 로컬 저장소 초기화 및 GitHub 연결:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/사용자명/저장소이름.git
   git push -u origin main
   ```

3. Vercel과 GitHub 저장소 연결:
   - [Vercel 대시보드](https://vercel.com/dashboard)에서 "New Project" 클릭
   - GitHub 저장소 선택
   - 프로젝트 설정 확인 후 "Deploy" 클릭

4. 또는 CLI로 배포 (GitHub 연결 후):
   ```bash
   vercel login
   vercel
   ```

5. 프로덕션 배포:
   ```bash
   vercel --prod
   ```

## 주의사항

- WordPress 사이트를 Vercel에 배포할 때는 데이터베이스 연결을 외부 데이터베이스(예: MySQL 호스팅 서비스)로 설정해야 합니다.
- 정적 콘텐츠만 Vercel을 통해 서빙됩니다. 동적 기능은 별도의 서버리스 함수로 구현해야 할 수 있습니다.
- 업로드된 미디어 파일은 외부 스토리지(예: AWS S3)에 저장해야 합니다.

## 환경 변수 설정

Vercel 대시보드에서 다음 환경 변수를 설정하세요:

- `DB_HOST`: 데이터베이스 호스트
- `DB_USER`: 데이터베이스 사용자 이름
- `DB_PASSWORD`: 데이터베이스 비밀번호
- `DB_NAME`: 데이터베이스 이름 