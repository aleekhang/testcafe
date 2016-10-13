# Contributing to TestCafe

Everyone is welcome to contribute to our project and we truly appreciate your help.
TestCafe would not be possible without active support from the community.

These guidelines help you contribute easily and painlessly.

* [Code of Conduct](#code-of-conduct)
* [General Discussion](#general-discussion)
* [Reporting a Problem](#reporting-a-problem)
* [Code Contribution](#code-contribution)

## Code of Conduct

TestCafe has adopted a [Contributor Code of Conduct](CODE_OF_CONDUCT.md).
By participating in the project you agree to abide by its terms.

## General Discussion

If you have a question about TestCafe or want to share your opinion,
welcome to our [discussion board](https://testcafe-discuss.devexpress.com/).

## Reporting a Problem

Something went wrong with TestCafe? File an issue in our [GitHub repository](https://github.com/DevExpress/testcafe/issues).
But first please search through the existing issues to see if the problem has already been reported or addressed.

When you create a new issue, a template text is automatically added to its body. To help us understand your
problem, be sure to fill in all sections in this template.

## Code Contribution

Please follow these steps when submitting your code.

1. Search the [list of issues](https://github.com/DevExpress/testcafe/issues) to see if
  there is an issue for the bug you are going to fix or the feature you are going to implement. If you don't find any, please create one.

2. If you are going to address an existing issue, check the comment thread to make sure that nobody is working on it at the moment.

3. Leave a comment saying that you are willing to fix this issue and if possible provide details on how you are going to do this.

4. Core team members may need to discuss the details of the proposed fix with you. As soon as you get the green light from them,
  leave a comment saying that you are currently working on this issue.

5. Fork TestCafe and create a branch in your fork. Name this branch with an issue number, e.g. `gh852`, `gh853`.
  
    > If you are going to update documentation, do this in a separate branch, e.g. `gh852-docs`.

6. Commit your changes into the branch.

7. Add regression tests to the appropriate sections if you are fixing a bug. You can find these sections by searching for `Regression` in code.

    Add unit and/or functional tests if you are developing new functionality.

8. Fetch upstream changes and rebase your branch onto `master`.

9. Run tests before submitting a pull request to ensure that everything works properly.

    ```sh
    gulp test-server
    gulp test-functional-local
    gulp test-client
    ```

10. Push changes to your fork.

11. Submit a pull request. If you are also updating documentation, submit a separate pull request for these changes.

    The pull request name should describe what has been done and contain
    the [closes](https://github.com/blog/1506-closing-issues-via-pull-requests) directive
    with an appropriate issue number.

    Documentation pull requests should have the `[docs]` prefix in their title.
    This ensures that documentation tests are triggered against these pull requests.