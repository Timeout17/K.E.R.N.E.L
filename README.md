# K.E.R.N.E.L
This is meant to be a personal assistant who helps me with my daily work and my college studies, much like J.A.R.V.I.S. and F.R.I.D.A.Y. are to Tony Stark—only this is a much smaller-scale project; I don’t intend to save the world, but I’d still like to develop and apply basic engineering principles here as well throughout the project. 
I’m a beginner! So if a senior colleague happens to visit this page, please view this project in that light.
Thank you🤗

## Features

Initially, K.E.R.N.E.L will have very basic tasks and tools, such as:
- Checking the weather and news
- Managing my Gmail and calendar
- Searching the internet
These would be part of the MVP; even just this would already be a huge help to me.
Later on, however, I plan to include a testing and coding component—but someone who would create boilerplate code for me rather than finished code.
And much later, it will also gain smart home tools.

## Architecture

I start speaking -> K.E.R.N.E.L picks up on a wake word -> it starts listening to what I’m saying -> it sends this to the orchestrator LLM via a FastAPI backend -> it decides which tool to use -> selects it -> executes it -> sends the results back -> finally, it tells me verbally and either repeats what I said or executes the command.

## Technology Stack

The technology stack is roughly as follows:

### Backend
- FastAPI / Uvicorn / SlowAPI

### AI 
- LangChain/LangGraph
- Ollama - vLLM
- Fine-tuning

### DevOps
- GitHub Actions
- Docker
- Prometheus / Grafana for monitoring