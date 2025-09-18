# model_note
大模型部署的笔记
1、大模型部署：
- 1-3个中文语言主力大模型，建议deepseek-v3.1-671B-A37B、GLM-4.5-335B-A32B或GLM-4.5-106B-A12B、Qwen3-235B-A22B-Thinking-2507或Qwen3-Next-80B-A3B，使用Ktransformers部署，显存载入最大激活专家+2左右即可，上下文拉到最大，要用就用最好的，可以参考排行榜；特殊用途的长上下文大模型Llama 4 Scout (17Bx16E) 10M、Qwen2.5-14B或GLM-4-9B-Chat-1M 1M
- 1个多模态大模型：MiniCPM-V-4_5-8.7B或Qwen2.5-Omni-7B统一多模态
- 至少1个 嵌入式模型：Qwen3-Embedding-8B
2、至少2个智能体平台：建议AIFlow类的Dify2.0、RagFlow，或Agent平台类的开源Coze、京东的JoyAgent、超级麦吉开源的Magic

MOE大模型务必使用KT或Chitu部署，其余大模型可以考虑使用llama.cpp或ollama等可自行调度资源的框架
