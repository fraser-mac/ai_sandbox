# AI Sandbox

This is a general purpose area for AI experimentation with AI tools.

23/12/2025

The notebooks folder currently contains three notebooks that were generated from exampless in Andrew Ng's 10/12/2025 Batch newsletter - "Claude Opus 4.5 Saves Tokens, White House Boosts AI-Powered Science, Amazon Exposes Nova 2 Pro Checkpoints, Small Models Solve Hard Puzzles"

We use his *aisuite* package to perform LLM calls to create apps using prompting.  The original notebook code expected the user to provide LLM API key in the .env file, but due to the way we access AWSBedrock, there was a bit of re-work (hacked iwth Gemini Pro) to get this working for my needs.  This also then necessitated changes to the way that output from the MCP server was dealt with, in terms of raw vs JSON wrapped text.

Finally, there were issues in getting the MCP filesytem tool to work, so for speed, we reverted to just using os for file output.

However, in all three notebook cases I was able to get an app working relatively quickly, with the R-Type game being very quick, and I just implemented some improvements thorugh simple updates to the prompt
