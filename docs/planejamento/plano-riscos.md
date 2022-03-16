## Escopo
Este documento visa documentar os riscos que afetam a realização do projeto, analizar seus impactos e registrar o plano de contingência para a ocorrência de cada risco.

## Riscos e suas consequências

### Riscos de projeto:

### Riscos técnicos
| ID | Risco | Consequêcia |
|--|--|--|
| 1 | Dificuldade com as tecnologias escolhidas | Atraso e diminuição da qualidade das entregas  |
| 2 | Dificuldade na adaptação do projeto | Atraso e diminuição da qualidade das entregas  |

### Riscos de gerenciamento
| ID | Risco | Consequêcia |
|--|--|--|
| 3 | Mudança de escopo | Alteração no cronograma e redefinição de requisitos |
| 4 | Falha na comunicação | Erros no projeto e entreguas diferentes do esperado |
| 5 | Falta de organização de EPS | Diminui a qualidade e gera atraso nas entregas |

### Riscos organizacionais
| ID | Risco | Consequêcia |
|--|--|--|
| 6 | Desistência de membros | Sobrecarga dos membros remanescentes |
| 7 | Atraso nas entregas | Não cumprimento do Roadmap e datas estabelecidas |

### Riscos externos
| ID | Risco | Consequêcia |
|--|--|--|
| 8 | Problemas de saúde entre os membros  | Atraso nas entregas e falta nas reuniões |
| 9 | Greve na UnB | O projeto fica inviável

<hr>

### Riscos de produto
| ID | Risco | Consequêcia |
|--|--|--|
| 10 | Ambiente de homologação descontinuado | O ambiente de homologação deixar de existir no término do semestre |


## Probabilidade x Impacto

| Probabilidade | % de certeza | Peso |
|--|--|--|
| Nula | 0% | 0 |
| Muito baixa | 0 a 20% | 1 |
| Baixa | 20 a 40% | 2 |
| Média | 40 a 60% | 3 |
| Alta | 60 a 80% | 4 |
| Muito alta | 80 a 100% | 5 |

| Impacto | Impacto sobre o Custo Original (%) | Peso |
|--|--|--|
| Nulo | 0% | 0 |
| Muito baixo | 1 a 5% | 1 |
| Baixo | 5 a 10% | 2 |
| Médio | 10 a 15% | 3 |
| Alto | 15 a 20% | 4 |
| Muito alto | Acima de 20% | 5 |

### Grau de risco:

O grau de risco é definido pela multiplicação da probabilidade pelo impacto. Sendo:

1. Risco >= 15: Elevado
2. 5 < Risco < 15: Médio
3. Risco =< 5: Baixo

<table class="table table-hover">
    <thead>
        <tr>
            <th scope="col">#</th>
            <th scope="col">Descrição</th>
            <th scope="col">Probabilidade</th>
            <th scope="col">Impacto</th>
            <th scope="col">Risco</th>
        </tr>
    </thead>
    <tbody>
        <tr class="table-danger">
            <th scope="row">1</th>
            <td>Dificuldade com as tecnologias escolhidass</td>
            <td> 4 </td>
            <td> 4 </td>
            <td> 16 </td>
        </tr>
        <tr class="table-warning">
            <th scope="row">2</th>
            <td>Dificuldade na adaptação do projeto</td>
            <td> 3 </td>
            <td> 4 </td>
            <td> 12 </td>
        </tr>
        <tr class="table-info">
            <th scope="row">3</th>
            <td>Mudança de escopo</td>
            <td> 1 </td>
            <td> 3 </td>
            <td> 3 </td>
        </tr>
        <tr class="table-warning">
            <th scope="row">4</th>
            <td>Falha na comunicação</td>
            <td> 2 </td>
            <td> 3 </td>
            <td> 6 </td>
        </tr>
        <tr class="table-warning">
            <th scope="row">5</th>
            <td>Falta de organização de EPS</td>
            <td> 3 </td>
            <td> 4 </td>
            <td> 12 </td>
        </tr>
        <tr class="table-danger">
            <th scope="row">6</th>
            <td>Desistência de membros</td>
            <td> 3 </td>
            <td> 5 </td>
            <td> 15 </td>
        </tr>
        <tr class="table-warning">
            <th scope="row">7</th>
            <td>Atraso nas entregas</td>
            <td> 5 </td>
            <td> 2 </td>
            <td> 10 </td>
        </tr>
        <tr class="table-warning">
            <th scope="row">8</th>
            <td>Problemas de saúde</td>
            <td> 3 </td>
            <td> 3 </td>
            <td> 9 </td>
        </tr>
        <tr class="table-info">
            <th scope="row">9</th>
            <td>Greve na UnB</td>
            <td> 1 </td>
            <td> 5 </td>d
            <td> 5 </td>
        </tr>
        <tr class="table-info">
            <th scope="row">10</th>
            <td>Ambiente de homologação descontinuado</td>
            <td> 1 </td>
            <td> 5 </td>
            <td> 5 </td>
        </tr>
    </tbody>
</table>
<br>
<br>

## Planejamento de resposta aos riscos

| # | Descrição | Risco | Ação | Descrição da ação | Responsável |
| -- | -- | -- | -- | -- | -- |
| 1 | Dificuldade com as tecnologias escolhidas | 6 | Previnir | Realizar treinamentos e acompanhar diariamente o aprendizado das tecnologias | EPS |
| 2 | Dificuldade na adaptação do projeto | 12 | Mitigar | Fazer acompanhamentos em horários específicos com o time de MDS | EPS |
| 3 | Mudança de escopo | 5 | Previnir | Construindo o escopo continuamente com os stakeholders | EPS |
| 4 | Falha na comunicação | 6 | Previnir | Incentivando a comunicação entre os membros nas reuniões e grupos | EPS |
| 5 | Falta de organização de EPS | 12 | Mitigar | Corrigir os problemas visualizados a cada sprint e aperfeiçoar em sprints seguintes | EPS |
| 6 | Desistência de membros | 15 | Aceitar | Realocar tarefas | EPS |
| 7 | Atraso nas entregas | 10 | Previnir | Fazer um acompanhamento mais de perto do andamento das tarefas para que não haja impeditivos | EPS | 
| 8 | Problemas de saúde | 9 | Previnir | Tentar adaptar o capacity enquanto o membro se encontra ausente | EPS |
| 9 | Greve na UnB | 5 | Aceitar | Retomar as atividades quando as aulas normalizarem | EPS |
| 10 | Ambiente de homologação descontinuado | 5 | Previnir | Hospedar projeto em um cloud gratuito e passar as senhas para os stakeholders | EPS |


# Histórico de Revisão

| Data | Versão | Modificação | Autor |
| :-- | :-- | :-- | :-- |
| 16/03/2022 | 0.1 | Criação do documento| Bruno Duarte |
| 16/03/2022 | 0.2 | Criação dos tópicos| Eugênio Sales e Luís Cláudio |
