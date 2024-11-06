# Pull Request Guidelines

## Purpose

This document outlines the best practices for creating and reviewing pull requests in Elabs.

## Structure

A well-crafted pull request should contain the following elements:

1. Title
2. Description
3. Screenshots/GIFs
4. Related Issues
5. Checklist
6. Reviewers

## Title

- Be concise but descriptive (50 characters max)
- Follow the format: "[Type] - Brief description"
- Examples:
  - "Fix: Update TypeScript version"
  - "Feature: Add React component"

## Description

- Provide enough context for reviewers to understand the change
- Explain why the change is necessary
- Describe any edge cases or potential issues
- Include relevant screenshots or GIFs to illustrate the change

## Related Issues

- Link to related GitHub issues (e.g., #123, #456)
- Explain how this PR addresses the linked issues

## Checklist

- [ ] Code follows Airbnb JavaScript Style Guide
- [ ] All new features are covered by unit tests
- [ ] No console.log statements left in production code
- [ ] All dependencies are up-to-date
- [ ] TypeScript errors are resolved
- [ ] Documentation has been updated accordingly

## Reviewers

- Assign relevant team members as reviewers
- Include at least one senior developer for code review

## Additional Guidelines

1. **Code Quality**: Ensure the code adheres to the Airbnb JavaScript Style Guide and TypeScript best practices.

2. **Testing**: Include unit tests for new features and significant changes.

3. **Documentation**: Update documentation if necessary, especially for public APIs.

4. **Performance**: Consider performance implications of large changes.

5. **Security**: Ensure no security vulnerabilities are introduced.

6. **Compatibility**: Verify compatibility with supported browsers and platforms.

7. **CI/CD**: Ensure the PR passes all CI/CD checks before merging.

8. **Code Coverage**: Maintain or increase code coverage percentage.

## Review Process

1. **Initial Review**: Assign reviewers and set review deadline.
2. **Code Review**: Focus on code quality, adherence to style guide, and overall design.
3. **Test Review**: Verify unit tests cover all new functionality.
4. **Documentation Review**: Check if documentation needs updating.
5. **Final Approval**: Merge PR once all checks pass and reviewers approve.

## Closing PRs

- Close related issues when the PR is merged
- Update release notes if applicable

## Valid PR Example 

    ### What does this do?

    * i.e Fixed issue relating to updating rfq

    ### What reviewer should know?
    
    * i.e reviewer should run build or migrations

    ### Test on
    * On staging



## Contributing

By submitting a pull request, you agree to abide by these guidelines. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.