# CLAUDE.md - AI Assistant Guidelines

This file provides context and guidelines for AI assistants (like Claude) working with this repository.

## Project Overview

**Repository:** my-repo
**Type:** Template/Demo Repository
**Status:** Early development stage
**Primary Language:** None (documentation only at present)

This is a minimal repository that can serve as a foundation for future development. Currently contains only basic documentation files.

## Repository Structure

```
my-repo/
├── .git/                 # Git configuration and history
├── CLAUDE.md            # This file - AI assistant guidelines
└── README.md            # Project description
```

## Development Guidelines

### Git Workflow

**Branch Naming Convention:**
- Feature branches: `claude/{feature-description}-{identifier}`
- Main branch: `main`

**Commit Practices:**
- Use clear, imperative mood commit messages (e.g., "Add feature", "Fix bug")
- All commits are signed using SSH keys
- Keep commits focused and atomic

**Push Commands:**
```bash
git push -u origin <branch-name>
```

### Code Style & Conventions

When this repository grows to include code, follow these general principles:

1. **Consistency:** Match the existing code style in any file you modify
2. **Simplicity:** Prefer simple, readable solutions over clever ones
3. **Documentation:** Document public APIs and complex logic
4. **Testing:** Include tests for new functionality when a test framework is set up

## For AI Assistants

### Before Making Changes

1. **Read before modifying:** Always read files before editing them
2. **Understand context:** Review related files and understand the broader picture
3. **Check for existing patterns:** Look for established conventions in the codebase

### When Writing Code

1. **Keep changes minimal:** Only change what's necessary for the task
2. **Avoid over-engineering:** Don't add features or abstractions that weren't requested
3. **Security awareness:** Be cautious about command injection, XSS, SQL injection, and other vulnerabilities
4. **No placeholder values:** Never use placeholder or hardcoded secrets

### When Committing

1. **Stage specific files:** Prefer `git add <file>` over `git add -A`
2. **Write descriptive messages:** Explain what changed and why
3. **Verify before pushing:** Review changes with `git status` and `git diff`

### File Operations

- Prefer editing existing files over creating new ones
- Use appropriate tools for file operations (not bash commands like cat/sed)
- Never create unnecessary documentation files unless explicitly requested

## Configuration

### Git Configuration

The repository is configured with:
- SSH commit signing enabled
- Local proxy for git operations
- Author: Claude (noreply@anthropic.com)

### Environment

- **Working Directory:** /home/user/my-repo
- **Platform:** Linux

## Common Tasks

### Adding New Features

1. Create a feature branch from main
2. Make focused, incremental changes
3. Test changes locally if applicable
4. Commit with clear messages
5. Push and create a pull request

### Fixing Issues

1. Reproduce the issue if possible
2. Identify the root cause
3. Implement the minimal fix
4. Verify the fix resolves the issue
5. Commit and push

## Future Development Notes

As this repository grows, consider adding:
- [ ] Package configuration (package.json, requirements.txt, etc.)
- [ ] Build scripts and automation
- [ ] Testing framework
- [ ] CI/CD pipeline (.github/workflows)
- [ ] Contributing guidelines (CONTRIBUTING.md)
- [ ] License file

---

*Last updated: 2026-01-30*
