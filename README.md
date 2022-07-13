# vuepress-deploy2

0. 创建新仓库 `vuepress-deploy2-target`。可以部署在当前仓库`vuepress-deploy2` 的gh-pages分支，也可以部署在新仓库`vuepress-deploy2-target`的master分支
1. 创建 [Github access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token);
2. 在目标仓库创建一个 [secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets)，填入刚创建的 `token`
3. 如果部署在当前仓库，在 docs/.vuepress/config.js 中设置 base 为 '/vuepress-deploy2/'
4. 如果部署在另一个仓库，在 docs/.vuepress/config.js 中设置 base 为 '/vuepress-deploy2-target/'

参考 [jenkey2011/vuepress-deploy](https://github.com/jenkey2011/vuepress-deploy/)
