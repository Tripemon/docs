---
title: codespace の既定の環境変数
shortTitle: Default environment variables
product: '{% data reusables.gated-features.codespaces %}'
intro: '{% data variables.product.prodname_dotcom %} は、codespace ごとに既定の環境変数を設定します。'
versions:
  fpt: '*'
  ghec: '*'
type: overview
topics:
  - Codespaces
  - Fundamentals
  - Developer
ms.openlocfilehash: e9034fb566c8245fff6d610ff456084dc9818f0b
ms.sourcegitcommit: 43a959b8faf78d9c5b3deadffa079d24cd11650b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/04/2022
ms.locfileid: '148134772'
---
## 既定の環境変数について

{% data variables.product.prodname_dotcom %} は、すべての codespace に既定の環境変数を設定します。 codespace で実行されるコマンドは、環境変数を作成、読み取り、変更できます。

{% note %}

**注**: 環境変数では、大文字と小文字が区別されます。

{% endnote %}

## 既定の環境変数のリスト

| 環境変数 | 説明 |
| ---------------------|------------ |
| `CODESPACE_NAME` | codespace の名前 (`monalisa-github-hello-world-2f2fsdf2e` など) |
| `CODESPACES` | codespace にいる間は常に `true` |
| `GIT_COMMITTER_EMAIL` | 将来の `git` コミットの [作成者] フィールドのメール アドレス。 |
| `GIT_COMMITTER_NAME` | 将来の `git` コミットの [コミッター] フィールドの名前。 |
| `GITHUB_CODESPACES_PORT_FORWARDING_DOMAIN`| {% data variables.product.prodname_github_codespaces %} 転送ポートのドメインを返します。 たとえば、`preview.app.github.dev` のようにします。 |
| `GITHUB_API_URL` | API URL を返します。 たとえば、`{% data variables.product.api_url_code %}` のようにします。 |
| `GITHUB_GRAPHQL_URL` | グラフ QL API の URL を返します。 たとえば、`{% data variables.product.graphql_url_code %}` のようにします。 |
| `GITHUB_REPOSITORY` | 所有者およびリポジトリの名前。 たとえば、`octocat/Hello-World` のようにします。 |
| `GITHUB_SERVER_URL`| {% data variables.product.product_name %} サーバーの URL を返します。 たとえば、`https://{% data variables.product.product_url %}` のようにします。 |
| `GITHUB_TOKEN` | codespace 内のユーザーを表す署名付き認証トークン。 これを使用して、GitHub API に対して認証済みの呼び出しを行うことができます。 詳細については、[認証](/codespaces/codespaces-reference/security-in-codespaces#authentication)に関するページをご覧ください。  |
| `GITHUB_USER` | codespace を開始したユーザーの名前。 たとえば、「 `octocat` 」のように入力します。 |
