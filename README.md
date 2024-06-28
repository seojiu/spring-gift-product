# spring-gift-product

# 구현할 기능 목록 정리

## GET
### 1. 전체 상품 조회
### 2. id로 상품 검색

## POST
### 3. 상품 추가

## PUT
### 4. 상품 수정

## Delete
### 5. 상품 삭제

------------------------


# 관리자 화면

### 1. 상품 조회(기본 화면)

### 2. 상품 추가

### 3. 상품 수정

### 4. 상품 삭제

### 상품 이미지의 경우, 파일을 업로드하지 않고 URL을 직접 입력한다


#### ProductService 클래스 수정 (id는 사용자가 지정할 수 없고 상품이 추가 될 때 마다 ++가 되도록 만들어야함)

#### ProductController 클래스 수정


![img_2.png](img_2.png)

#### 상품 추가 버튼

#### 상품 마다 수정 버튼, 삭제 버튼

#### 총 3 페이지 필요함 (메인 화면, 수정 페이지, 상품 추가 페이지)


--------------------------------------------------


## 데이터베이스 적용

### 1. 메모리에 저장하고 있던 모든 코드를 제거하고 H2 데이터베이스를 사용하도록 변경한다.
### 2. 사용하는 테이블은 애플리케이션이 실행될 때 구축되어야 한다.



### 스키마 스크립트는 schema.sql, 데이터 스크립트는 data.sql
### 스키마 및 데이터 스크립트의 위치는 각각 spring.sql.init.schema-locations 및 spring.sql.init.data-locations를 사용하여 사용자 지정할 수 있다.