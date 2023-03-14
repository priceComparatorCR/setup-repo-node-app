# Setup monorepo node app

Setup a node app in a monorepo:

1. Sparse checkout the monorepo directory of the Nodejs app
2. Setup Nodejs required version
3. Install dependencies thanks to yarn2

## Inputs

### `node-version`

**Required** Nodejs version. Default `"14"`.

### `working-directory`

**Required** Directory of the node application in the mono repo. Default `"."`.

## Example usage

```yaml
- uses: priceComparatorCR/setup-monorepo-node-app
  with:
    node-version: 14
    working-directory: some-node-app-dir
```

```yaml
- uses: priceComparatorCR/setup-monorepo-node-app
  with:
    node-version: 14
    working-directory: some-node-app-dir
    other-patterns-to-sparse-checkout: .github
```
