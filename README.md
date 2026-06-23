# 🛍️ XMPY MALL

> 카테고리별 상품 탐색부터 장바구니, 결제, 리뷰까지 — 쇼핑의 모든 것을 한 곳에서

---

## 📋 프로젝트 개요

- **프로젝트명**: XMPY MALL
- **팀명**: XMPY
- **프로젝트 타입**: Full-stack Web Application (React + Spring Boot)

## 🎯 개발 배경

온라인 쇼핑몰의 핵심 기능인 상품 탐색 → 장바구니 → 결제 → 리뷰 흐름을 직접 구현하며, 실무에 가까운 쇼핑몰 서비스를 풀스택으로 경험하는 것을 목표로 제작되었습니다.

카테고리 기반 상품 분류, 베스트 상품 노출, 사이즈/색상 옵션별 재고 관리, 구매 후 리뷰 작성까지 실제 이커머스 플로우를 그대로 구현하였습니다.

---

## ✨ 주요 기능

### 🏠 홈 & 상품 탐색

**홈 화면**
- 베스트 상품을 Swiper 슬라이더로 노출
- 카테고리 드롭다운 네비게이션을 통한 빠른 이동

**베스트 페이지**
- 카테고리별 베스트 상품 목록 제공

**카테고리 상품 목록 페이지 (SubMenuPage)**
- 카테고리 상세별 상품 리스트 조회
- 페이지네이션 기반 탐색

**상품 상세 페이지**
- 상품 썸네일, 이름, 가격, 상세 설명 제공
- 사이즈 / 색상 옵션 선택 후 장바구니 담기
- 구매자 리뷰 목록 및 별점 확인

### 🛒 장바구니 & 결제

**장바구니 페이지**
- 담은 상품 목록 확인 및 수량 조절
- 선택 상품 삭제 및 전체 금액 합산

**결제 페이지**
- 배송지 입력 (Daum 우편번호 API 연동)
- 주문 상품 최종 확인 및 결제 처리

### ⭐ 리뷰
- 구매 완료된 상품에 한해 리뷰 작성 가능
- Quill 에디터를 이용한 서식 있는 리뷰 작성
- 별점 기반 평가

### 👤 마이페이지

**일반 유저**
- 내 정보 조회 및 수정 (프로필 이미지 포함)
- 주문 내역 조회
- 내가 작성한 리뷰 확인

**관리자 (OwnerPage)**
- 상품 등록 페이지: 카테고리, 이미지, 상세 정보, 옵션(사이즈/색상/재고) 입력
- 재고 관리 페이지: 상품별 사이즈/색상별 재고 수량 수정

### 🔐 인증
- 이메일 / 비밀번호 회원가입 및 로그인
- 회원가입 시 입력값 형식 검증
- JWT 기반 인증 (AccessToken → LocalStorage 저장)
- 역할 기반 접근 제어 (일반 유저 / 관리자)

---

## 🚀 주요 기능 화면

### 1. 홈
- 홈 화면: 베스트 슬라이더 표시

### 2. 상품 목록 & 상세
- 카테고리별 (상의 / 하의 / 아우터) 상품 목록 조회
- 상품 상세 페이지 및 주문 기능

### 3. 장바구니 & 결제
- 장바구니 담기 / 수량 조절 / 삭제
- 결제 페이지에서 배송지 입력 및 주문 완료

### 4. 로그인 & 회원가입
- 이메일/비밀번호 로그인
- 로그인 성공 시 일반 유저 / 관리자 역할에 따라 분기
- 회원가입 시 유효성 검사

### 5. 마이페이지
- 사용자 마이페이지: 주문 내역, 리뷰 확인
- 관리자 마이페이지: 주문 관리, 리뷰 관리, 상품 추가, 재고 관리, 옵션 추가

---

## 🛢️ ERD

- 추후 첨부 예정

---

## 🛠️ 기술 스택

| 분류 | 기술 |
|------|------|
| Frontend | React, Zustand, Axios, Swiper, Quill Editor |
| Backend | Spring Boot, Spring Security, MyBatis, JWT |
| Database | MySQL |
| 외부 서비스 | Supabase (이미지 스토리지), Daum 우편번호 API |

---

## 📂 Project Structure

### 🖥 Frontend
```
XMPY-MALL-FRONT/
└── src/
    ├── apis/
    │   ├── instance.js
    │   └── endpoints/
    │       ├── admin.js
    │       ├── auth.js
    │       ├── category.js
    │       ├── order.js
    │       ├── product.js
    │       ├── review.js
    │       ├── stock.js
    │       └── user.js
    ├── components/
    ├── constants/
    ├── hooks/
    ├── layouts/
    ├── pages/
    │   ├── Home/
    │   ├── Best/
    │   ├── SubMenuPage/
    │   ├── ProductDetailPage/
    │   ├── CartPage/
    │   ├── PaymentPage/
    │   ├── Signin/
    │   ├── Signup/
    │   ├── Mypage/
    │   ├── AddProduct/
    │   └── StockManagePage/
    ├── routes/
    ├── stores/
    └── supabase/
```

### 🖥 Backend
```
XMPY-MALL-BACK/
└── src/main/java/com/xmpy/demo/
    ├── config/
    ├── controller/
    ├── dto/
    ├── entity/
    ├── jwt/
    ├── mapper/
    ├── service/
    └── resources/
        └── mappers/
```
