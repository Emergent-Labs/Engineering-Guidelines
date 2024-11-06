# Git Guidelines

## Commit Messages

We follow the Conventional Commits specification for our commit messages. This ensures consistency and makes it easy to generate changelogs automatically.

### Format

<type>[optional scope]: <description>

[optional body]

[optional footer(s)]

### Types

- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `perf`: Performance improvements
- `test`: Adding missing tests or correcting existing tests
- `chore`: Maintenance tasks (like updating dependencies)

### Scope

An optional scope may be added after the type/scope delimiter. This could be used to separate independent directives.

### Body

If the commit requires additional explanation, provide a body.

### Footer

May be used for breaking changes, deprecations, or other special situations.

## Branch Naming Conventions

- Main branches:
  - `main`: Production-ready code
  - `develop`: Development branch

- Feature branches:
  - `feature/<ticket-number>-<short-description>`: e.g., `feature/123-add-user-authentication`

- Hotfix branches:
  - `hotfix/<ticket-number>-<short-description>`: e.g., `hotfix/456-fix-login-bug`

- Release branches:
  - `release/<version>`: e.g., `release/v1.2.3`

## Workflow

1. Create a new branch from `develop` for each feature or hotfix:
```

git checkout develop
git pull origin develop
git checkout -b feature/123-add-user-authentication

```

2. Make commits on this branch, following the Conventional Commits specification.

3. Push changes to remote:
```

git push origin feature/123-add-user-authentication

```

4. Create a Pull Request from the feature/hotfix branch to `develop`.

5. After approval and successful CI tests, merge the PR into `develop`.

6. For hotfixes, create a Pull Request from the hotfix branch to both `main` and `develop`.

## Production and Staging Branches

- Do not push directly to `production` or `staging` branches.
- These branches should only be updated through merges from `develop`.

## Review Process

- All pull requests must be reviewed by at least one senior developer.
- Only senior developers can merge pull requests into production or staging branches.

## Best Practices

1. Keep commits small and focused.
2. Write clear, descriptive commit messages.
3. Use meaningful branch names.
4. Regularly update your local repository with `git fetch` and `git pull`.
5. Always test your changes locally before pushing.
6. Use meaningful commit message subjects and bodies.

## Tools

We use GitHub for our version control system. Familiarize yourself with GitHub's web interface and Git commands.

By following these guidelines, we maintain consistency across our project and make it easier for everyone to contribute and understand the codebase.

This Git guidelines document covers:

1. Commit message format using Conventional Commits specification
2. Branch naming conventions for main, feature, hotfix, and release branches
3. Workflow for creating and merging branches
4. Guidelines for production and staging branches
5. Review process for pull requests
6. Best practices for Git usage
7. Recommended tools (GitHub)
