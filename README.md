# 사진 공유 앱 프로토타입

휴대폰에서 앱처럼 조작할 수 있는 HTML 워킹 프로토타입이에요. 앱은 `phou/index.html`, 받는 사람용 웹은 `web/index.html` 에 들어 있어요.

## 바로 열기 (GitHub Pages, 어디서나 열림)

- 첫 화면: https://smpkjh3-d4ng.github.io/2216556-smvd202602/
- 앱: https://smpkjh3-d4ng.github.io/2216556-smvd202602/phou/
- 초대 링크 웹: https://smpkjh3-d4ng.github.io/2216556-smvd202602/web/

## 휴대폰에서 열기 (로컬 서버)

Mac에서 서버를 켜요 (macOS 기본 Ruby 사용).

```bash
ruby -run -e httpd phou -b 0.0.0.0 -p 8123
```

휴대폰을 같은 Wi-Fi에 연결하고 `http://<Mac의 IP>:8123` 으로 들어가요. Mac의 IP는 `ipconfig getifaddr en0` 으로 확인할 수 있어요.
Safari/Chrome의 공유 → **홈 화면에 추가** 로 열면 주소창 없이 전체 화면으로 떠요.

## 프로토타입 조작

- 상태 전환 패널(로딩·비어 있음·오류 등): 휴대폰에서 **두 손가락으로 탭**, 또는 주소 끝에 `?dev`
- 컴퓨터 브라우저에서는 원래의 폰 프레임 + 상태 전환 바로 보여요
