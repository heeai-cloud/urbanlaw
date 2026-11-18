# UrbanLaw for ChatGPT & Claude

Claude 채팅·Cowork·Claude Code에서 희림 사내 UrbanLaw로 토지 정보를 보고 건축법규·도시계획 조문을 찾고 UrbanLaw 법규 검토를 돌립니다.

- 명령: `/urbanlaw 강남구 역삼동 737 업무시설 신축 법규 검토` (Claude Code는 `/urbanlaw`, Cowork는 `/urbanlaw:urbanlaw`, 채팅에서는 그냥 말해도 됩니다)
- 설치(Claude Code): `claude plugin install urbanlaw --marketplace heeai-cloud/urbanlaw` · Claude 앱은 «마켓플레이스 추가»에 `heeai-cloud/urbanlaw`
- 연결: 커넥터 주소는 `https://urbanlaw.heeai.cloud/mcp`입니다. 연결할 때 heeai.cloud 로그인 화면이 뜹니다(희림 아이디, 사내 도구 대문과 같은 아이디).
- 할 수 있는 것: 토지 정보(용도지역·지구단위계획·토지이용규제·건축물대장 — UrbanLaw Step 1 화면 전부), 고시 문서 읽기(지구단위계획·특별계획구역·가로구역·정비사업 고시 PDF·HWP와 결정도), 법령 찾기(조문 원문과 국가법령정보센터 링크, 긴 별표는 전문까지), 법규 검토(보통 5~10분, 끝나면 UrbanLaw «내 보고서»에 저장), 법령 개정 이력
- 주고받는 곳: urbanlaw.heeai.cloud 한 곳입니다. 검토 질문과 결과는 희림 사내 서버에 저장됩니다.
- UrbanLaw 결과는 실무 검토용 참고 자료이며 법률 의견이 아닙니다.
- `/urbanlaw`만 입력하면 첫 화면이 뜹니다. Claude 채팅·Cowork에서는 카드에 주소나 질문을 넣고 단추를 누르면 바로 시작합니다. Claude Code에서는 선택지 메뉴에서 고릅니다.
- 설치 안내: https://urbanlaw.heeai.cloud/claude/ · 사용법(질문 예와 받는 답): https://urbanlaw.heeai.cloud/claude/usage (둘 다 희림 아이디로 로그인해서 엽니다)
- ChatGPT 앱(데스크톱): 설정 → 플러그인 → «추가 → 마켓플레이스 추가»의 «출처»에 `heeai-cloud/urbanlaw`(저장소 이름)을 넣고 설치합니다. 새 대화의 «작업 위치»를 «이 컴퓨터»(로컬에서 작업)로 고르고 `@urbanlaw` 뒤에 부탁할 내용을 적습니다. 일반 채팅이나 «클라우드에서 작업»으로 도는 대화에는 도구가 붙지 않습니다.

© HeeAI. All rights reserved.
