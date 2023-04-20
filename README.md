# [llama.cpp](https://github.com/ggerganov/llama.cpp)

## Build:
```shell
git clone https://github.com/star-bits/llama.cpp
cd llama.cpp
make
```

## Models:
```shell
ls ./models
alpaca-7b-ggml-q4_0-lora-merged			gpt4all-unfiltered-7b-ggml-q4_0-lora-merged
ggml-vocab.bin					llama-7b-ggml-q4_0
gpt4all-7b-ggml-q4_0-lora-merged		vicuna-7b-ggml-4bit
```
- `./models/alpaca-7b-ggml-q4_0-lora-merged/ggml-model-q4_0.bin`
- `./models/gpt4all-7b-ggml-q4_0-lora-merged/ggml-model-q4_0.bin`
- `./models/gpt4all-unfiltered-7b-ggml-q4_0-lora-merged/ggml-model-q4_0.bin`
- `./models/llama-7b-ggml-q4_0/ggml-model-q4_0.bin`
- `./models/vicuna-7b-ggml-4bit/ggml-vicuna-7b-4bit.bin`

## Help:
```shell
./main -h
```

## System prompt:
`./prompts/context-setting.txt`
```
A conversation with an AI that provides helpful and accurate answers.

User: Hi!
AI: Hello! What can I help you with?
User: Tell me about alpacas.
AI: Alpacas are South American camelids raised for soft, warm fleece. They're social, gentle, and popular as pets. 
User:
```

## [pyllamacpp](https://github.com/nomic-ai/pyllamacpp)
`./pyllamacpp.ipynb`

## Run:
```shell
./main -m ./models/gpt4all-7b-ggml-q4_0-lora-merged/ggml-model-q4_0.bin -n 256 --repeat_penalty 1.0 --color -i -r "User:" -f prompts/context-setting.txt
```
