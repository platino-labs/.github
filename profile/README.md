# Platino Labs

We build small, dependency-light tools, audit them against our own claims, and publish the ones that survive.

## Open source

### 🔐 [hub-chat](https://github.com/platino-labs/hub-chat)

A team chat you run on your own machine or server. Accounts, channels and history in plain Node.js — no framework, no database, no npm dependencies.

Messages are chained so unexpected changes are easier to notice. That chain is not encryption and does not stop edits, so the README says so plainly, together with what the tool does *not* do.

### 🕵️ [secret_hygiene](https://github.com/platino-labs/secret_hygiene)

Finds passwords and API keys left in a project's files or past commits, and gives a team a workflow for rotating them before rotating becomes an incident.

The report hides detected values so nobody repeats a secret into a ticket. A clean scan is not proof that no secret exists, and the tool does not revoke anything on its own — it says that too.

## How we build

- **Minimal by default.** If the standard library does it, we do not add a dependency.
- **Fail closed.** An unknown state stops the run instead of guessing; exit codes are part of the interface.
- **Limits are documented, not omitted.** Every repository states what it does not protect you from.
- **Claims carry a command.** What we publish can be reproduced by anyone who clones the repository.

## The standard behind the code

We do not ask you to trust the tools because we wrote them. We ask you to check them against the rules we apply to our own claims: prediction fixed before the run, an instrument that can be proven to fail, identity anchors, declared edges, and every sentence carrying its artifact.

**[Read the manifesto →](https://github.com/platino-labs/.github/blob/main/profile/MANIFESTO.md)**

## Want an audit?

We look for exposed credentials, unsafe defaults and dependency rot, and report what we found with the command that found it. Open an issue in either repository, or reach out at <https://github.com/platino-labs>.

## License

Everything published here is MIT licensed unless its own `LICENSE` file says otherwise.
