# 원문과 검토 기록

작성일: 2026-09-11

## 사용자가 제공한 기준

아래 프롬프트는 사용자가 대화에 직접 제공했다. 사용자는 Anthropic에서 제공했다고 설명했으나 공식 출처까지 확인하지는 않았다.
```text
Avoid mannered prose.

Do not replace clear, literal statements with decorative metaphors,
clever phrasing, or unnecessary flourishes.

Prefer direct, precise language.
If a literal phrase expresses the meaning accurately, use it.

Do not write to display style.
Write to make the idea easier to understand.

Before finalizing, check:

- Is this metaphor necessary?
- Is this phrase clearer than the literal version?
- Does it introduce unintended connotations?
- Can the sentence be stated more directly?
```

지정 파일은 `/Users/lavickim/_Dev/doctorpost-ecosystem/doctorpost/app/2026-09-09-anthropic-avoid-mannered-prose-prompt.md`이다. 해당 경로는 확인 당시 존재하지 않았다. `lavicbiz/doctorpost-ecosystem/doctorpost/app`과 관련 저장소에서도 같은 이름이나 원문을 찾지 못해 대화의 원문을 사용했다. 누락 문서를 찾았거나 원본을 수정했다고 주장하지 않는다.

사용자는 ‘대화할 때는 자연스러운데 구현을 요청하면 문장이 어색해진다’는 관찰도 반영하도록 요청했다. 독자의 질문에 직접 답한 초안을 쓰고 필요한 배경과 적절한 말투를 적용하도록 구성했다. 이는 작성 방식에 관한 실무적 판단이며 모델 내부 원인을 검증한 결과는 아니다.

## im-not-ai 검토

공개 저장소: [epoko77-ai/im-not-ai](https://github.com/epoko77-ai/im-not-ai)

검토 시점 main 커밋: `9747f036cdc28a1a8aea4dc71fef1f7846eb96f7`

- [Codex SKILL.md](https://github.com/epoko77-ai/im-not-ai/blob/9747f036cdc28a1a8aea4dc71fef1f7846eb96f7/codex/skills/humanize-korean/SKILL.md)
- [한국어 quick-rules.md](https://github.com/epoko77-ai/im-not-ai/blob/9747f036cdc28a1a8aea4dc71fef1f7846eb96f7/skills/humanize-korean/references/quick-rules.md)
- [MIT License](https://github.com/epoko77-ai/im-not-ai/blob/9747f036cdc28a1a8aea4dc71fef1f7846eb96f7/LICENSE)

기존 `~/.codex/skills/humanize-korean`은 `/Users/lavickim/_Dev/im-not-ai/codex/skills/humanize-korean`을 가리키는 링크로 이미 설치돼 있었다. 로컬 커밋은 `85c2044aaab3383e07cd16a3be3f50044a6231b7`이었다. 기존 설치를 덮어쓰지 않고 별도 스킬을 만들었다.

반영한 기준은 사실·직함·수치와 주장 강도를 보존하는 것, 번역투와 명사 나열을 문맥에 맞게 다듬는 것, 원래 말투와 자연스러운 문장을 살리는 것이다. 최신 규칙도 대명사와 접속사를 문맥에 따라 보존하도록 다루며 이를 단어 금지 목록으로 옮기지 않았다.

수정 비율 제한, 강제 롤백, 등급 산정, 문장 길이 배합, 파일 출력과 요약 블록 강제, 다른 모델로 전환하는 절차는 가져오지 않았다. AI 탐지 지표를 글의 품질이나 인간 작성 여부의 증명으로 쓰지 않는다. 규칙과 예시는 사용자 목적에 맞게 새로 작성했으며 참고 프로젝트의 라이선스 고지는 [upstream-license.txt](upstream-license.txt)에 보존한다.

## 기존 copywriting과의 역할

검토한 설치 파일: `/Users/lavickim/.agents/skills/copywriting/SKILL.md`

판매 페이지 구성과 행동 유도를 위한 스킬이다. 명확성과 정직성을 강조하는 부분은 유용하지만 수사적 질문·비유·재치를 권하고 영어 중심 예시를 사용한다. 이것만으로 한국어 조사, 어미, 격식, 번역투까지 충분히 다루지는 않는다. 한국어에 쓸 수 없다고 단정하지 않고 페이지 구성에는 보조로 쓰되 문장 표현에는 사용자 기준과 새 한국어 스킬을 적용한다.
