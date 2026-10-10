# interactor-multiplayer-fabric-llm

An Elixir NIF that loads a GGUF language model and runs chat completion in process, streamed or whole.

## What it is for

Zone servers and bots get inference without a separate HTTP sidecar. The API mirrors the engine module's model, context and chat classes. The native side builds a vendored inference runtime fork that adds quantized KV-cache types, and it picks its GPU backend at compile time.

## Build and run

```sh
git submodule update --init --recursive
mix deps.get
mix compile
```

## Licence

MIT. See [LICENSE](LICENSE).
