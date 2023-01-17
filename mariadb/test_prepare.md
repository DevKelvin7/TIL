# 데이터베이스 

## 데이터베이스의 개요
---
### 1. 데이터베이스 특징
- 무결성: 오류가 없는 정확한 데이터 확보
- 중복 최소화: 동일한 데이터는 가능한 하나의 테이블에 저장
- 독립성: 응용 프로그램은 DBMS변경에 영향받지 않아야함
- 보안성: 사용자별 데이터에 대한 접근 권한 관리
- 안정성: 데이터 유실 및 하드웨어 문제 발생 시 복원 가능

## SQL 기본
---
### 1. DML(데이터 조작 언어)
- 데이터 조작에 사용되는 언어
- SELECT, INSERT, UPDATE, DELETE
- DML은 테이블을 대상으로 하며, 테이블이 정의 되어 있어야함
- 트랜젝션이 발생하는 SQL
  - DML 중 데이터 변경 SQL 문장 실행 시 결과를 임시로 저장하여, 필요시 SQL 취소가 가능함

### 2. DDL(데이터 정의 언어)
- 데이터베이스의 개체(데이터베이스, 테이블, 뷰, 인덱스)를 관리하는 언어
- CREATE, ALTER, DROP
- DDL SQL은 수행 즉시 DBMS에 적용됨
  - DDL SQL 수행 취소 불가(기존 DML 수행 SQL문 포함)

### 3. DCL(데이터 제어 언어)
- 사용자에게 데이터베이스 내 권한을 부여하거나 제거를 위한 구문
- GRANT, REVOKE
- 데이터 베이스 개체별 SQL 명령문에 대한 권한 부여

### 4. TCL(트랜젝션 제어 언어)
- 데이터 변경내용을 DBMS에 반영, 취소
- COMMIT, ROLLBACK
- 데이터 변경 SQL중 오류 등의 이유로 취소 시 트랜젝션 단위로 처리함

## SQL 명령어 모음
---
### 1. 데이터 조회 
- Database 조회
  - ``` SHOW DATABASE;```
- Database 선택
  - ```USE 데이터베이스명;```
- Table 조회
  - ```SHOW TABLES;```
- Table 구조 조회 
  - ```DESC|DESCRIBE 테이블명```
- SELECT 기본 구문
  - ```mysql
    SELECT 조회 표현식
    [FROM] 테이블 명
    [WHERE] 조건식
    [GROUP BY] 컬럼명
    [HAVING] 집계 조건식
    [ORDER BY] 컬럼명 [ASC|DESC]
    [LIMIT] 조회 ROW 개수
    ```

