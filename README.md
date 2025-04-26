# Dan's Workflow

Since many people have asked about the system prompts and custom modes I use, I've compiled them here.

## System Prompts

I have replaced the default system prompts of the `Code` mode with one I made based on the Cursor AI IDE system prompt.

This prompt is reduced in length, some of the rules of the default prompt are removed, some were moved to the tool description when that ruled applid to the tool.

There are a couple of missing tools as well, the MCP instructions and MCP resource tools were removed since I don't user them at all.
I haven't tested the new `insert_content` and `search_and_replace` tools, so they are not included in the prompt yet.

## Custom Modes

### Researcher (dev-research)

This mode is designed to be used with the [Perplexity MCP Server](https://github.com/daniel-lxs/mcp-perplexity).

The purpose of the mode is to provide accurate, relevant, and current information and also verify and cross-reference the information provided by the Perplexity since the information given by it can be incorrect (The LLMs sometimes hallucinate information or the lack of it).

### Chat (chat-mode)

This mode is used to plan, debug, and analyze code.

This mode is designed to be very chatty and will repeatedly ask questions about what you want to do unless you specifically ask it to create a new `Code` task or perform another action.

This mode cannot create or edit files at all.
