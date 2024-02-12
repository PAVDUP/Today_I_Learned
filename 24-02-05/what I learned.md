# LLAMA - vLLM, HuggingFace Space, RunPod Worker.

- vLLM + Runpod Worker

vLLM 공부. Paged attention 등의 특성. Docker 혹은 코드를 통해 Hugging Face의 LLM 을 가져와 어떻게 사용하는지. 
Runpod을 및 runpod 내 Jupiter notebook 기반 vLLM 사용환경 구축. 하지만, vLLM 을 기반으로 local에 구축된 API Server를 ngrok 과 npx 를 이용하여 외부 port 로 forwarding 하고자 하였으나 실패. (Runpod - Container로 구축한 환경에서 연결하는데 실패)

방법을 찾던 중, Runpod Worker 기능을 통한 serverless api endpoint 생성을 확인. 해당 기능 학습 후 vLLM Endpoint 를 생성. 이후 기능 동작을 확인하여 해결하기까지의 과정을 진행..

- HuggingFace Spaces

vLLM 및 TGI 배포시 활용할 수 있는 공간으로서 HuggingFace Spaces 를 탐구함. DockerFile 을 통한 자동 생성이 가능하나, vLLM 혹은 TGI 구축 시 사용되는 DockerFile 을 조정하여 Spaces 를 올리고자 할 때, 변경해야 하는 변경 요소가 너무 많다는 것(1)과, Spaces 이용 비용이, Runpod 의 Worker 혹은 GPU 대여 비용보다 훨씬 비싸다는 점을 감안하여 학습만을 진행.

- Unity Client 내 Runpod 기능 제작

Runpod Worker 기능을 기반으로 제작한 LLM 을 Unity Client 내에서 사용할 수 있는 Endpoint 에 대한 제작을 진행하는 중에 있음.