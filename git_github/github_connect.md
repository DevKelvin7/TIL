# Github 
2023년 1월 13일 (금요일)

## 원격 저장소(Remote Repository)
---
### 1. 로컬 저장소와 원격 저장소 연결
1. 원격 저장소가 잘 생성되었는지 확인 후, 저장소의 주소를 복사합니다.
2. git init을 통해 로컬 저장소를 생성합니다.
```bash
git init
```
3. git remote
```bash
git remote add origin [원격저장소 repository link]
```
- 조회 : git remote -v
- 삭제 : git remote rm origin

### 2. 원격 저장소에 업로드
---
1. 로컬 저장소에서 커밋 생성
```bash
git status
git add [file name]
git commit -m "comment"
```
2. git push
```bash
git push origin -u master
git push origin master
```
