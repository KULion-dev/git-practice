# 🚀 KULion Git 실습 세션

이 레포지토리는 Git과 GitHub의 핵심 워크플로우를 직접 경험해보기 위한 실습 공간입니다.  
처음 시작하는 분들도 차근차근 따라 하실 수 있도록 구성되어 있습니다.

---

## 🛠 실습 진행 순서 (Step-by-Step)

모든 과정은 터미널(Terminal) 또는 Git Bash에서 진행합니다.

### 0 레포지토리 Fork
가장 먼저 github에서 이 레포지토리를 Fork해서 가져옵니다.

### 1️⃣ 레포지토리 클론 (Clone)
원격 저장소의 코드를 내 컴퓨터로 가져옵니다.
```bash
git clone https://github.com/KULion-dev/git-practice.git
cd git-practice
```

### 2️⃣ 본인 이름의 브랜치 생성 (Branch)
메인 코드(main)를 보호하기 위해 본인만의 작업 공간을 만듭니다.  
*브랜치 이름은 영문 이름으로 생성해 주세요. (예: `jinmo-yang`)*
```bash
git checkout -b [본인이름]
```

### 3️⃣ [본인이름].md 생성 (Create)
`[본인이름].md` 파일을 생성해서 간단한 자기소개를 자유롭게 추가합니다.

### 4️⃣ 변경 사항 커밋 및 푸시 (Commit & Push)
작업한 내용을 저장하고 GitHub 서버로 올립니다.
```bash
git add .
git commit -m "feat: [본인이름] 참여 완료"
git push origin [본인이름]
```

### 5️⃣ Pull Request (PR) 생성
GitHub 웹사이트에서 `Compare & pull request` 버튼을 눌러 PR을 생성합니다.
- **Base:** `main` ← **Compare:** `[본인이름]`
- 제목은 `[이름] 깃 실습 완료`로 작성해 주세요.

### 6️⃣ 병합 확인 및 최신화 (Pull)
PR이 승인되어 `main`에 합쳐졌다면, 다시 로컬의 `main`을 최신 상태로 업데이트합니다.
```bash
git checkout main
git pull origin main
```

