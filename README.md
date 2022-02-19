# 2021-2 PUMA 

Repositório de documentação do projeto PUMA.

## Repositórios de Implementação

[Deploy](https://github.com/fga-eps-mds/2021-2-PUMA-Deploy)

[Front-end](https://github.com/fga-eps-mds/2021-2-PUMA-Frontend)

[Api Gateway](https://github.com/fga-eps-mds/2021-2-PUMA-ApiGateway)

[User Service](https://github.com/fga-eps-mds/2021-2-PUMA-UserService)

[Project Service](https://github.com/fga-eps-mds/2021-2-PUMA-ProjectService)

[Notify Service](https://github.com/fga-eps-mds/2021-2-PUMA-NotifyService)

[Alocate Service](https://github.com/fga-eps-mds/2021-2-PUMA-AlocateService)

## Time 

| Matrícula  | Nome                             | Github                                                  |
| ---------- | -------------------------------- | ------------------------------------------------------- |
| 17/0138551 | Bruno Henrique Sousa Duarte      | [Mexazonic](https://github.com/Mexazonic)               |
| 17/0033112 | Eugênio Sales Siqueira           | [Eugeniosales](https://github.com/Eugeniosales)         |
| 20/0018248 | Gabriel Roger Amorim da Cruz     | [GabrielRoger07](https://github.com/GabrielRoger07)     |
| 20/0030264 | Guilherme Nishimura              | [Guilherme-Nishi](https://github.com/Guilherme-Nishi)   |
| 17/0144259 | Gustavo Nogueira Rodrigues       | [Gustavo-Nogueira](https://github.com/Gustavo-Nogueira) |
| 20/0020650 | João Pedro de Camargo Vaz        | [JoaoPedro0803](https://github.com/JoaoPedro0803)       |
| 16/0153204 | Luís Cláudio Telles Lima         | [LuisCL94](https://github.com/LuisCL94)                 |
| 17/0051277 | Nicolas Georgeos Mantzos         | [ngm1450](https://github.com/ngm1450)                   |
| 19/0094478 | Pedro Henrique Noguiera Bragança | [pehenobra2](https://github.com/pehenobra2)             |
| 18/0011472 | Rodolfo Cabral Neves             | [roddas](https://github.com/roddas)                     |
| 20/0028472 | Vinicius Assumpção de Araujo     | [viniman27](https://github.com/viniman27)               |


## Desenvolvimento Local

### Dependências

Virtualenv: 
> $ pip3 install virtualenv

### Preparando Ambiente e Subindo Servidor

No diretório raiz do repositório, crie o ambiente: 
> $ virtualenv -p python3 env

Ative o ambiente: 
> $ source env/bin/active

Instale o Material mkdocs: 
> $ pip3 install mkdocs-material

Inicie o servidor de desenvolvimento:
> $ mkdocs serve

### Rodar o Projeto Localmente
Antes de iniciarmos o tutorial: Abra o Terminal, crie uma pasta em sua área de trabalho. copie o arquivo [clone_pumas.sh](https://github.com/fga-eps-mds/2021-2-PUMA-Doc/blob/main/clone_pumas.sh) nesta pasta vazia.
1) Execute o arquivo .sh
```console
bash clone_pumas.sh
```
2) Adicionar as Variáveis de Ambiente como arquivos .env na raiz de cada repositório

3) Entrar no repositório Api-Gateway e executar
```console
make up-build
```
4) Abrir outro terminal; entrar no docker do banco de dados através do comando
```console
sudo docker ps // Lista os containers rodando e suas informações(ids, nomes, portas, etc)
sudo docker exec -it ID_CONTAINER_postgres bash
```
5) Após entrar no container, executar os seguintes comandos
```console
su - postgres
psql -U username -d puma
Exemplo: psql -U neymar -d puma
```
6) Inserir alguns dados manualmente para execução do projeto
```SQL
> INSERT INTO knowledge_area(knowledgearea) VALUES('Area de Conhecimento');
> INSERT INTO subject(name, coursesyllabus) VALUES('Nome Subject', 'Descricao do Subject');
> INSERT INTO subarea(knowledgeareaid, description) VALUES(1, 'Descricao da Area de conhecimento');
```
7) Acessar o Projeto pelo link gerado
8) Cadastrar o Usuário, Logar e por fim Explorar :)
