# Unity MCP

Is a free [Unity package that adds Unity specific skills to an AI](https://github.com/IvanMurzak/Unity-MCP). 35 minute [demo of usage](https://youtu.be/dACQfUE_aZY).

## Install

- ClaudeCode is installed on windows by typing [winget install Anthropic.ClaudeCode](https://github.com/anthropics/claude-code#get-started) into a terminal. (poor) video [demonstrationg ClaudeCode install](https://www.youtube.com/watch?v=Z38iu02JFT8).

## Setup

ClaudeCode can be setup to use [free LLMs](https://www.google.com/search?q=can+i+use+claude+code+for+free) with either:

1. using google gemini  https://prince-arora-aws.medium.com/how-i-set-up-claude-code-for-free-no-subscription-no-credit-card-and-what-i-learned-along-the-2cba880682a2  unlimited but more [setup](https://aistudio.google.com/).
2. using openrouter.ai's openrouter/free    Limited to 50 requests/day.
    1. https://www.youtube.com/watch?v=GRUjApPqCoE - 9 min
        1. [video](https://youtu.be/GRUjApPqCoE?si=F903WEEQrPGKituR&t=206) Create API key is requested as soon as you [create an account](https://openrouter.ai).
        2. [video](https://youtu.be/GRUjApPqCoE?si=IA2E4R3L9wfrWMdR&t=262) settings.json didn't work. Instead search for and then click "[Project Settings File](https://openrouter.ai/docs/cookbook/coding-agents/claude-code-integration#step-2-connect-claude-to-openrouter)" to modify the file at `C:\Users\<username>\.claude\settings.json`. be sure to include `"ANTHROPIC_MODEL": "openrouter/free"`.
        3. type `cmd` in the address bar of windows explorer when its at the root of the project to be modified.
        4. type `claude` in the cmd prompt. Should not have to login at all.
        5. you can now request edits to the project folder. [monitor usage](https://openrouter.ai/activity) for the 50 requests/day limit.
    2. https://www.youtube.com/watch?v=BxD6_ig_T08 - 14 min [openrouter doc](https://openrouter.ai/docs/guides/coding-agents/claude-code-integration)
