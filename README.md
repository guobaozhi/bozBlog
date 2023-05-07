# 使用Hugo的hugo-book主题构建文档站点

[![Github Actions][github-action-image]][github-repo-url]
[![license][license-image]](LICENSE)
[![Github Star][github-repo-star-image]][github-repo-url]
[![standard-readme compliant][standard-readme-image]](standard-readme-url)

[背景](#背景) | [介绍](#介绍) | [使用](#使用) | [示例](#示例) | [相关仓库](#相关仓库) | [维护者](#维护者) | [如何贡献](#如何贡献) | [协议](#协议) 

## 背景

使用[Hugo][hugo-website]自动构建文档站点，使用[hugo-book][hugo-book-theme]主题v8版本。

## 介绍

[Hugo][hugo-website]是一个快速建站工具，可以用于创建自己的[博客][my-blog]，使用[hugo-book][hugo-book-theme]主题，可以创建文档站点。
本仓库是一个`Github Template`仓库，可以通过点击[template][generate]快速干净的创建自己的文档站点仓库。

### 详细介绍

1. [README.md](README.md)

    > 自诉文件，包含仓库中文件相关信息的文本文件，通常是仓库访问者看到的第一个文件。自述文件连同仓库许可证、参与指南以及行为准则，帮助您交流要求和管理项目的参与。

2. [README.en-US.md](README.en-US.md)

    > 自诉文件英文版。

3. [LICENSE](LICENSE)

    > 许可，一种可随附于项目的文档，告知们能够对您的源代码执行哪些操作，不能执行哪些操作。

4. [.gitignore](.gitignore)

    > gitignore文件指定Git应该忽略的故意未跟踪的文件。 Git已经跟踪的文件不受影响； 有关详细信息，请参见[链接](https://git-scm.com/docs/gitignore)。

5. [CHANGELOG.md](CHANGELOG.md)

    > 每次发布新版本时，记录新版本变化的特性，以及修改的bug等信息。

6. [CONTRIBUTING.md](CONTRIBUTING.md)

    > 贡献规范，比如代码编写规范，如果提问题、提bug、提需求，如何编写文档等。

7. [.github/COMMIT_CONVERTION.md](.github/COMMIT_CONVERTION.md)

    > git提交信息规范。

8. [.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md)

    > 提交`pull request`模版。

9. [.github/ISSUE_TEMPLATE/bug_report.md](.github/ISSUE_TEMPLATE/bug_report.md)

    > 在`issue`中提bug的模版。

10. [.github/ISSUE_TEMPLATE/custom.md](.github.com/ISSUE_TEMPLATE/custom.md)

    > 自定义`issue`模版。

11. [.github/ISSUE_TEMPLATE/feature_request.md](.github/ISSUE_TEMPLATE/feature_request.md)

    > 在`issue`中提需求的模版。

12. [.github/workflows/main.yml](.github.com/workflows/main.yml)

    > GitHub Action配置文件，可以配置仓库的CI/CD。

## 使用

点击[![使用这个模板][use-this-template]][generate]按钮，复制到你自己的GitHub仓库中。

或者使用`gh`命令行创建项目

```
gh repo create myRepository -p GitHubTemplates/docs-use-hugo-with-hugobook-theme
```

## 示例

一般开源项目的仓库，都需要有一些示例说明或者代码，供使用者参考。

## 相关仓库

- [Hugo](https://github.com/gohugoio/hugo)
- [hugo-book](https://github.com/alex-shpak/hugo-book)

## 维护者

[@BruceMaa](https://github.com/BruceMaa)。

## 如何贡献

非常欢迎你的加入！[提一个 Issue](https://github.com/GitHubTemplates/docs-use-hugo-with-hugobook-theme/issues/new) 或者提交一个 Pull Request。

docs-use-hugo-with-hugobook-theme 遵循 [Contributing](CONTRIBUTING.md) 编写规范。

docs-use-hugo-with-hugobook-theme 遵循 [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) 行为规范。

## 协议

[MIT © Bruce Maa.](LICENSE)

[github-action-image]: https://github.com/GitHubTemplates/docs-use-hugo-with-hugobook-theme/actions/workflows/main.yml/badge.svg
[github-repo-url]: https://github.com/GitHubTemplates/docs-use-hugo-with-hugobook-theme/actions/workflows/main.yml
[license-image]: https://img.shields.io/badge/license-MIT-green.svg
[github-repo-star-image]: https://img.shields.io/github/stars/GitHubTemplates/docs-use-hugo-with-hugobook-theme.svg?style=social
[use-this-template]: https://img.shields.io/badge/-use%20this%20template-brightgreen.svg
[generate]: https://github.com/GitHubTemplates/docs-use-hugo-with-hugobook-theme/generate
[standard-readme-image]: https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square
[standard-readme-url]: https://github.com/RichardLitt/standard-readme
[hugo-website]: https://gohugo.io
[hugo-book-theme]: https://github.com/alex-shpak/hugo-book
[my-blog]: https://brucemaa.cn