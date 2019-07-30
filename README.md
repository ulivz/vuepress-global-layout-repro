# vuepress-global-layout-repro

[![Greenkeeper badge](https://badges.greenkeeper.io/ulivz/vuepress-global-layout-repro.svg)](https://greenkeeper.io/)

> Reproduction of https://github.com/vuejs/vuepress/issues/1304

## Step to reproduce

1. yarn install
2. yarn build
3. You'll see following error:

```bash
TypeError: Cannot read property 'globalLayout' of null
    at AppContext.getThemeConfigValue (/Users/ulivz/Documents/ulivz/vuepress-global-layout-repro/node_modules/@vuepress/core/lib/prepare/AppContext.js:377:65)
    at AppContext.resolveCommonAgreementFilePath (/Users/ulivz/Documents/ulivz/vuepress-global-layout-repro/node_modules/@vuepress/core/lib/prepare/AppContext.js:301:35)
    at AppContext.resolveGlobalLayout (/Users/ulivz/Documents/ulivz/vuepress-global-layout-repro/node_modules/@vuepress/core/lib/prepare/AppContext.js:271:30)
    at AppContext.process (/Users/ulivz/Documents/ulivz/vuepress-global-layout-repro/node_modules/@vuepress/core/lib/prepare/AppContext.js:99:10)
    at process._tickCallback (internal/process/next_tick.js:68:7)
```
