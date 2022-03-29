# 2021-2 PUMA 

Repositório de documentação do projeto PUMA.

## Repositórios de Implementação

[Deploy](https://github.com/fga-eps-mds/2021-2-PUMA-Deploy)

[Front-end](https://github.com/fga-eps-mds/2021-2-PUMA-Frontend)

[Api Gateway](https://github.com/fga-eps-mds/2021-2-PUMA-ApiGateway)

[User Service](https://github.com/fga-eps-mds/2021-2-PUMA-UserService)

[Project Service](https://github.com/fga-eps-mds/2021-2-PUMA-ProjectService)

[Alocate Service](https://github.com/fga-eps-mds/2021-2-PUMA-AlocateService)

[Notify Service](https://github.com/fga-eps-mds/2021-2-PUMA-NotifyService)

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


## GitHub Pages - Desenvolvimento Local 

### Dependências

Virtualenv: 
```console
pip3 install virtualenv
```

### Preparando Ambiente e Subindo Servidor

No diretório raiz do repositório, crie o ambiente: 
```console
virtualenv -p python3 env
```

Ative o ambiente: 

```console
source env/bin/activate
```

Instale o Material mkdocs: 
```console
pip3 install mkdocs-material
```

Inicie o servidor de desenvolvimento:
```console
mkdocs serve
```

## PUMA - Desenvolvimento Local

1. Crie uma pasta para armazenar os repositórios do projeto.

2. Insira os [scripts](https://drive.google.com/drive/folders/11_sBJonAoB_wbzEFLuyG1D0dMOTSvECL?usp=sharing) dentro da pasta criada.

3. Insira a [pasta envs](https://drive.google.com/drive/folders/1bCZ2RPNPU7U_vFwq6A_C2P2FjUKI3q92?usp=sharing) dentro da pasta criada. 

4. Recupere o IP da sua máquina(ifconfig) e insira nas variáveis de IP dos .envs que estão dentro da pasta envs.

5. Entre na pasta criada a partir do terminal.

6. Clone os repositórios do projeto:
   - Via ssh:
        ```console
        source clone_repos_ssh.sh
        ```

   - Via http:
        ```console
        source clone_repos_http.sh
        ```
        
7. Utilize o script move_envs.sh para mover todos os .envs para os seus respectivos repositórios.
    ```console
    source move_envs.sh
    ```

8. Entre no repositório Api-Gateway e execute:
    ```console
    make up-build
    ```

9. Após subir todos os containers com _make up-build_, abra outro terminal na pasta criada na etapa 1 e popule o banco de dados da aplicação:
    ```console
    source db_script.sh populate
    ```

10.   Pronto ! Agora é só acessar http://localhost:8080/
