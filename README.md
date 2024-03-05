# NourybotGPT

Twitch chat bot that interacts with ollama. Work in Progress.

## Requirements:
[Golang](https://go.dev/)

[Ollama.com](https://ollama.com)

## Build and run:
1. Change the example values in the provided `env.example` and rename it to `.env`.
2. Make sure ollama is running on the host and reachable at `localhost:11434` and the model that you specified in the `.env` file is already downloaded and ready to go. (Can be checked with e.g. `ollama run wizard-vicuna-uncensored`)
3. Run:
    - With docker compose (might need sudo infront if you haven't setup rootless):
        - `$ make up`
    - Without docker:
        - `$ make build && make run`
4. Join the Twitch channels you chose and type `()gpt <cool query>` and hopefully get a response.
