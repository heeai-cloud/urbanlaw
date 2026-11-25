# UrbanLaw for Claude

희림 사내 건축법규·도시계획 검토 도구 UrbanLaw(urbanlaw.heeai.cloud)를 Claude에서 쓰는 플러그인입니다. 주소로 용도지역·지구단위계획 같은 토지 정보를 보고, 법령 조문을 찾고, UrbanLaw 법규 검토를 대화에서 돌립니다.

로그인은 heeai.cloud 희림 아이디로 합니다. 희림 아이디가 없으면 쓸 수 없습니다.

## Claude 앱(채팅·Cowork)

1. 왼쪽 메뉴의 플러그인(Plugins)에서 «추가 → 마켓플레이스 추가»(Add marketplace)를 누릅니다.
2. 저장소 칸에 `heeai-cloud/urbanlaw`를 넣고 «동기화»(Sync)를 누릅니다.
3. 목록에 나온 urbanlaw를 추가하면 플러그인 화면이 열립니다. «연결»을 누르고 이어지는 창에서 «계속», «추가»를 차례로 누른 다음 희림 아이디로 로그인합니다.

Claude를 회사 조직 계정으로 쓰면 조직 관리자가 커넥터 주소 `https://urbanlaw.heeai.cloud/mcp`를 먼저 넣어 두어야 «연결»이 눌립니다.

## Claude Code

```
claude plugin install urbanlaw --marketplace heeai-cloud/urbanlaw
```

설치한 다음 `/mcp`에서 urbanlaw를 골라 로그인합니다.

## 쓰는 법

- `/urbanlaw 강남구 역삼동 737 업무시설 신축 법규 검토` (Cowork는 `/urbanlaw:urbanlaw`, 채팅에서는 그냥 말해도 됩니다)
- 땅 정보는 UrbanLaw Step 1 화면의 내용을 모두 받습니다. 고시는 지구단위계획·특별계획구역·가로구역·정비사업마다 최신 고시 한 건만 가져와 이 땅이 나오는 부분을 함께 넘깁니다. 원문(PDF·HWP·결정도)은 Claude가 필요할 때 직접 읽습니다. 이전 고시는 따로 물을 때만 엽니다.
- 토지 정보와 법령 찾기는 몇 초 안에 끝납니다. 별표처럼 긴 표는 전문을 끝까지 읽습니다. 법규 검토는 보통 5~10분 걸리고 끝나면 UrbanLaw «내 보고서»에 저장됩니다.
- UrbanLaw 결과는 실무 검토용 참고 자료이며 법률 의견이 아닙니다.
- `/urbanlaw`만 입력하면 첫 화면이 뜹니다. Claude 채팅·Cowork에서는 카드에 주소나 질문을 넣고 단추를 누르면 바로 시작합니다. Claude Code에서는 선택지 메뉴에서 고릅니다.
- 설치 안내: https://urbanlaw.heeai.cloud/claude/ · 사용법(질문 예와 받는 답): https://urbanlaw.heeai.cloud/claude/usage (둘 다 희림 아이디로 로그인해서 엽니다)

## 주고받는 곳

urbanlaw.heeai.cloud 한 곳입니다. 검토 질문과 결과는 희림 사내 서버에 저장되고 Claude 대화 내용은 받지 않습니다.

© HeeAI. All rights reserved.
