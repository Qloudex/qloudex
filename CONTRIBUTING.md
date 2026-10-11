# Contributing to Qloudex

Thanks for your interest. Qloudex is early-stage, so small, focused contributions are very welcome.

## Ways to help

- Report bugs or unclear documentation
- Suggest features or new troubleshooting scenarios
- Improve docs and examples
- Fix issues labeled `good first issue`

## Reporting an issue

1. Search existing issues first.
2. Open a new issue with: what you expected, what happened, steps to reproduce, and your environment (OS, versions, cluster type if relevant).
3. Remove secrets, tokens and private hostnames from logs before pasting.

## Submitting a pull request

1. Fork the repository and create a branch: `git checkout -b fix/short-description`
2. Make your change. Keep it focused on one thing.
3. Test it locally and update docs if behavior changes.
4. Commit with a clear message, for example `fix: handle empty pod logs`.
5. Open a pull request describing what changed and why. Link the related issue.

## Code style

- Python: follow PEP 8; format with `black`; add type hints where practical
- Go: run `gofmt` and `go vet`
- Shell: use `shellcheck`
- Infrastructure code: format with `terraform fmt` and keep manifests valid YAML
- Write clear names and short comments for non-obvious logic

## Security

Do not commit credentials. If you find a security problem, contact the maintainers privately instead of opening a public issue.

## Conduct

Be respectful and constructive. Assume good intent and keep feedback about the work.
