# geekhub-lab.github.io

[![CircleCI](https://circleci.com/gh/geekhub-lab/geekhub-lab.github.io/tree/deploy.svg?style=svg)](https://circleci.com/gh/geekhub-lab/geekhub-lab.github.io/tree/deploy)

https://geekhub.co.kr/

## Setup

You should have [yarn](https://yarnpkg.com/lang/en/) to setup.

```bash
# Clone
git clone -b vuepress git@github.com:geekhub-lab/geekhub-lab.github.io

# Install packages
yarn install

# Run dev server
yarn docs:dev
```

## Deployment

When you `rebase` or `merge` the `vuepress` to `deploy` branch, the CircleCI will auto deploy the static blog to `master` branch. Using `rebase` is recommended rather than `merge`.

Steps:

1. Working on `vuepress` branch
2. When done, `rebase` or `merge` to `deploy`
3. Push to remote `deploy` branch
4. Auto build and deploy will be processed

> `deploy` branch is protected. Only @mingrammer can push to this branch now. If you need to push to `deploy` branch, please contact me.
