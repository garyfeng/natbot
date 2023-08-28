# natbot

Drive a browser with GPT-3

Here's a demo: https://twitter.com/natfriedman/status/1575631194032549888

Lots of ideas for improvement:
- Better prompt
- Prompt chaining
- Make a recorder to collect human feedback and do better few-shot
- Better DOM serialization
- Let the agent use multiple tabs and switch between them

Improvements welcome!

# Installation
Using the GitHub CodeSpace, first launch the codespace. 

1. Edit the `natbot.py` to set `headless=True` (L169)

2. In the terminal, do the following

```sh
# install dependencies
pip install playwright, openai
playwright install
# set up OpenAI
export OPENAI_API_KEY=sk-xxxxxxxx

```
3. Start
```sh
# start the demo. Note Google.com no longer exposes the input field. Use an alternative search engine 
python natbot.py 
```
The default is google.com. You need to switch:

```
g
http://duckduckgo.com
t
3
what is today's date
...
```
