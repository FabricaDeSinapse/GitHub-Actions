name: Hello GitHub Actions

on:
    push:
        branches: ["*"]

jobs:
    build:
        runs-on: ubuntu-latest
        steps:
            - uses: actions/checkout@v2
            - uses: actions/setup-node@v1
              with:
                  node-version: 16
            - run: npm ci
            - run: npm run test
            - run: npm run build
            - run: npm run deploy
