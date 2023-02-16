# Reset Head

Resetting hard branch to certain HEAD

# Before you start

`reset-head` requires a GitHub token with write permission.
You configure this token via the `token` configuration option.

You can use the built-in `GITHUB_TOKEN` secret, however, you have to grant write permission:

1. navigate to the main page of the repository.
2. Under your repository name, click **Settings**.
3. In the left sidebar, click **Actions**, then click **General**.
4. In Workflow permissions section check **Read and write permissions** and click **Save**.

# Usage

```
- uses: dudisamarel/reset-head@v1
  with:
    branch-name: develop
```

# Configuration

| input       | description                                                                                              |
| ----------- | -------------------------------------------------------------------------------------------------------- |
| branch-name | **required**. The name of the branch to reset.                                                           |
| token       | **optional**. A GitHub secret token, the action defaults to using the the built-in `GITHUB_TOKEN` secret |
| head        | **optional**. The commit or tag to reset the branch to. Default `$GITHUB_REF_NAME`                       |
