
## Workflow

![Master-Devel](https://user-images.githubusercontent.com/18370133/54881036-5dc07e00-4e2a-11e9-8164-4ee64526939b.png)

### Observações
No projeto Puma:

* A `develop` é equivalente à `dev`
* A `master` é equivalente à `main`

### Develop e Master Branches
Ao invés de uma única branch `master`, esse fluxo de trabalho usa duas branches para registrar o histórico do projeto. A branch `master` armazena o histórico do lançamento oficial, e a branch `develop` serve como uma branch de integração para recursos. Também é conveniente marcar todos os commits na branch `master` com um número de versão.

A primeira etapa serve para complementar a branch `master` padrão com uma branch `develop`. Um jeito simples de alcançar esse resultado é com um desenvolvedor criando uma branch `develop` no local e fazendo o push para o servidor:

### Feature Branches

Cada novo recurso deve residir em sua própria branch, que pode ser enviada ao repositório central para backup/colaboração. Mas, em vez de criar a branch da `master`, as branches de recursos usam a `develop` como seu branch pai. Quando um recurso é concluído, ele é mesclado de volta ao `develop`. Os recursos **nunca** devem interagir diretamente com o `master`.

![Feature Branches](https://user-images.githubusercontent.com/18370133/54881065-97918480-4e2a-11e9-8560-13c1336c05d6.png)

### Criando Feature Branch

```bash
git checkout develop
git pull origin develop
git checkout -b feature_branch
```

### Finalizando Feature Branch

Quando você terminar o trabalho de desenvolvimento do recurso, o próximo passo é mesclar o `feature_branch` em `develop`. Você deve então abrir um **Pull Request** de `feature_branch` para `develop`, que será revisado por um dos membros da equipe EPS.

### Mantendo Issues

A definição de _done_ de _issues_ abertas:

- Critérios de aceitação completos;
- _Tasks_, se houverem, concluídas.

O _ZenHub_ foi a ferramenta escolhida para auxiliar a equipe na condução do _scrum_, que utilizará sua funcionalidade de _pipelines_ para fins rastreabilidade e transparência do trabalho a ser realizado na _sprint_.

As _pipelines_ utilizadas serão:

- **Backlog** - Todo o _Backlog_ atualizado do produto.
- **Sprint Backlog** - _Issues_/histórias que foram alocadas para a _Sprint._
- **Ice Box** - _Issues_/histórias que foram retiradas da coluna _In Progress_ numa _Sprint_ por algum motivo de força maior.
- **In Progress** - _Issues_/Histórias sendo trabalhadas no momento.
- **Review** - Necessário revisão de EPS.
- **Done** - _Issue_/história concluída.

Assim que uma história técnica ou de usuário respeitar a definição de pronto acordada, e, caso possua testes unitários, e a _build_ esteja passando, o responsável por ela abrirá um _Pull Request_, e assim que for revisado por um membro de EPS, que, caso aceite a história, ela poderá ser movida para _done_. Além disso, a cobertura de testes deverá estar em 90%.

## Política de Adição de Branches

* Branches em português.

* A Branch deve ter uma *TAG* que faça referência ao problema que esta branch resolverá.

* Exemplo:

Uma branch para a issue "#13 Validacao de Cadastro de Usuário" deve ser como:

```git
git checkout -b 13-validacao_cadastro_usuario
```

* Se o título da edição for muito grande, use apenas as primeiras palavras significativas para criá-la

## Política de Commits

* Commits em português

* Um bom commit deve sempre ser capaz de completar a seguinte frase.

> *se aplicado, este commit irá [commit message]*

* Exemplo prático:

```git
git commit -m Corrigir bug no formulário de cadastro de usuário
git commit -m Adicionar funcionalidade de correção de senha
```

## Histórico de Versão

| Data       | Versão | Descrição            | Autores          |
| ---------- | ------ | -------------------- | ---------------- |
| 02/03/2022 | 1.0    | Criação do documento | Eugênio Siqueira |

## Referências

- How to write a git commit message. Disponível em: <https://chris.beams.io/posts/git-commit/>. Acesso em: 02 de março de 2022.
- Fluxo de trabalho de um branch de recurso do Git. Disponível em: <https://br.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow>. Acesso em: 02 de março de 2022.
- Fluxo de trabalho de Gitflow. Disponível em: <https://br.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow>. Acesso em: 02 de março de 2022.