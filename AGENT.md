# Review before every push

IMPORTANT: Before any `git push` or `gh pr create`, run the pre-push review in `.claude/skills/review-pr-loop/SKILL.md`. In Claude Code, invoke the `review-pr-loop` skill; any other agent reads that file and follows it. This applies every time: when asked to "push" or "open a PR", and for commits going to an existing PR branch.

The review reports blockers only, has subagents fix them, and reviews again. Then it decides where the change goes: a clean change that meets its low-risk rules goes straight to `main`, and everything else opens a PR. Skip the review only when the user explicitly says to skip it for that push.
