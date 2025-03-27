# TurnLLM-llama.cpp

![UpHub AI Agent Arch](https://github.com/turnllm/turnllm-llama.cpp/blob/master/turnllama/uphub-ai-agent-arch.png?raw=true)

TurnLLM is the **AIer** of the arch! the turnllama is C++ implement of turnllm powered by llama.cpp(backend)!

The term "**turn**" is derived from "**in-turn**" (i.e., reversed). The main AI inference architecture currently utilizes a REST API framework, where the inference program operates as a server endpoint and the API invocation endpoint acts as the client. Access to the inference service requires an API key, which imposes limitations on scalability and availability. The AI inference program essentially functions as a task handler: it pulls tasks, processes them (performs inference), and returns results. This is a classic Producer-Consumer design pattern, effectively decoupling the AI application from the AI inference component. This structure allows for scalable and on-demand task expansion without requiring modifications to the AI application layer. The turnllama.cpp is primarily based on llama.cpp, and turnllm can represent any inference program as long as it can pull tasks, process them, and return results (e.g., in Python).
