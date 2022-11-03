# Update Submodule Action

This action creates a pull request in a parent repository to update one of its submodules.

## Inputs

### `github-token`

**Required** Personal access token (PAT) used to access the project board.

### `submodule-path`

**Required** The path to the submodule inside the parent repository.

### `parent-repository`

**Required** The name of the parent repository, e.g., `my-org/my-repo`.

### `parent-branch`

**Required** The base branch of the parent repository.

## Example usage

```yaml
uses: vtisweden/action-update-submodule@main
with:
  github-token: ${{ secrets.TOKEN }}
  submodule-path: path/to/submodule
  parent-repository: my-org/my-repo
  parent-branch: main
```
