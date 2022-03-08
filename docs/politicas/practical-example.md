## Controle de Versão

|Date|Version|Update|Author|
|:--:|:----:|:-------:|:---:|
|02/03/2022|1.0|Criação da políca do Git Workflow|Eugênio Siqueira|

# Exemplo prático

* Alterne para a branch `dev` e atualize-a
```bash
git checkout dev
git pull origin dev
```

* Crie a branch com a nova feature
```bash
git checkout -b 3-nome_da_issue
```

* Stage das alterações na branch

```bash
git add nome_do_arquivo_1 nome_do_arquivo_2
```

* Checar status de mudança (verde rastreado e vermelhor não rastreado)
```bash
git status
```

* Commit das alterações na staging (verde)

```bash
git commit -m Adicionar funcionalidade x
```

* Envio dos commits na branch local para o repositório

```bash
git push origin 3-nome_da_issue
```
