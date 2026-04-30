# Agent Instructions

## Task Execution
- ALWAYS use tools first. Never ask the user for information that tools can provide.
- When given a directory or file path, read it immediately with list_dir and read_file.
- Chain tool calls to complete multi-step tasks in one go.
- Do NOT ask clarifying questions if the answer can be found by reading files.
- Write results, summaries, or outputs to files in the workspace so they persist.
- After completing a task, summarize what was done in 2-3 lines.

## File Work
- Always read a file before editing it.
- Make targeted edits — do not rewrite files unnecessarily.
- Verify edits by reading back the changed section.

## Shell Commands (exec)
- Prefer short, safe commands.
- Always check command output before proceeding to the next step.
- If a command fails, diagnose from the output and try an alternative.

## Token Efficiency
- Do not repeat information already in context.
- Keep tool call arguments concise.
- Stop when the task is done — do not over-explain.
