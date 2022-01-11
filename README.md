<p align="middle" >
  <img src="https://techcourse-storage.s3.ap-northeast-2.amazonaws.com/0fefce79602043a9b3281ee1dd8f4be6" width="400">
</p>
<h2 align="middle">페이먼츠</h2>
<p align="middle">React 모바일 페이먼츠 애플리케이션</p>
</p>


# 미션 키워드 
- Component
- Props
- Controlled & Uncontrolled Components
- Storybook
- Hooks API
- Context API

# Step1 - Component-Driven Development
## 🚀 Getting Started
> `Component-Driven Development` 에 따라 UI를 구성하고 재사용 가능한 `Component`를 작성합니다.
 
✔️ `모바일 타겟`의 웹 앱을 구현하며 사용하기 `편리한 모바일 UI/UX`에 대해 고민해봅니다.
✔️ 다른 라이브러리나 프레임워크 없이 오로지 `React`만으로 상태를 관리하고 컴포넌트를 설계합니다.
✔️ `재사용 가능한 Component`를 직접 작성하고 사용합니다.
✔️ `Controlled` & `Uncontrolled Components`에 입각하여 `Form`을 핸들링합니다.
✔️ [Github Repository](https://github.com/next-step/react-payments)
✔️ [Figma](https://www.figma.com/file/uDHr0HNizeHMNpCbxT69KV/payments)
## 📝 Requirements
### 필수 요구사항 
- [ ] `Storybook` 상호 작용 테스트
- [ ] `재사용 가능한 Component` 작성
#### 카드 추가
- [ ] `<`(뒤로가기) 버튼 클릭 시, 카드 목록 페이지로 이동한다.
- [ ] 카드 번호를 입력 받을 수 있다.
    - [ ] 카드 번호입력 폼에 라벨을 보여준다.
    - [ ] 카드 번호는 숫자만 입력가능하다.
    - [ ] 카드 번호 4자리마다 `-`가 삽입된다.
    - [ ] 카드 번호는 실시간으로 카드 UI에 반영된다.
    - [ ] 카드 번호는 앞 8자리만 숫자로 보여지고, 나머지 숫자는 `*`로 보여진다.
    - [ ] 카드 번호 앞 8자리로 카드사를 추정하여 그 테마를 카드 UI에 반영한다.
    - [ ] 카드사가 선택되고 유효한 카드 번호 16자리를 모두 입력하면, 자동으로 만료일로 focus된다.
    - [ ] 카드 앞 8자리 숫자를 입력하고 카드사가 선택되지 않은 경우, 나머지 카드 번호 입력 시도 시, 카드사 선택 모달이 보여진다.
    - [ ] 유효하지 않은 카드 번호를 입력하면, 입력 폼 아래에 에러 메시지를 보여준다.
- [ ] 만료일을 입력 받을 수 있다.
    - [ ] 만료일 입력 폼에 라벨을 보여준다.
    - [ ] `MM / YY` 로 placeholder를 적용한다.
    - [ ] 월, 년 사이에 자동으로 `/`가 삽입된다.
    - [ ] 만료일은 실시간으로 카드 UI에 반영된다.
    - [ ] 월은 1이상 12이하 숫자여야 한다.
    - [ ] 월, 년 입력이 유효하면 보안코드 입력으로 focus된다
    - [ ] 유효하지 않은 만료일을 입력하면, 입력 폼 아래에 에러 메시지를 보여준다.
- [ ] 보안코드를 입력 받을 수 있다.
    - [ ] 카드 보안코드 입력 폼에 라벨을 보여준다.
    - [ ] 보안코드는 `*`으로 보여진다.
    - [ ] 보안코드 3자리가 입력되면 카드 비밀번호 입력으로 focus된다.
    - [ ] 보안코드는 숫자만 입력가능하다.
    - [ ] 유효하지 않은 보안코드를 입력하면, 입력 폼 아래에 에러 메시지를 보여준다.
- [ ] 카드 비밀번호의 앞 2자리를 입력 받을 수 있다.
    - [ ] 카드 비밀번호 입력 폼에 라벨을 보여준다.
    - [ ] 카드 비밀번호는 각 폼마다 한자리 숫자만 입력가능하다.
    - [ ] 첫자리 입력이 완료되면 둘째자리 입력으로 focus된다.
    - [ ] 카드 번호 입력 시, `*`으로 보여진다.
    - [ ] 유효하지 않은 카드 비밀번호를 입력하면, 입력 폼 아래에 에러 메시지를 보여준다.
- [ ] 카드 소유자 이름을 입력 받을 수 있다.
    - [ ] 카드 소유자 이름 입력 폼 라벨을 보여준다.
    - [ ] 이름은 30자리까지 입력할 수 있다.
    - [ ] 이름 입력 폼 위에, 현재 입력 자릿수와 최대 입력 자릿수를 실시간으로 보여준다.
- [ ] 클릭 시, 카드 등록 완료 페이지로 이동한다.
### 심화 요구사항 (선택사항)
- [ ] `Storybook` 단위 테스트
- [ ] 유효성 검증 실패에 대한 UI/UX 추가
- [ ] 카드사 선택
  - [ ] 카드사를 선택하면 모달이 닫히고, 그 테마를 카드 UI에 반영한다.
  - [ ] 카드사를 선택하지 않아도 모달을 닫을 수 있다.
- [ ] 보안코드 툴팁
  - [ ] 클릭 시, 보안코드 관련 안내 메시지를 보여준다.
  - [ ] focusout 시, 툴팁이 닫힌다.
- [ ] 가상 키보드
  - [ ] 마스킹 처리된 값 입력시 사용
  - [ ] 숫자를 랜덤으로 배열

# Step2 - Controlled & Uncontrolled Components + Context API
## 🚀 Getting Started
> `Component-Driven Development` 에 따라 UI를 구성하고 재사용 가능한 `Component`를 작성합니다.
 
✔️ `모바일 타겟`의 웹 앱을 구현하며 사용하기 `편리한 모바일 UI/UX`에 대해 고민해봅니다.
✔️ 다른 라이브러리나 프레임워크 없이 오로지 `React`만으로 상태를 관리하고 컴포넌트를 설계합니다.
✔️ React `Context API`를 활용합니다.
✔️ `재사용 가능한 Component`를 직접 작성하고 사용합니다.
✔️ `Controlled` & `Uncontrolled Components`에 입각하여 `Form`을 핸들링합니다.
✔️ [Github Repository](https://github.com/next-step/react-payments)
✔️ [Figma](https://www.figma.com/file/uDHr0HNizeHMNpCbxT69KV/payments)
## 📝 Requirements
### 필수 요구사항 
- [ ] `Storybook` 상호 작용 테스트
- [ ] `Controlled` & `Uncontrolled Components`에 입각하여 `Form` 핸들링
- [ ] `Context API`를 활용해 전역 상태 관리 및 계층 재구성
#### 카드 추가 확인
- [ ] 이전 폼에서 입력된 카드를 보여준다.
- [ ] 카드 별칭을 입력할 수 있다.
    - [ ] placeholder는 `카드 별칭 (선택)`이다.
    - [ ] 빈 입력값인 경우, 카드사 이름이 별칭으로 저장된다.
    - [ ] 최대 길이는 10자리이다.
- [ ] 확인 버튼을 누르면, 카드 목록 페이지로 이동한다.
#### 카드 목록
- [ ] 카드 목록을 조회할 수 있다.
- [ ] 카드 목록은 최신순(내림차순)으로 정렬된다.
- [ ] 목록 최상단에 `+`을 누르면 카드 추가 페이지로 이동한다.
- [ ] 카드를 클릭하면, 카드 별칭 수정(카드 추가 완료 페이지)로 이동한다.
- [ ] 카드를 삭제할 수 있다.
### 선택 요구사항
- [ ] `Storybook` 스냅샷 테스트
- [ ] 비동기 통신
  - [ ] 다양한 도구를 활용 (예 JSON Server, Strapi 등등)
  - [ ] 등록된 카드 정보를 CRUD 합니다.
- [ ] 나열된 카드 클릭시 `카드 추가 확인` 화면 재활용
  - [ ] 별칭 수정 가능
