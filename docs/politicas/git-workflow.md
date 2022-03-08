## Controle de Versão

|Date|Version|Update|Author|
|:--:|:----:|:-------:|:---:|
|02/03/2022|1.0|Criação da políca do Git Workflow|Eugênio Siqueira|

# Git Workflow

![Master-Devel](https://user-images.githubusercontent.com/18370133/54881036-5dc07e00-4e2a-11e9-8164-4ee64526939b.png)


## Observações
No projeto Puma:

* A `develop` é equivalente à `dev`
* A `master` é equivalente à `main`

## Develop e Master Branches
Ao invés de uma única branch `master`, esse fluxo de trabalho usa duas branches para registrar o histórico do projeto. A branch `master` armazena o histórico do lançamento oficial, e a branch `develop` serve como uma branch de integração para recursos. Também é conveniente marcar todos os commits na branch `master` com um número de versão.

A primeira etapa serve para complementar a branch `master` padrão com uma branch `develop`. Um jeito simples de alcançar esse resultado é com um desenvolvedor criando uma branch `develop` no local e fazendo o push para o servidor:

## Feature Branches

Cada novo recurso deve residir em sua própria branch, que pode ser enviada ao repositório central para backup/colaboração. Mas, em vez de criar a branch da `master`, as branches de recursos usam a `develop` como seu branch pai. Quando um recurso é concluído, ele é mesclado de volta ao `develop`. Os recursos **nunca** devem interagir diretamente com o `master`.

![Feature Branches](https://user-images.githubusercontent.com/18370133/54881065-97918480-4e2a-11e9-8560-13c1336c05d6.png)

## Criando feature branch

```bash
git checkout develop
git pull origin develop
git checkout -b feature_branch
```

## Finalizando feature branch

Quando você terminar o trabalho de desenvolvimento do recurso, o próximo passo é mesclar o `feature_branch` em `develop`. Você deve então abrir um **Pull Request** de `feature_branch` para `develop`, que será revisado por um dos membros da equipe EPS.

## Referência

[1] https://br.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow

[2] https://br.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
