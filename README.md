# UrbanLaw for Claude

희림 사내 건축법규·도시계획 검토 도구 UrbanLaw(urbanlaw.heeai.cloud)를 Claude에서 쓰는 플러그인입니다. 주소로 용도지역·지구단위계획 같은 토지 정보를 보고, 법령 조문을 찾고, UrbanLaw 법규 검토를 대화에서 돌립니다.

로그인은 heeai.cloud 희림 아이디로 합니다. 희림 아이디가 없으면 쓸 수 없습니다.

## Claude 앱(채팅·Cowork)

1. 사용자 지정 → 플러그인(Customize → Plugins)에서 «추가 → 마켓플레이스 추가»(Add marketplace)를 누릅니다.
2. 저장소 칸에 `heeai-cloud/urbanlaw`를 넣습니다.
3. 목록에 나온 urbanlaw를 추가한 다음 커넥터(Connectors) 탭에서 «연결»을 누르고 희림 아이디로 로그인합니다.

Claude를 회사 조직 계정으로 쓰면 조직 관리자가 커넥터 주소 `https://urbanlaw.heeai.cloud/mcp`를 먼저 넣어 두어야 «연결»이 눌립니다.

## Claude Code

```
claude plugin install urbanlaw --marketplace heeai-cloud/urbanlaw
```

설치한 다음 `/mcp`에서 urbanlaw를 골라 로그인합니다.

## 쓰는 법

- `/urbanlaw 강남구 역삼동 737 업무시설 신축 법규 검토` (Cowork는 `/urbanlaw:urbanlaw`, 채팅에서는 그냥 말해도 됩니다)
- 토지 정보와 법령 찾기는 몇 초 안에 끝납니다. 법규 검토는 보통 5~10분 걸리고 끝나면 UrbanLaw «내 보고서»에 저장됩니다.
- UrbanLaw 결과는 실무 검토용 참고 자료이며 법률 의견이 아닙니다.
- 자세한 안내: https://urbanlaw.heeai.cloud/claude/ (희림 아이디로 로그인해서 엽니다)

## 주고받는 곳

urbanlaw.heeai.cloud 한 곳입니다. 검토 질문과 결과는 희림 사내 서버에 저장되고 Claude 대화 내용은 받지 않습니다.

© HeeAI. All rights reserved.
