# README

<div align="center">
  <h1>🛍️ XMPY MALL</h1>
  <strong>카테고리별 상품 탐색부터 장바구니, 결제, 리뷰까지 — 쇼핑의 모든 것을 한 곳에서</strong>
</div>

<br />

## 📋 프로젝트 개요

- **프로젝트명**: XMPY MALL
- **팀명**: 1조
- **프로젝트 타입**: Full-stack Web Application (React + Spring Boot)

---

## 🎯 개발 배경

온라인 쇼핑몰의 핵심 기능인 **상품 탐색 → 장바구니 → 결제 → 리뷰** 흐름을 직접 구현하며, 실무에 가까운 쇼핑몰 서비스를 풀스택으로 경험하는 것을 목표로 제작되었습니다.

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

<table>
  <tbody>
    <tr>
      <td>홈 화면</td>
      <td>베스트 슬라이더</td>
    </tr>
    <tr>
      <td>
        <!-- 홈 화면 이미지를 여기에 첨부해 주세요 -->
      </td>
      <td>
        <!-- 베스트 슬라이더 이미지를 여기에 첨부해 주세요 -->
      </td>
    </tr>
  </tbody>
</table>

### 2. 상품 목록 & 상세

<table>
  <tbody>
    <tr>
      <td>카테고리 상품 목록</td>
      <td>상품 상세 페이지</td>
    </tr>
    <tr>
      <td>
        <!-- 카테고리 상품 목록 이미지를 여기에 첨부해 주세요 -->
      </td>
      <td>
        <!-- 상품 상세 페이지 이미지를 여기에 첨부해 주세요 -->
      </td>
    </tr>
  </tbody>
</table>

### 3. 장바구니 & 결제

<table>
  <tbody>
    <tr>
      <td>장바구니</td>
      <td>결제 페이지</td>
    </tr>
    <tr>
      <td>
        <!-- 장바구니 이미지를 여기에 첨부해 주세요 -->
      </td>
      <td>
        <!-- 결제 페이지 이미지를 여기에 첨부해 주세요 -->
      </td>
    </tr>
  </tbody>
</table>

### 4. 로그인 & 회원가입

<table>
  <tbody>
    <tr>
      <td>로그인</td>
      <td>회원가입</td>
    </tr>
    <tr>
      <td>
        <!-- 로그인 화면 이미지를 여기에 첨부해 주세요 -->
      </td>
      <td>
        <!-- 회원가입 화면 이미지를 여기에 첨부해 주세요 -->
      </td>
    </tr>
  </tbody>
</table>

### 5. 마이페이지

<table>
  <tbody>
    <tr>
      <td>유저 마이페이지</td>
      <td>관리자 페이지</td>
    </tr>
    <tr>
      <td>
        <!-- 유저 마이페이지 이미지를 여기에 첨부해 주세요 -->
      </td>
      <td>
        <!-- 관리자 페이지 이미지를 여기에 첨부해 주세요 -->
      </td>
    </tr>
    <tr>
      <td>상품 등록</td>
      <td>재고 관리</td>
    </tr>
    <tr>
      <td>
        <!-- 상품 등록 이미지를 여기에 첨부해 주세요 -->
      </td>
      <td>
        <!-- 재고 관리 이미지를 여기에 첨부해 주세요 -->
      </td>
    </tr>
  </tbody>
</table>

---

## 🛠️ 기술 스택

### Frontend

<p>
  <img src="https://img.shields.io/badge/React-19.2.0-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/JavaScript-ES2023-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Vite-8.0-646CFF?style=for-the-badge&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/Axios-1.13.5-5A29E4?style=for-the-badge&logo=axios&logoColor=white" />
  <img src="https://img.shields.io/badge/Zustand-5.0.11-764ABC?style=for-the-badge&logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/TanStack_Query-5.90.21-FF4154?style=for-the-badge&logo=react-query&logoColor=white" />
  <img src="https://img.shields.io/badge/React_Router_Dom-7.13.0-CA4245?style=for-the-badge&logo=react-router&logoColor=white" />
</p>
<p>
  <img src="https://img.shields.io/badge/Emotion-11.x-DB7093?style=for-the-badge&logo=emotion&logoColor=white" />
  <img src="https://img.shields.io/badge/Swiper-12.1.2-6332F6?style=for-the-badge&logo=swiper&logoColor=white" />
  <img src="https://img.shields.io/badge/React_Quill-3.8.3-FF4154?style=for-the-badge&logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/React_Toastify-11.0.5-FF6347?style=for-the-badge&logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/React_Spinners-0.17.0-888888?style=for-the-badge&logo=react&logoColor=white" />
</p>
<p>
  <img src="https://img.shields.io/badge/Supabase-2.98.0-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/Daum_Postcode_API-4.0.0-FFCD00?style=for-the-badge&logoColor=black" />
  <img src="https://img.shields.io/badge/jwt--decode-4.0.0-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white" />
</p>

### Backend

<p>
  <img src="https://img.shields.io/badge/Spring_Boot-3.5.10-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-17+-007396?style=for-the-badge&logo=java&logoColor=white" />
  <img src="https://img.shields.io/badge/MyBatis-3.0.5-000000?style=for-the-badge&logo=mybatis&logoColor=white" />
  <img src="https://img.shields.io/badge/Lombok-1.18.30-FF6347?style=for-the-badge&logo=java&logoColor=white" />
</p>

### Database

<p>
  <img src="https://img.shields.io/badge/MySQL-003545?style=for-the-badge&logo=mysql&logoColor=white" />
</p>

### Security

<p>
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=spring-security&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white" />
</p>

### 외부 서비스

<p>
  <img src="https://img.shields.io/badge/Supabase_Storage-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/Daum_우편번호_API-FFCD00?style=for-the-badge&logoColor=black" />
</p>

---

## 📂 프로젝트 폴더 구조

### Frontend

```bash
XMPY-MALL-FRONT/
└── src/
    ├── apis/
    │   ├── instance.js               # Axios 인스턴스 (JWT 헤더 설정)
    │   └── endpoints/                # API 호출 함수 모음
    │       ├── auth.js               # 로그인 / 회원가입
    │       ├── product.js            # 상품 조회 / 등록
    │       ├── order.js              # 주문 생성 / 조회
    │       ├── review.js             # 리뷰 조회 / 작성
    │       ├── stock.js              # 재고 조회 / 수정
    │       ├── category.js           # 카테고리 조회
    │       ├── user.js               # 유저 정보 조회 / 수정
    │       └── admin.js              # 관리자 전용 API
    ├── components/
    │   └── Spinner/                  # 로딩 스피너 공용 컴포넌트
    ├── constants/
    │   ├── menu.jsx                  # 라우트 및 메뉴 정의
    │   ├── colors.js                 # 색상 상수
    │   └── images.js                 # 이미지 상수
    ├── hooks/                        # 공용 커스텀 훅
    ├── layouts/
    │   ├── Header/                   # 헤더 (카테고리 드롭다운 포함)
    │   ├── Footer/                   # 푸터
    │   └── MainLayout/               # 공통 레이아웃 (Outlet)
    ├── pages/
    │   ├── Home/                     # 홈 (베스트 슬라이더)
    │   ├── Best/                     # 베스트 상품 페이지
    │   ├── SubMenuPage/              # 카테고리별 상품 목록
    │   ├── ProductDetailPage/        # 상품 상세 (옵션 선택, 리뷰)
    │   ├── CartPage/                 # 장바구니
    │   ├── PaymentPage/              # 결제
    │   ├── Signin/                   # 로그인
    │   ├── Signup/                   # 회원가입
    │   ├── Mypage/
    │   │   ├── pages/UserPage/       # 유저 마이페이지 (주문내역, 리뷰, 내정보)
    │   │   └── pages/OwnerPage/      # 관리자 마이페이지
    │   ├── AddProduct/               # 상품 등록 (관리자)
    │   └── StockManagePage/          # 재고 관리 (관리자)
    ├── routes/
    │   ├── AppRoutes.jsx             # 전체 라우팅 구성
    │   ├── UserRoute.jsx             # 유저 전용 보호 라우트
    │   └── AdminRoute.jsx            # 관리자 전용 보호 라우트
    ├── stores/
    │   └── authStore.js              # Zustand 인증 전역 상태
    ├── quill/                        # Quill 에디터 래퍼
    └── supabase/
        └── supabase.js               # Supabase 클라이언트 설정
```

### Backend

```bash
XMPY-MALL-BACK/
└── src/
    └── main/
        ├── java/com/xmpy/demo/
        │   ├── config/
        │   │   └── SecurityConfig.java       # Spring Security 설정
        │   ├── controller/
        │   │   ├── AuthController.java       # 회원가입 / 로그인
        │   │   ├── ProductController.java    # 상품 CRUD
        │   │   ├── OrderController.java      # 주문 처리
        │   │   ├── ReviewController.java     # 리뷰 작성 / 조회
        │   │   ├── StockController.java      # 재고 관리
        │   │   ├── CategoryController.java   # 카테고리 조회
        │   │   ├── MyPageController.java     # 마이페이지
        │   │   └── AdminController.java      # 관리자 전용
        │   ├── dto/
        │   │   ├── req/                      # 요청 DTO
        │   │   └── res/                      # 응답 DTO
        │   ├── entity/                       # 엔티티 (User, Product, Orders, Review 등)
        │   ├── jwt/
        │   │   ├── JwtUtil.java              # JWT 생성 / 검증
        │   │   └── JwtAuthenticationFilter.java
        │   ├── mapper/                       # MyBatis Mapper 인터페이스
        │   └── service/                      # 비즈니스 로직
        └── resources/
            ├── mappers/                      # MyBatis XML SQL 매핑
            └── application.yaml             # 애플리케이션 설정
```
