# 낚시의 기술 — Interactive Poster (B)

웹캠으로 손끝만 추적해, 손짓에 따라 물고기 떼가 흩어지고 다시 글자로 모이는 B판형 인터랙티브 포스터.

https://eecchaann.github.io/waysofhooking/

- 렌더링: WebGL2 인스턴싱(물고기 1만 2천 마리를 한 번에), 미지원 시 2D 자동 전환 (강제: ?2d)
- 구형 맥: 자동 저사양 모드, 손 추적 GPU/CPU 자동 전환 (강제: 주소 뒤 ?cpu, ?low)
- 손끝 추적: MediaPipe Hands (엄지·검지·중지·약지·새끼 끝) — 각 지점이 마우스 커서처럼 작동
- 소리: 손짓이 빠를수록 보글보글 물방울 소리가 많아짐 (Web Audio로 실시간 합성)
- F 전체화면 · M 소리 · V 웹캠 표현(끔/손끝만/전신 옅게) · C 카메라 · [ ] 감도 · D 추적 지점 보기 · H 안내 숨기기

## 전시 모드

https://eecchaann.github.io/waysofhooking/show (= #kiosk) — 포스터만 (남는 화면은 검정), 커서 자동 숨김, 화면 꺼짐 방지. 더블클릭으로 전체화면.

맥에서 Chrome 키오스크로 바로 띄우기 (터미널):

    open -na "Google Chrome" --args --kiosk --autoplay-policy=no-user-gesture-required "https://eecchaann.github.io/waysofhooking/#kiosk"

(이 방식으로 열면 클릭 없이 소리가 바로 나옵니다. 일반 창에서는 화면을 한 번 클릭해야 소리가 켜집니다.)

종료: Cmd+Q

전시용 맥에서 시작 안내·명령어 복사 페이지: https://eecchaann.github.io/waysofhooking/start
