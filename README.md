# Langgraph_SideKick

The Sidekick is a personal co-worker you can give a task and a definition of success, and it will work away using a real browser, a filesystem, web search and more, until it has met your criteria or needs to ask you something.

The Sidekick is a "create_agent" worker wrapped in a homemade evaluator loop.

The worker is a single create_agent. The loop runs around it that checks
the worker's answer against the user's success criteria, and either accepts it, sends it
back for another attempt, or returns to the user with a question. Middleware gives the
worker a plan it shares with the UI, guardrails for PII and runaway costs, and a pause
for human approval before sensitive actions

