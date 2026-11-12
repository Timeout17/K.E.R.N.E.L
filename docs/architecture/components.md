# Components of K.E.R.N.E.L

## Wakeword Monitoring
- It must be able to listen for a specific sound or word and start recording my voice

## Audio Recording
- This must be automatic: when it hears the wakeword, it must immediately start listening for about 5 seconds, and if no command is spoken, it stops recording
- As soon as a command is spoken, it records it and sends it via a FastAPI backend to the component capable of processing the audio

## FastAPI
- We need this because I’d like it to eventually appear on smartwatches and phones as well, and for them to share a common backend.
- I’d also like to build a rate limit into it here, as this will help prevent too many tasks from being executed within a short period of time.

## Llama Orchestrator
- It will receive the message (currently without validation, but Llama Guard will be added later), and this LLM will interpret it and call the appropriate tools.


## Tools
- WeatherTool -> Its main task is to retrieve the current weather.
- NewsTool -> Its task is to return the latest news.
- SearchTool -> It can go online and search for something for me.
- GmailTool -> It can read my Gmail messages and write emails on my behalf.
- CalendarTool -> It can tell me my calendar schedule and make entries in it.

## Voice-based responses
