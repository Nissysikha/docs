---
ms.openlocfilehash: 744983c086ce7f67bb25cd9508e080ceb12ea517
ms.sourcegitcommit: 47bd0e48c7dba1dde49baff60bc1eddc91ab10c5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/05/2022
ms.locfileid: "145096593"
---
No caso em que um cliente atualiza seu plano e o pagamento falhar, o GitHub reverte sua assinatura de {% data variables.product.prodname_marketplace %} ao seu estado anterior. O GitHub também envia um e-mail ao cliente para informá-lo sobre a falha e permitir que ele tente novamente sua compra. Você receberá um webhook com a ação `changed` solicitando que você reverta para o plano anterior.
