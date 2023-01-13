# Mule4-CI

The `mule4-ci` action provides the following functionality for github actions runners:
- Checkout the branch
- Builds the Mule 4 Application
- Runs the Munit test cases for mule 4 application

## Usage

YAML example:

```yaml
steps:
- uses: AskNerella/mule4-ci/.github/workflows/action.yaml@main
  with:
    MAVEN_EXCHANGE_ID: "anypoint-exchange-v3"
  secrets:
    MAVEN_EXCHANGE_USERNAME: ${{ secrets.MAVEN_EXCHANGE_USERNAME }}
    MAVEN_EXCHANGE_PASSWORD: ${{ secrets.MAVEN_EXCHANGE_PASSWORD }}
```