# Contributing to Qloudex

Thanks for helping improve Qloudex. This repository is the project hub for
shared documentation, the organization roadmap, and the project directory. It
does not contain the application code for KubePilot, SystemMonitoring, Codewise
CLI, or GO-CI-CD.

## Choose the right repository

| Change | Repository |
| --- | --- |
| Studio overview, project directory, roadmap, or shared documentation | [Qloudex/qloudex](https://github.com/Qloudex/qloudex) |
| KubePilot behavior or documentation | [Qloudex/kubepilot](https://github.com/Qloudex/kubepilot) |
| SystemMonitoring behavior or documentation | [Qloudex/SystemMonitoring](https://github.com/Qloudex/SystemMonitoring) |
| Codewise CLI behavior or documentation | [Qloudex/Codewise-CLI](https://github.com/Qloudex/Codewise-CLI) |
| GO-CI-CD application or pipeline documentation | [Qloudex/GO-CI-CD](https://github.com/Qloudex/GO-CI-CD) |
| Organization profile | [Qloudex/.github](https://github.com/Qloudex/.github) |
| Website | [Qloudex/qloudex.github.io](https://github.com/Qloudex/qloudex.github.io) |

Check the target repository's README and contribution guidance before making a
change. Requirements and available checks differ between projects.

## Propose a change

1. Search the target repository's existing issues and pull requests.
2. For a substantial change, open an issue describing the problem and proposed
   scope before implementation.
3. Do not include credentials, access tokens, private hostnames, customer data,
   or other sensitive information.

An existing issue or label is not required unless the target repository
explicitly says otherwise.

## Submit a pull request

1. Fork or clone the correct repository.
2. Create a focused branch from its default branch.
3. Make the smallest change that addresses the documented problem.
4. Run the checks documented by that repository. For documentation-only work,
   review Markdown rendering, links, spelling, and code examples.
5. Open a pull request explaining what changed, why it changed, how it was
   verified, and any remaining limitations.

Do not include unrelated formatting or refactoring in the same pull request.

## Documentation standards

- Describe implemented behavior, not intended behavior.
- Label experimental and planned work clearly.
- Do not invent customers, outcomes, benchmarks, certifications, or production
  claims.
- Use repository-relative links for files in the same repository.
- Preserve historical attribution and existing license terms.
- Remove secrets and identifying infrastructure details from examples and logs.

## Security-sensitive reports

Do not open a public issue containing exploitable details or credentials. Follow
the target repository's `SECURITY.md` when one exists. If it does not provide a
private reporting channel, contact a maintainer to request one before sharing
details.

## Conduct

Be respectful, specific, and constructive. Keep feedback focused on the work.
