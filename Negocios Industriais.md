👨‍🏭 Mapeamento de Regras de Negócio Industriais

Industrial Control Tower

1. Objetivo

Este documento reúne as principais regras de negócio consideradas para o Industrial Control Tower. O objetivo é definir condições que devem ser respeitadas durante os processos de pedidos, estoque, produção e logística.

As regras foram organizadas considerando uma indústria de fabricação de cabos, utilizando situações simuladas para representar o funcionamento da operação.

2. Regras gerais

Código

Regra

RN01

Todo pedido deverá possuir um cliente, produtos, quantidades e prazo de entrega.

RN02

Toda ordem de produção deverá estar relacionada a um produto e a uma quantidade planejada.

RN03

A produção deverá considerar a disponibilidade das matérias-primas necessárias.

RN04

Cada linha de produção deverá possuir uma capacidade definida.

RN05

As movimentações de estoque deverão ser registradas para manter o histórico dos materiais.

RN06

As informações dos setores deverão estar relacionadas para permitir o acompanhamento da operação.

3. Regras de pedidos

Código

Regra

RN07

Um pedido não poderá ser acompanhado sem identificação do cliente.

RN08

O prazo de entrega deverá ser registrado no momento do cadastro do pedido.

RN09

Pedidos deverão possuir um status para indicar sua situação atual.

RN10

Um pedido poderá estar relacionado a uma ou mais ordens de produção.

RN11

Pedidos próximos do prazo e sem avanço produtivo deverão ser analisados como possíveis riscos de atraso.

4. Regras de estoque

Código

Regra

RN12

Cada matéria-prima deverá possuir uma quantidade disponível registrada.

RN13

O estoque mínimo deverá ser utilizado como referência para identificar materiais críticos.

RN14

Quando a quantidade disponível atingir ou ficar abaixo do estoque mínimo, deverá ser gerado um alerta.

RN15

O consumo de materiais deverá ser relacionado às ordens de produção correspondentes.

RN16

A quantidade disponível deverá ser considerada antes de liberar uma produção.

RN17

As entradas e saídas de materiais deverão atualizar o saldo do estoque.

RN18

O sistema deverá identificar quando a quantidade disponível não for suficiente para atender à demanda programada.

5. Regras de produção

Código

Regra

RN19

Toda ordem de produção deverá possuir produto, quantidade planejada e linha de produção definida.

RN20

A quantidade produzida deverá ser acompanhada em relação à quantidade planejada.

RN21

O andamento de cada ordem deverá possuir um status atualizado.

RN22

A capacidade disponível da linha deverá ser considerada no planejamento da produção.

RN23

Quando a demanda ultrapassar a capacidade disponível, o sistema deverá identificar uma possível sobrecarga.

RN24

Ordens com prazo comprometido deverão ser destacadas para análise da gestão.

6. Regras de logística

Código

Regra

RN25

Toda entrega deverá estar relacionada a um pedido.

RN26

A previsão de entrega deverá considerar o prazo informado no pedido e a situação da produção.

RN27

Pedidos com atrasos na produção deverão ser sinalizados para acompanhamento logístico.

RN28

Quando houver risco de atraso, a logística deverá conseguir visualizar os pedidos afetados.

7. Regras de inteligência operacional

Código

Regra

RN29

O sistema deverá comparar os prazos dos pedidos com o andamento das ordens de produção.

RN30

O risco de falta de materiais deverá considerar o estoque disponível e o consumo previsto.

RN31

A identificação de gargalos deverá comparar a capacidade produtiva com a demanda programada.

RN32

Uma ocorrência em determinado setor deverá ser relacionada aos demais setores afetados, quando houver dependência entre eles.

RN33

Os alertas deverão possuir níveis de criticidade.

RN34

As recomendações apresentadas deverão servir como apoio à decisão dos responsáveis.

RN35

O sistema deverá manter um histórico dos alertas e das ocorrências identificadas.

8. Níveis de criticidade dos alertas

Nível

Situação

Baixo

Situação que merece acompanhamento, mas não apresenta impacto imediato identificado.

Médio

Problema que pode afetar o andamento de um pedido ou processo.

Alto

Situação com possibilidade de comprometer a produção ou o prazo de entrega.

Crítico

Ocorrência com impacto significativo em diferentes setores da operação.

A classificação deverá considerar as informações disponíveis e poderá ser ajustada conforme as regras definidas pela equipe.

9. Cenários de aplicação

Cenário 1 — Falta de matéria-prima

O estoque apresenta quantidade insuficiente de determinado material para atender à produção programada.

O sistema deverá identificar as ordens afetadas, relacionar os pedidos envolvidos e gerar um alerta para o responsável pelo estoque.

Cenário 2 — Pedido com risco de atraso

Um pedido possui prazo de entrega próximo, mas sua produção ainda não foi iniciada.

O sistema deverá destacar o pedido e permitir que a gestão acompanhe a situação.

Cenário 3 — Sobrecarga na produção

Uma linha de produção recebe uma demanda superior à sua capacidade disponível.

O sistema deverá identificar as ordens afetadas e indicar a necessidade de revisão do planejamento.

Cenário 4 — Problema com impacto em vários setores

Uma matéria-prima indisponível compromete uma ordem de produção, que pode prejudicar um pedido e gerar atraso na entrega.

O sistema deverá relacionar essas informações para apresentar o impacto completo da ocorrência.

10. Considerações finais

O mapeamento das regras de negócio ajuda a estabelecer como o Industrial Control Tower deverá interpretar as informações e acompanhar os processos industriais.

Essas regras servirão como referência para o desenvolvimento do backend, a organização do banco de dados e a implementação dos alertas e análises operacionais.

Os critérios e limites que ainda não foram definidos deverão ser validados pela equipe durante o desenvolvimento do projeto.
