# Contributing to DuraGraph

Thank you for your interest in contributing to DuraGraph! This document provides guidelines and information for contributors.

## Getting Started

### Prerequisites

- Git
- Go 1.23+ (for duragraph, duragraph-go)
- Python 3.11+ with uv (for duragraph-python)
- Node.js 20+ with pnpm (for duragraph-docs, duragraph-studio)

### Repository Structure

| Repository | Description | Language |
|------------|-------------|----------|
| [duragraph](https://github.com/Duragraph/duragraph) | Core API server and control plane | Go |
| [duragraph-python](https://github.com/Duragraph/duragraph-python) | Python SDK | Python |
| [duragraph-go](https://github.com/Duragraph/duragraph-go) | Go SDK | Go |
| [duragraph-docs](https://github.com/Duragraph/duragraph-docs) | Documentation site | Astro |
| [duragraph-examples](https://github.com/Duragraph/duragraph-examples) | Example projects | Various |
| [duragraph-studio](https://github.com/Duragraph/duragraph-studio) | Interactive UI | TypeScript |

## How to Contribute

### Reporting Issues

1. Search existing issues to avoid duplicates
2. Use the issue templates when available
3. Provide clear reproduction steps
4. Include relevant environment details

### Submitting Changes

We use a **fork-based workflow**:

1. **Fork** the repository to your GitHub account
2. **Clone** your fork locally
3. **Create a branch** with a descriptive name:
   ```bash
   git checkout -b feat/your-feature-name
   # or
   git checkout -b fix/issue-description
   ```
4. **Make your changes** following our coding standards
5. **Commit** with conventional commit messages:
   ```bash
   git commit -m "feat: add new feature"
   git commit -m "fix: resolve issue with X"
   git commit -m "docs: update README"
   ```
6. **Push** to your fork
7. **Create a Pull Request** against the `main` branch

### Commit Message Format

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>: <description>

[optional body]

[optional footer]
```

Types:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `perf`: Performance improvements
- `test`: Adding or updating tests
- `build`: Build system changes
- `ci`: CI/CD changes
- `chore`: Maintenance tasks

### Pull Request Guidelines

- Keep PRs focused and reasonably sized
- Include tests for new functionality
- Update documentation as needed
- Ensure CI checks pass
- Request review from maintainers
- Respond to feedback constructively

## Development Setup

### duragraph (Go API Server)

```bash
git clone https://github.com/YOUR_USERNAME/duragraph.git
cd duragraph
task up        # Start services with Docker
task dev       # Run in development mode
task test      # Run tests
```

### duragraph-python

```bash
git clone https://github.com/YOUR_USERNAME/duragraph-python.git
cd duragraph-python
uv sync                    # Install dependencies
uv run pytest              # Run tests
uv run ruff check .        # Lint
```

### duragraph-go

```bash
git clone https://github.com/YOUR_USERNAME/duragraph-go.git
cd duragraph-go
go mod download            # Install dependencies
go test ./...              # Run tests
```

### duragraph-docs

```bash
git clone https://github.com/YOUR_USERNAME/duragraph-docs.git
cd duragraph-docs
pnpm install               # Install dependencies
pnpm dev                   # Start dev server
pnpm build                 # Build for production
```

## Code Style

### Go
- Follow [Effective Go](https://go.dev/doc/effective_go)
- Use `go fmt` and `go vet`
- Keep functions focused and testable

### Python
- Follow PEP 8
- Use type hints
- Format with `ruff format`
- Lint with `ruff check`

### TypeScript
- Use TypeScript strict mode
- Format with Prettier
- Follow ESLint rules

## Testing

- Write tests for new functionality
- Maintain or improve code coverage
- Include unit tests and integration tests where appropriate

## Documentation

- Update README files as needed
- Add inline comments for complex logic
- Update API documentation for new endpoints
- Add examples for new features

## Community

- Join discussions in [GitHub Discussions](https://github.com/orgs/Duragraph/discussions)
- Be respectful and follow our [Code of Conduct](CODE_OF_CONDUCT.md)
- Help others in issues and discussions

## License

By contributing, you agree that your contributions will be licensed under the Apache License 2.0.

## Questions?

If you have questions, feel free to:
- Open a [Discussion](https://github.com/orgs/Duragraph/discussions)
- Check existing issues and PRs
- Review the documentation

Thank you for contributing to DuraGraph!
