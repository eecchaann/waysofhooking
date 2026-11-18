# 낚시의 기술 — Interactive Poster (B)

웹캠으로 손을 추적해, 손짓에 따라 물고기 떼가 흩어지고 다시 글자로 모이는 B판형 인터랙티브 포스터.

https://eecchaann.github.io/waysofhooking/

- 손끝 추적: MediaPipe Hands (엄지·검지·중지·약지·새끼 끝) — 각 지점이 마우스 커서처럼 작동
- F 전체화면 · V 웹캠 표현(끔/손끝만/전신 옅게) · C 카메라 · [ ] 감도 · D 추적 지점 보기 · H 안내 숨기기

## 전시 모드

https://eecchaann.github.io/waysofhooking/#kiosk — 여백·안내 문구 없이 포스터만, 커서 자동 숨김, 화면 꺼짐 방지. 더블클릭으로 전체화면.

맥에서 Chrome 키오스크로 바로 띄우기 (터미널):

    open -na "Google Chrome" --args --kiosk "https://eecchaann.github.io/waysofhooking/#kiosk"

종료: Cmd+Q
