# PlantPick 리뉴얼 첫 화면 시안

## 실행
preview.html은 이미지와 폰트가 내장된 단일 파일이므로 이 파일만 브라우저에서 열면 됩니다. 개발용 index.html을 열 때는 assets 폴더를 같은 위치에 유지하세요. 운영 사이트에 배포하거나 데이터를 변경하지 않은 독립 시안입니다.

## 반영 내용
- 기존 Vegan & Green 로고 원본 유지
- Pretendard Variable을 로컬 포함하여 전체 적용
- 비건·오가닉 분위기의 자연광 히어로
- 기존 카테고리 8종을 실사형 AI 샘플로 교체
- 상품 AI 샘플 4종, 필터·검색·상품 상세·샘플 장바구니
- PC 및 모바일 반응형

## 검토 근거 (2026-10-27)
- https://plantpickstore.com/ : 기존 8개 분류, 생활 동사형 탐색, 로고와 사업자 정보 확인. 동일 토너가 FESTA PICK, MD PICK, NEW AT FESTA, MY DAILY PICK에 반복됨.
- https://www.oasis.co.kr/main : 검색·전체 카테고리, 대형 기획전, 실사 카테고리 바로가기, 특가 및 BEST의 상품 중심 흐름 참고. 오아시스 이미지나 코드는 복제하지 않음.
- 사용자 첨부 이미지: 기존 8개 아이콘 카테고리 확인.

## 제작 방식 및 실제 운영과의 구분
| 파일 | 제작 방식과 주의점 |
|---|---|
| index.html | 직접 코드 작성. 레이아웃·반응형·UI 동작 시안, 실제 주문·결제 미연동 |
| assets/hero.png | AI 생성(openai-codex / chatgpt-image-generation). 비건 식탁 연출 사진, 실제 상품 아님 |
| assets/product-*.jpg | 동일 모델로 AI 생성 후 4종 분할. 상품명과 가격은 가상 예시 |
| assets/cat-*.jpg | 동일 모델로 AI 생성 후 8종 분할. 실제 상품이나 인증 근거 아님 |
| assets/logo.png | 기존 운영몰 로고 원본 다운로드, AI 생성 및 재디자인 아님 |
| assets/PretendardVariable.woff2 | Pretendard v1.3.9 원본, SIL OFL 1.1, Copyright 2021 Kil Hyung-jin |

상품 성분·중량·유기농/비건 인증·할인율·배송 보장은 확인되지 않아 표시하지 않았습니다. 실제 적용 전 운영 데이터와 상품별 확인이 필요합니다. 샘플 장바구니는 새로고침 시 초기화됩니다. 카테고리 펼침 메뉴와 전체 상품/브랜드관/약관은 기존 운영몰을 새 탭으로 엽니다.
