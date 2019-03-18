# [ Go Survey ] WebApp

_Last Modified: 2019-03-18_<br>
저장소: https://github.com/AnnYKim/goSurvey

## 19-03-11

- 파일 목록은 index.html에 정리되어있습니다.
- 고서베이 작업 부분은 html_bs/ 내에 존재합니다.
- 고서베이는 css/style.css를 사용합니다.
- 블캠 작업 부분은 html_bc/ 내에 존재합니다.
- 블캠은 css/style_bc.css를 사용합니다.
- 고보트 이미지 교체 부분은 images/ 폴더 내 이미지만 교체해주세요.
- js/폴더 내 bc.js와 test.js는 동작 확인용이니 지우셔도 됩니다.
- 마크업 구조 및 클래스 네임은 기존 고보트와 거의 유사합니다. 전달사항은 주석 참고 부탁드립니다!

---

## 19-03-12

- 수정사항(슬라이더 라이브러리 변경, 드래그앤드롭 라이브러리 추가, step3 마크업 분리) 반영했습니다.
- index_190312.html을 참고하시거나 기존 index.html에서 초록색으로 칠한 부분에 해당합니다.

---

## 19-03-18

수정사항 반영했습니다.
마크업만 수정하시면 되며, CSS는 교체하실 필요가 없습니다.<br>
**[190318]** 로 주석 검색하시면 됩니다~!

### 1. 결과숨김 switch 버튼 추가 및 여부 표시

- (03-01)create_step1.html에서 아래와 같이 추가했습니다.

```
<li>
  <div class="create-toggle">
    <p class="toggle-title">결과 숨김</p>
    <input id="option-hide-result" type="checkbox" class="toggle-checkbox" checked />
    <label for="option-hide-result" class="toggle-switch">
      <div class="toggle-body"></div>
      <div class="toggle-head"></div>
    </label>
  </div>
</li>
```

- (03-06)create_step4.html에서 아래와 같이 추가했습니다.

```
<div class="option-block">
  <div class="option-name">결과 숨김</div>
  <div class="option-setting active">선택</div>
</div>
```

- **goVote도 동일합니다!!!**<br>
  혹시 몰라서 확인용으로 html_goVote/도 함께 첨부하긴 했지만, 현재 개발된 것에 맞춰 마크업 복사 후 텍스트만 수정하시면 되겠습니다.<br>
  css/ 내에 govote(TEST).css가 추가됐는데, 오로지 이 수정사항 확인용이니 지워주세요!! (이미지도 마찬기지로 교체하지 않으셔도 됩니다)

### 2. export as csv button 부활

- (05-01)과 (05-02)에서 .button-next의 텍스크를 Export로 변경 후 기능 연결해주시면 될 것 같습니다.

### 3. details에서 뒤로가기(<) 대신 닫기(X) 아이콘으로 수정

- (05-01)과 (05-02)에서 .icon-back 대신 .icon-close로 수정해주세요.

```
<button class="icon-container">
  <i class="icon icon-close"></i>
</button>
```
