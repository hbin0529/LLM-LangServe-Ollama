# LLM-LangServe-Ollama
Ollama+LangServe+LLM

1. Ollama Windows 설치 : https://ollama.com/download

2. HuggingFace-Hub 설치
pip install huggingface-hub

3. GGUF 파일 : https://huggingface.co/heegyu/EEVE-Korean-Instruct-10.8B-v1.0-GGUF 
    - windows 또는 Cli 로 설치
    - Cli 설치 방법: huggingface-cli download heegyu/EEVE-Korean-Instruct-10.8B-v1.0-GGUF ggml-model-Q5_K_M.gguf --local-dir 본인의_컴퓨터_다운로드폴더_경로 --local-dir-use-symlinks False

- Ollama 실행
    ollama create EEVE-Korean-10.8B -f EEVE-Korean-Instruct-10.8B-v1.0-GGUF/Modelfile
- Ollama 모델 목록
    ollama list
Ollama 모델 실행
    ollama run EEVE-Korean-10.8B:latest

app 폴더 진입 후 python server.py 실행
