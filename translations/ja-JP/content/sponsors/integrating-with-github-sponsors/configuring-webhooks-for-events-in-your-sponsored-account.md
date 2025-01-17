---
title: スポンサードアカウントでイベントに webhook を設定する
intro: 新しいスポンサーシップを受領したとき、または既存のスポンサーシップに変更があったときにアラートがあるように webhook を設定することができます。
redirect_from:
  - /github/supporting-the-open-source-community-with-github-sponsors/configuring-webhooks-for-events-in-your-sponsored-account
versions:
  fpt: '*'
  ghec: '*'
type: how_to
topics:
  - Webhooks
  - Events
  - Open Source
shortTitle: Webhooks for events
ms.openlocfilehash: 2ac78162ae29c10861c7bf3bad8c18b9e0a56ccf
ms.sourcegitcommit: 47bd0e48c7dba1dde49baff60bc1eddc91ab10c5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/05/2022
ms.locfileid: '145118830'
---
## スポンサードアカウントでのイベントの webhook について

支払い期間の終了に伴うキャンセルなど、スポンサーシップに対する変更を監視するために、スポンサードユーザまたはスポンサード Organization のアカウントに webhook を作成できます。 スポンサードアカウントに webhook を設定すると、スポンサーシップが作成、編集、削除されたときにアップデートを受け取れます。 詳しくは、[`sponsorship` Webhook イベント](/webhooks/event-payloads/#sponsorship)に関する記事をご覧ください。

## スポンサードアカウントでイベントの webhook を管理する

{% data reusables.sponsors.navigate-to-sponsors-dashboard %} {% data reusables.sponsors.navigate-to-webhooks-tab %} {% data reusables.sponsors.add-webhook %} {% data reusables.sponsors.add-payload-url %} {% data reusables.sponsors.webhook-content-formatting %} {% data reusables.sponsors.webhook-secret-token %} {% data reusables.sponsors.add-active-triggers %} {% data reusables.sponsors.confirm-add-webhook %} {% data reusables.sponsors.manage-existing-webhooks %}
