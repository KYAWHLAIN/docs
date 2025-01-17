---
title: Solicitar uma revisão de pull request
intro: 'Depois de criar uma pull request, você pode pedir para uma pessoa específica revisar as alterações propostas. Se você for um integrante da organização, poderá pedir para uma equipe específica revisar suas alterações.'
product: '{% data reusables.gated-features.multiple-pr-reviewers %}'
redirect_from:
  - /github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review
  - /articles/requesting-a-pull-request-review
  - /github/collaborating-with-issues-and-pull-requests/requesting-a-pull-request-review
  - /github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Pull requests
shortTitle: Solicitar revisão de PR
---

Os repositórios pertencem a uma conta pessoal (um único proprietário) ou a uma conta da organização (uma conta compartilhada com inúmeros colaboradores ou mantenedores). Para obter mais informações, consulte "[Tipos de contas de {% data variables.product.prodname_dotcom %}](/get-started/learning-about-github/types-of-github-accounts)". Proprietários e colaboradores de um repositório pertencente a uma conta pessoal podem atribuir revisões de pull requests. Os integrantes da organização com permissões de triagem também podem atribuir um revisor a um pull request.

Para atribuir um revisor a um pull request, você precisará de acesso de gravação ao repositório. Para obter mais informações sobre o acesso do repositório, consulte "[Funções do repositório para uma organização](/organizations/managing-access-to-your-organizations-repositories/repository-roles-for-an-organization)". Se você tiver acesso de gravação, você pode atribuir a qualquer pessoa que tenha acesso de leitura ao repositório como revisor.

Os integrantes da organização com acesso de gravação também podem atribuir um comentário de pull request a qualquer pessoa ou equipe com acesso de leitura a um repositório. O revisor ou a equipe receberão uma notificação informando que você solicitou a revisão de uma pull request. If you request a review from a team and code review assignment is enabled, specific members will be requested and the team will be removed as a reviewer. Para obter mais informações, consulte "[Gerenciando as configurações de revisão de código para a sua equipe](/organizations/organizing-members-into-teams/managing-code-review-settings-for-your-team)."

{% note %}

**Observação:** os autores da pull request não podem solicitar revisões, a menos que sejam colaboradores ou proprietários do repositório com acesso de gravação no repositório.

{% endnote %}

Você pode solicitar uma revisão para uma pessoa específica ou sugerida. Os revisores sugeridos são baseados nos [dados de blame do Git](/articles/tracking-changes-in-a-file/). Se você solicitar uma revisão, outras pessoas com acesso de leitura no repositório poderão revisar sua pull request. Depois que alguém revisar sua pull request e você fizer as alterações necessárias, você poderá solicitar novamente a revisão do mesmo revisor. Se o revisor solicitado não enviar uma revisão e a pull request atender aos requisitos de mesclagem do repositório [](/articles/defining-the-mergeability-of-pull-requests), você ainda poderá fazer o merge da pull request.

{% data reusables.repositories.sidebar-pr %}
1. Na lista de pull requests, clique na pull request que deve ser revisada por uma pessoa ou equipe específica.
2. Navegue até **Reviewers** (Revisores) na barra lateral direita.
3. Para solicitar a revisão para uma pessoa sugerida, em **Reviewers** (Revisores), clique em **Request** (Solicitar) ao lado do nome de usuário. ![Ícone de solicitação de revisores da barra lateral direita](/assets/images/help/pull_requests/request-suggested-review.png)
5. Opcionalmente, para solicitar a revisão para uma pessoa diferente da pessoa sugerida, clique em **Reviewers** (Revisores) e depois clique em um nome no menu suspenso. ![Ícone de engrenagem de revisores da barra lateral direita](/assets/images/help/pull_requests/request-a-review-not-suggested.png)
6. Opcionalmente, se souber o nome da pessoa ou da equipe da qual deseja a revisão, clique em **Reviewers** (Revisores) e insira o nome de usuário da pessoa ou o nome da equipe para a qual deseja solicitar a revisão das alterações. Clique no nome da equipe ou no nome de usuário para solicitar a revisão. ![Campo para inserir um nome de usuário do revisor e menu com nome do revisor](/assets/images/help/pull_requests/choose-pull-request-reviewer.png)
7. Depois que a pull request for revisada e você fizer as alterações necessárias, você poderá solicitar que ela seja revisada novamente por um revisor. Navegue até **Reviewers** na barra lateral direita e clique em {% octicon "sync" aria-label="The sync icon" %} ao lado do nome do revisor desejado. ![Ícone de sincronização de re-revisão na barra lateral direita](/assets/images/help/pull_requests/request-re-review.png)

## Leia mais

- "[Sobre revisões de solicitação pull](/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews)"
