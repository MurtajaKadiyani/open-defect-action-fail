# Github Defect(Issue) Action

This action opens a new github Defect(Issue).

## Inputs

### `token`

**Required** Github Token.

### `title`

**Required** Issue title.

### `body`

Issue body.

### `assignees`

Issue assignees. Passed as a formatted multi-line string using the | character.

## Outputs

### `issue`

The issue object as a json string.

## Example usage

```yaml
uses: MurtajaKadiyani/open-defect-action-fail@v1
with:
  token: ${{ secrets.GITHUB_TOKEN }}
  title: Some Issue Title
  body: Some Issue Body
  assignees: |
    MurtajaKadiyani
