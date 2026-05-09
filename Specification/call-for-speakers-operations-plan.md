# Call For Speakers Operations Plan

이 문서는 새 call for speakers 공지를 추가하고, 필요한 경우 종료된 공지를 archive로 전환할 때 사용하는 반복 가능한 작업 계획이다.

## 목적

- 새 open call이 홈과 목록에서 바로 보이도록 한다.
- 종료하기로 결정된 공지를 archive 상태로 정리한다.
- 새 공지를 추가해도 기존 open call이 자동으로 종료되는 것은 아님을 명확히 한다.
- call for speakers 운영 작업의 순서와 완료 기준을 명확히 한다.

## 적용 범위

- `Pages/CallForSpeakers/<slug>.html`
- `Pages/call-for-speakers.html`
- `index.html`
- `images/call-for-speakers/`

## 작업 순서

### 1. 기존 open call 종료 여부 확인

- 새 open call을 추가하기 전에 현재 open 상태인 call for speakers 항목을 확인한다.
- 현재 open call이 있다면, 작업자나 요청자에게 해당 항목을 종료하고 archive로 정리할지 반드시 확인한다.
- 종료하기로 확인된 항목만 archive로 전환한다.
- 종료하지 않기로 한 항목은 open 상태로 유지하며, 새 open call과 함께 목록에 노출될 수 있다.

### 2. 종료하기로 한 open call을 archive로 정리

- 공지 상세 페이지의 상태 문구를 완료형 아카이브 기준으로 맞춘다.
- 초대, 모집, 신청 유도 문구가 있으면 제거한다.
- archive에는 공지 내용 자체에 기반한 설명만 남긴다.
- 홈과 목록에서 더 이상 진행 중인 공지처럼 보이지 않게 한다.

### 3. 새 open call 상세 페이지 생성

- 가장 최근 call for speakers 페이지를 기준으로 새 공지 상세 페이지를 만든다.
- 대표 이미지와 안내 이미지를 올바른 순서로 연결한다.
- `Theme Overview`를 넣어 공지의 맥락을 설명한다.
- 모집 포인트, 질문 목록, 진행 형식을 분리해 쓴다.
- CTA 버튼은 신청 링크와 연결한다.

### 4. 목록 페이지 반영

- `Pages/call-for-speakers.html`은 공개 목록 페이지 `https://ctalkdiversity.org/Pages/call-for-speakers.html`의 소스 파일이다.
- 새 open call 상세 페이지를 만들었다면, 반드시 `Pages/call-for-speakers.html`의 공지 목록에도 새 항목을 추가한다.
- 새 항목은 목록의 첫 번째 공지 카드/게시물 위치에 배치한다. 즉, 기존 항목들보다 위에 있어야 하며 공개 페이지에서도 가장 상단 항목으로 보여야 한다.
- 기존 open call은 종료 여부 확인 결과에 따라 open 상태로 유지하거나 archive 상태로 정리한다.
- 여러 open call이 동시에 유지되는 경우, 최신 open call을 위에 두고 기존 open call은 그 아래에 open 상태로 남긴다.
- 종료된 공지는 archive 상태로 유지한다.
- 카드 제목, 요약, 이미지, 링크가 실제 파일과 일치하는지 확인한다.

### 5. 홈 페이지 반영

- `index.html`의 최신 call for speakers 카드 또는 섹션을 새 open call로 교체한다.
- 외부 사용자가 첫 화면에서 최신 open call을 확인할 수 있어야 한다.

### 6. 검증

- 홈, 목록, 상세 페이지의 `href`와 `src`를 확인한다.
- 기존 open call의 종료 여부를 확인한 기록이나 작업 맥락이 남아 있는지 확인한다.
- archive 상태로 옮긴 공지가 있다면 완료형으로 보이는지 확인한다.
- archive 페이지에 남는 문구가 초대/모집 중심이 아니라 내용 요약 중심인지 확인한다.
- 필요 시 공지 결과물 링크, 후속 conference 링크, 뉴스 링크, podcast 링크를 추가할 수 있는 위치가 있는지 확인한다.
- 새 open call이 실제 공개 entry point에서 노출되는지 확인한다.
- 브라우저에서 외부 사용자 관점으로 한 번 더 확인한다.

## 완료 기준

- 새 open call이 `index.html`에 노출된다.
- 새 open call이 `Pages/call-for-speakers.html`에 추가되어 있으며, 공개 목록 페이지 `https://ctalkdiversity.org/Pages/call-for-speakers.html`에서 첫 번째 공지 카드/게시물로 보인다.
- 새 open call 상세 페이지가 실제 이미지와 연결된다.
- 기존 open call을 종료할지 확인한 뒤, 종료 대상만 archive로 정리했다.
- archive로 옮긴 공지가 있다면 완료형 상태로 보인다.
- archive 결과물 링크를 추가할 수 있는 구조가 유지된다.
- 로컬 참조 오류가 없다.
