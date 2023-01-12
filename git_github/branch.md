# branch
2023년 1월 13일 (금요일)
## 1. branch 정의
---
> git에서 branch란 나뭇가지처럼 여러 갈래로 작업 공간을 나누어 독립적으로 작업을 할 수 있도록 도와주는 git의 도구

- 장점
  1. branch는 독립 공간을 형성하기 때문에 원본(master)에 대해 안전합니다.
  2. 하나의 작업은 하나의 branch로 나누어 진행되므로 체계적인 개발이 가능합니다.
  3. 특히나 git은 브랜치를 만드는 속도가 빠르며, 용량도 적게 사용됩니다.

## 2. git branch
---
```bash
# 브랜치 목록 확인
$git branch
# 원격 저장소의 브랜치 목록 확인
$git branch -r
# 새로운 브랜치 생성
$git branch <branch name>
# 특정 커밋 기준으로 브랜치 생성
$git branch <branch name> <commit id>
# 특정 브랜치 삭제
$git branch -d <branch name> 
```
## 3. git switch
---
> 현재 브랜치에서 다른 브랜치로 HEAD를 이동시키는 명령어
> ```HEAD```란 현재 브랜치를 가리키는 포인터를 의미합니다.

```bash
# 다른 브랜치로 이동
$git switch <other branch name>
# 브랜치를 새로 생성과 동시에 이동
$git switch -c <branch name>
# 특정 커밋 기준으로 브랜치 생성과 동시에 이동
$git switch -c <branch name> <commit id>
```