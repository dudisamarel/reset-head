# Reset Head
Resetting hard branch to certain HEAD

# Workflow Permissions
Before you start you need to grant GITHUB_TOKEN write permission:
1. navigate to the main page of the repository.
2. Under your repository name, click **Settings**.
3. In the left sidebar, click **Actions**, then click **General**.
4. In Workflow permissions section check **Read and write permissions** and click **Save**.

[Workflow Permissions](https://raw.githubusercontent.com/dudisamarel/reset-head/blob/master/assets/workflow-permissions.png)

# Usage
```
- uses: dudisamarel/reset-head@v1.0.0-beta
  with:
    branch-name: develop
    github-secret: ${{ secrets.GITHUB_TOKEN }}
```
