---
title: 推送更改到 GitHub
shortTitle: Pushing changes
intro: '在本地将更改提交到项目时，您可以将这些更改推送到 {% data variables.product.prodname_dotcom %}，以便其他人可以从远程仓库访问它们。'
permissions: People with write permissions can push changes to a repository.
redirect_from:
  - /desktop/contributing-to-projects/pushing-changes-to-github
  - /desktop/contributing-and-collaborating-using-github-desktop/pushing-changes-to-github
versions:
  fpt: '*'
ms.openlocfilehash: b881fa5d9e66c4a63b8c648d87072037a8cba543
ms.sourcegitcommit: 47bd0e48c7dba1dde49baff60bc1eddc91ab10c5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/05/2022
ms.locfileid: '145085093'
---
## 关于推送更改到 {% data variables.product.prodname_dotcom %}

在推送更改时，会将本地仓库中已提交的更改发送到 {% data variables.product.prodname_dotcom %} 上的远程仓库。 如果在本地更改项目，并且希望其他人也能访问这些更改，您必须将更改推送到 {% data variables.product.prodname_dotcom %}。

在推送更改之前，应更新本地分支以包括已添加到远程仓库的任何提交。 如果有人在不在您本地分支的远程上进行了提交，{% data variables.product.prodname_desktop %} 将在您推送更改之前提示您提取新的提交，以避免合并冲突。 有关详细信息，请参阅“[同步分支](/desktop/contributing-to-projects/syncing-your-branch)”。

{% data reusables.desktop.protected-branches %}

## 推送更改到 {% data variables.product.prodname_dotcom %}

{% note %}

注意：如果超过特定限制，{% data variables.product.prodname_desktop %} 将会拒绝推送。

- 推送包含大小超过 {% data variables.large_files.max_github_size %} 的大文件。
- 推送总大小超过 {% data variables.large_files.max_file_size %}。

如果配置 {% data variables.large_files.product_name_long %} 以跟踪大型文件，您可以推送正常情况下会被拒绝的大型文件。 有关详细信息，请参阅“[关于 {% data variables.large_files.product_name_long %} 和 {% data variables.product.prodname_desktop %}](/desktop/getting-started-with-github-desktop/about-git-large-file-storage-and-github-desktop)”。

{% endnote %}

{% data reusables.desktop.push-origin %}
2. 如果 {% data variables.product.prodname_desktop %} 提示从远程提取新的提交，请单击“提取”。
  ![“提取”按钮](/assets/images/help/desktop/fetch-newer-commits.png)
3. （可选）单击“创建拉取请求”来打开拉取请求并协作进行更改。 有关详细信息，请参阅“[创建议题或拉取请求](/desktop/contributing-to-projects/creating-an-issue-or-pull-request)”![“创建拉取请求”按钮](/assets/images/help/desktop/create-pull-request.png)

## 延伸阅读
- {% data variables.product.prodname_dotcom %} 术语表中的“[推送](/github/getting-started-with-github/github-glossary/#push)”
- “[提交并审查对项目的更改](/desktop/contributing-to-projects/committing-and-reviewing-changes-to-your-project)”
