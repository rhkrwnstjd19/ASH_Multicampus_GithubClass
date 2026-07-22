# Git & GitHub 기초 가이드

Git과 GitHub 사용법, 그리고 기초 마크다운 문법을 정리한 문서입니다.

---

## 1. Git이란?

- **Git**: 내 컴퓨터에서 코드의 변경 이력을 관리하는 **버전 관리 시스템**
- **GitHub**: Git으로 관리하는 코드를 **온라인에 저장하고 공유**하는 웹 서비스

```
[내 컴퓨터]  ──push──▶  [GitHub 저장소]
   Git                    (원격)
```

---

## 2. 자주 쓰는 Git 명령어

### 저장소 시작하기

```bash
git init                 # 현재 폴더를 Git 저장소로 만들기
git clone <저장소 주소>    # GitHub 저장소를 내 컴퓨터로 복제
```

### 기본 작업 흐름 (가장 중요!)

```bash
git status               # 현재 변경 상태 확인
git add <파일명>          # 파일을 스테이지에 올리기
git add .                # 모든 변경 파일 올리기
git commit -m "메시지"    # 변경 내용을 커밋(기록)
git push                 # GitHub에 업로드
git pull                 # GitHub의 최신 내용 내려받기
```

### 흐름 요약

```
수정 → git add → git commit → git push
```

### 브랜치 다루기

```bash
git branch               # 브랜치 목록 보기
git branch <이름>         # 새 브랜치 만들기
git checkout <이름>       # 브랜치 이동
git checkout -b <이름>    # 만들면서 바로 이동
git merge <이름>          # 브랜치 병합
```

### 기록 확인

```bash
git log                  # 커밋 기록 보기
git log --oneline        # 한 줄로 간단히 보기
```

---

## 3. GitHub 협업 흐름

1. 저장소를 **Fork** 또는 **Clone**
2. 새 **브랜치** 생성 후 작업
3. 변경 내용 **commit & push**
4. **Pull Request(PR)** 로 병합 요청
5. 리뷰 후 **Merge**

---

## 4. 기초 마크다운(Markdown) 문법

### 제목

```markdown
# 제목 1
## 제목 2
### 제목 3
```

### 강조

```markdown
**굵게**      → **굵게**
*기울임*      → *기울임*
~~취소선~~    → ~~취소선~~
```

### 목록

```markdown
- 순서 없는 목록
- 항목 2
  - 하위 항목

1. 순서 있는 목록
2. 항목 2
```

### 링크 & 이미지

```markdown
[링크 텍스트](https://github.com)
![이미지 설명](이미지주소.png)
```

### 코드

````markdown
`인라인 코드`

```python
print("코드 블록")
```
````

### 인용 & 구분선

```markdown
> 인용문입니다.

---
```

### 표

```markdown
| 이름 | 나이 |
|------|------|
| 홍길동 | 20 |
| 김철수 | 25 |
```

| 이름 | 나이 |
|------|------|
| 홍길동 | 20 |
| 김철수 | 25 |

---

## 5. 참고 링크

- [Git 공식 문서](https://git-scm.com/doc)
- [GitHub 가이드](https://docs.github.com)
- [마크다운 문법 정리](https://www.markdownguide.org)
