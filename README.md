## POC - Chatbot Copilot Tool

### What is this?

This is a proof of concept GPTScript chatbot tool that can be used to help make LLMs behave more like traditional chatbots.

Features:

- Ask for multiple inputs from the user one at a time instead of all at once.
- Confirms the users responses before moving on to the next part of the flow.
- Looks for a tool called `out_of_bounds` to respond to things you don't want the chatbot to respond to.

## Example

```gptscript
chat: true
context: github.com/cloudnautique/chatbot-copilot/context.txt
tools: github.com/cloudnautique/chatbot-copilot

You are a helpful assistant that needs to ask if the user wants to sign up for a newsletter.

If they do, ask for their first name and email address.

If they don't, say goodbye.
```
