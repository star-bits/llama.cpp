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
alpaca-7b-ggml-q4_0-lora-merged		llama-7b-ggml-q4_0
ggml-vocab.bin				vicuna-13b
gpt4all-7b-ggml-q4_0-lora-merged	vicuna-7b
```
- `./models/alpaca-7b-ggml-q4_0-lora-merged/ggml-model-q4_0.bin`
- `./models/gpt4all-7b-ggml-q4_0-lora-merged/ggml-model-q4_0.bin`
- `./models/llama-7b-ggml-q4_0/ggml-model-q4_0.bin`
- [<code>./models/vicuna-7b/ggml-vic7b-q4_0.bin</code>](https://huggingface.co/eachadea/ggml-vicuna-7b-1.1)
- [<code>./models/vicuna-13b/ggml-vic13b-q4_0.bin</code>](https://huggingface.co/eachadea/ggml-vicuna-13b-1.1)

## Help:
```shell
./main -h
```

## System prompt:
`./prompts/context-setting.txt`
```
A conversation with an AI that provides helpful, polite, and concise answers.

User: Hey, you there?
AI: At your service, sir.
User:
```

## [pyllamacpp](https://github.com/nomic-ai/pyllamacpp)
`./pyllamacpp.ipynb`

## Run:
```shell
./main -m ./models/vicuna-13b/ggml-vic13b-q4_0.bin -n -1 --repeat_penalty 1.0 --color -i -f prompts/context-setting.txt -r "User:"
```
