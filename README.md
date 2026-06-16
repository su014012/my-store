# 💰 우리집 가계부

스마트 재정 관리 웹 애플리케이션

## 📱 화면 구성

| 화면 | 파일 | 설명 |
|---|---|---|
| 대시보드 | index.html | 월별 요약, 차트, 마감 처리 |
| 가계부 관리 | ledger.html | 수입/지출 등록 및 조회 |
| 일/월별 조회 | inquiry.html | 기간별 내역 검색 |
| 고정지출 관리 | fixed.html | 정기 지출 항목 관리 |
| 부채 관리 | debt.html | 대출/할부 상환 관리 |
| 지출 분석 그래프 | graph.html | 카테고리별 지출 분석 |
| 월별 리포트 | report.html | 월별 결산 및 JSON 백업 |

## 💾 데이터 관리

- 데이터는 브라우저 **localStorage**에 저장됩니다
- **월별 리포트 → JSON 저장** 버튼으로 백업 가능
- 기기 변경 시: JSON 파일을 **대시보드 → 💾 데이터 관리 → JSON 불러오기**로 복원

## 🚀 배포 방법

### 1. GitHub에 올리기
```bash
git init
git add .
git commit -m "우리집 가계부 초기 배포"
git remote add origin https://github.com/YOUR_USERNAME/my-store.git
git push -u origin main
```

### 2. Vercel 연결
1. [vercel.com](https://vercel.com) 로그인
2. **Add New Project** → GitHub 저장소 선택
3. 설정 변경 없이 **Deploy** 클릭
4. 배포 완료 후 URL 접속

## 📋 localStorage 키

| 키 | 내용 |
|---|---|
| `household_ledger` | 가계부 내역 |
| `household_fixed` | 고정지출 항목 |
| `household_debt` | 부채 항목 |
| `household_pay_history` | 상환 이력 |
| `fixed_history` | 월 마감 이력 |
