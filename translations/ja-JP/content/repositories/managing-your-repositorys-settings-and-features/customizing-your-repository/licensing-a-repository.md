---
title: リポジトリのライセンス
intro: GitHub のパブリックリポジトリは、オープンソース ソフトウェアの共有にも頻繁に利用されています。 リポジトリを真にオープンソースにしたければ、他のユーザが自由にそのソフトウェアを使用でき、変更や配布もできるように、ライセンスを付与する必要があります。
redirect_from:
  - /articles/open-source-licensing
  - /articles/licensing-a-repository
  - /github/creating-cloning-and-archiving-repositories/licensing-a-repository
  - /github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/licensing-a-repository
versions:
  fpt: '*'
  ghes: '*'
  ghec: '*'
topics:
  - Repositories
ms.openlocfilehash: f49dad5c20909647b1d7da7bb44a80a771337966
ms.sourcegitcommit: 47bd0e48c7dba1dde49baff60bc1eddc91ab10c5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/05/2022
ms.locfileid: '145132223'
---
## 適切なライセンスを選択する

コードにライセンスを付与する方法についての理解に役立つ、[choosealicense.com](https://choosealicense.com) を作成しました。 ソフトウェアのライセンスは、ソースコードに対して許可されることとされないことを規定するものなので、十分な情報に基づいて決定することが重要です。

ライセンスの選択は義務ではありませんが、 ライセンスがない場合はデフォルトの著作権法が適用されます。つまり、ソースコードについては作者があらゆる権利を留保し、ソースコードの複製、配布、派生物の作成は誰にも許可されないということです。 オープンソースのプロジェクトを作成する場合は、オープンソース ライセンスを設定することを強くおすすめします。 [オープン ソース ガイド](https://opensource.guide/legal/#which-open-source-license-is-appropriate-for-my-project)には、ご自分のプロジェクトに対する正しいライセンスの選択についての追加のガイダンスが用意されています。

{% note %}

**注:** [利用規約](/free-pro-team@latest/github/site-policy/github-terms-of-service)に従って、ご自分のソース コードを {% data variables.product.product_name %}, {% ifversion fpt or ghec %} のパブリック リポジトリに公開すると {% endif %}{% data variables.product.product_location %} の他のユーザーが、リポジトリを表示およびフォークする権限があります。 すでにリポジトリを作成していて、ユーザによるリポジトリへのアクセスを禁止する場合は、リポジトリをプライベートにすることができます。 リポジトリの表示をプライベートに変更しても、他のユーザによって作成された既存のフォークまたはローカルコピーは存続します。 詳細については、「[リポジトリの可視性を設定する](/github/administering-a-repository/setting-repository-visibility)」を参照してください。

{% endnote %}

## ライセンスの置かれている場所を確認する

ほとんどのユーザーは、ライセンス テキストをリポジトリのルートにある `LICENSE.txt` (または `LICENSE.md` か `LICENSE.rst`) という名前のファイルに配置します。[こちらに Hubot の例を示します](https://github.com/github/hubot/blob/master/LICENSE.md)。

プロジェクトによっては、ライセンスに関する情報は README に記載されています。 たとえばプロジェクトの README には、「当ライセンスは MIT ライセンスの規約に基づいて付与されています」などの文言が書かれていることがあります。

ベスト プラクティスとして、プロジェクトにはライセンス ファイルを含めることをお勧めします。

## ライセンス別に GitHub を検索する

`license` 修飾子と、正確なライセンス キーワードを使用すると、ライセンスまたはライセンス ファミリーに基づいてリポジトリをフィルター処理することができます。

ライセンス | ライセンス キーワード
---  | ---
| Academic Free License v3.0 | `afl-3.0` |
| Apache license 2.0 | `apache-2.0` |
| Artistic license 2.0 | `artistic-2.0` |
| Boost Software License 1.0 | `bsl-1.0` |
| BSD 2-clause "Simplified" license | `bsd-2-clause` |
| BSD 3-clause "New" or "Revised" license | `bsd-3-clause` |
| BSD 3-clause Clear license | `bsd-3-clause-clear` |
| Creative Commons license family | `cc` |
| Creative Commons Zero v1.0 Universal | `cc0-1.0` |
| Creative Commons Attribution 4.0 | `cc-by-4.0` |
| Creative Commons Attribution Share Alike 4.0 | `cc-by-sa-4.0` |
| Do What The F*ck You Want To Public License | `wtfpl` |
| Educational Community License v2.0 | `ecl-2.0` |
| Eclipse Public License 1.0 | `epl-1.0` |
| Eclipse Public License 2.0 | `epl-2.0` |
| European Union Public License 1.1 | `eupl-1.1` |
| GNU Affero General Public License v3.0 | `agpl-3.0` |
| GNU General Public License family | `gpl` |
| GNU General Public License v2.0 | `gpl-2.0` |
| GNU General Public License v3.0 | `gpl-3.0` |
| GNU Lesser General Public License family | `lgpl` |
| GNU Lesser General Public License v2.1 | `lgpl-2.1` |
| GNU Lesser General Public License v3.0 | `lgpl-3.0` |
| ISC | `isc` |
| LaTeX Project Public License v1.3c | `lppl-1.3c` |
| Microsoft Public License | `ms-pl` |
| MIT | `mit` |
| Mozilla Public License 2.0 | `mpl-2.0` |
| Open Software License 3.0 | `osl-3.0` |
| PostgreSQL License | `postgresql` |
| SIL Open Font License 1.1 | `ofl-1.1` |
| University of Illinois/NCSA Open Source License | `ncsa` |
| The Unlicense | `unlicense` |
| zLib License | `zlib` |

ファミリー ライセンス別で検索すると、結果にはそのファミリーのライセンスがすべて含まれます。 たとえば、`license:gpl` というクエリを実行した結果には、GNU General Public License v2.0 と GNU General Public License v3.0 でライセンスされているリポジトリが含まれます。 詳細については、「[リポジトリを検索する](/search-github/searching-on-github/searching-for-repositories/#search-by-license)」を参照してください。

## ライセンスを見つけてもらう

[オープンソース Ruby gem Licensee](https://github.com/licensee/licensee) は、リポジトリの *LICENSE* ファイルと既知のライセンスの短いリストを比較します。 Licensee は [Licenses API](/rest/reference/licenses) も提供しており、[{% data variables.product.product_name %} 上のリポジトリがライセンスを取得する方法に関する分析情報を提供します](https://github.com/blog/1964-open-source-license-usage-on-github-com)。 ご自分のリポジトリが[ライセンス選択の Web サイト](https://choosealicense.com/appendix/)に記載されていないライセンスを使用している場合は、[ライセンスを含めて要求する](https://github.com/github/choosealicense.com/blob/gh-pages/CONTRIBUTING.md#adding-a-license)ことができます。

自分のリポジトリで使用しているライセンスが、ライセンス選択のウェブサイトにはリストされていて、リポジトリ ページのトップに明示的に表示されていない場合には、複数のライセンスが含まれるなど、複雑な状況が考えられます。 ライセンスが検出されるようにするには、*LICENSE* ファイルはシンプルにして、リポジトリの *README* ファイルのなど、どこか別のところで、その複雑さを記します。

## 既存のライセンスでリポジトリにライセンスを適用する

ライセンスを選択できるのは、GitHub で新しいプロジェクトを作成するときだけです。 ブラウザを使って、手動でライセンスを追加できます。 リポジトリにライセンスを追加する方法の詳細については、「[リポジトリへのライセンスの追加](/articles/adding-a-license-to-a-repository)」を参照してください。

![GitHub.com でのライセンス選択のスクリーンショット](/assets/images/help/repository/repository-license-picker.png)

## 免責情報

GitHub がオープンソース ライセンスへの取り組みで目指しているのは、ユーザが十分な情報に基づいて選択できるように基盤を作ることです。 GitHub は、オープンソース ライセンスとそれを使用しているプロジェクトについての情報をユーザが取得できるように、ライセンス情報を掲載しています。 その情報がお役に立つことを願っていますが、GitHub は法律の専門家ではなく、誤りがないとは言えません。 そのため、GitHub は情報を "現状有姿" で提供するものであり、GitHub で、または GitHub を通じて提供する情報またはライセンスについては何らの保証もせず、かかるライセンス情報の利用に起因する損害については責任を負いません。 コードに適したライセンスや、ライセンスに関する他の法的な問題について不明な点がある場合は、必ず専門家にご相談ください。

## 参考資料

- オープン ソース ガイドのセクション "[オープン ソースの法的側面](https://opensource.guide/legal/)"{% ifversion fpt or ghec %}
- [{% data variables.product.prodname_learning %}]({% data variables.product.prodname_learning_link %}){% endif %}
