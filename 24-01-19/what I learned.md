# ManysenseVR 제작

- VR 프로젝트에 연결된 컨텍스트 유형에 관계없이 데이터를 수집할 수 있는 툴인 ManysenseVR 을 제작 완료. (이번에 연구실을 나오게 되었는데, 마지막으로 완결 지은 프로젝트.) 현재 수집/데이터 내보내기 방식이 지원되지 않더라도 확장하기 좋은 구조를 제공. 이와 관련하여 사용법 작성, 마지막 구조 및 일부 기능 리팩토링 등의 과정을 거침.

# OpenAI 기반 APP 및 구조 완성

- OpenAI 의 Assistant 기능을 활용하여 Player 에게 질문할 고민을 생성하는 AI 및, Player 가 해당 고민에 대해 대답하면 이에 대한 반응을 해주는 AI 를 GPT Assistant 기능을 활용하여 제작.

# LLAMA - LLM(+BASICS).

- OpenAI 를 제외한 다른 모델들을 활용하고자 하였음. 이에 따라, 남게되는 모델은 Llama 와 같은 OpenSource Model, 그리고 홈페이지 자체적으로 제공되는 Gemini, HyperClovaX 가 존재하였음.
- Gemini, HyperClovaX와 같은 모델들은 모델을 자체적으로 제공하는 것이 아닌, API 를 통해 여기에 접근할 수 있는 방법을 제공하므로, 이는 각각의 API 에 따라 개발되어야 한다고 파악하였으며, 이에 따라 "모델들"에 대해 보다 쉽게 확장할 수 있는 OpenSourceLLM 들에 대해 조사.

- LLM(+BASICS) : 현재 나는 인공지능 기초 지식 및 LLM(Large Language Models) 사용에 대한 지식 (FineTuning - LoRA, HyperNetworking) 등이 부족하기 때문에, 이러한 주제를 공부할 수 있는 필요 학습 자원과 공부 방법을 탐색하는 데 초점을 맞춤. 인공지능의 기본 원리, 신경망, LLM의 원리 및 사용법에 대한 개념 정리와 함께, GPT, Gemini, Llama, HyperClovaX 등 LLM 모델을 활용한 프로젝트 수행을 위한 실무적 방법을 고민함. Stanford CS231N, 자연어 처리 입문, 및 Andrew Ng의 강의 등을 통한 기초 지식 공부법으로 결론을 내림. 단, 이 강의들의 경우 그 깊이와 양이 많기 때문에, LLM 사용 등을 우선시 하여 진행하되, 토대로서 지속적으로 병행하자 결론 내림.