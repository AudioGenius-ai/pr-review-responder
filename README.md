# pr-review-responder
A local task that runs whenever a comment is added on GitHub and passes it to Codex.

## Plan
1. Initialize the project with pnpm and the Vite Node/TypeScript template.
2. Add dependencies for scheduling (`node-cron`) and Docker communication (`dockerode`).
3. Implement a CLI entry point in `src/cli.ts` that schedules periodic checks for new comments.
4. Forward each comment to a running Codex container.
5. Use Vite to build the TypeScript sources to a runnable Node bundle.
6. Provide npm scripts for building and starting the CLI.
