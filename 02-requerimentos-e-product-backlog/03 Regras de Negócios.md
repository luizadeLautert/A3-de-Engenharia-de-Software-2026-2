Este documento estabelece as regras de negócio que determinam as condições, restrições e políticas operacionais do BairroDelivery.

## Usuários

| ID | Regra de Negócio |
|---|---|
| RN-001 | Cada conta deverá estar associada a um endereço de e-mail único. |
| RN-002 | Os usuários somente poderão executar operações autorizadas para seu respectivo perfil. |
| RN-003 | Restaurantes e entregadores deverão possuir cadastro aprovado pela administração da plataforma para iniciar suas atividades. |

## Restaurantes e Cardápios

| ID | Regra de Negócio |
|---|---|
| RN-004 | Os restaurantes somente poderão atender consumidores localizados em um raio de até 5 km. |
| RN-005 | Cada restaurante será responsável pela definição dos preços e pela disponibilidade de seus produtos. |
| RN-006 | Restaurantes fechados ou temporariamente indisponíveis não poderão receber novos pedidos. |
| RN-007 | Produtos indisponíveis não poderão ser adquiridos. |

## Pedidos

| ID | Regra de Negócio |
|---|---|
| RN-008 | Cada pedido deverá estar associado a um único consumidor mas pode ter mais de um restaurante. |
| RN-009 | Um pedido deverá conter pelo menos um produto. |
| RN-010 | O valor total do pedido corresponderá à soma dos produtos e da taxa de entrega, descontados eventuais descontos aplicáveis. |
| RN-011 | O endereço de entrega deverá estar dentro da área de atendimento do restaurante. |
| RN-012 | O consumidor poderá cancelar o pedido antes do início de sua preparação. |
| RN-013 | Alterações posteriores nos preços dos produtos não deverão modificar os valores de pedidos já confirmados. |

## Pagamentos

| ID | Regra de Negócio |
|---|---|
| RN-014 | Cada pedido deverá possuir uma forma de pagamento definida. |
| RN-015 | Pedidos com pagamento antecipado somente poderão ser encaminhados para preparação após a confirmação do pagamento. |
| RN-016 | Pedidos cancelados com pagamento antecipado deverão ser submetidos ao processo de reembolso. |

## Entregas

| ID | Regra de Negócio |
|---|---|
| RN-017 | Somente entregadores cadastrados, aprovados e disponíveis poderão receber solicitações de entrega. |
| RN-018 | Cada entrega deverá estar associada a um pedido e a um entregador responsável. |
| RN-019 | Uma entrega somente poderá ser iniciada após a conclusão da preparação do pedido. |
| RN-020 | Uma entrega somente poderá ser marcada como concluída após o registro da coleta. |

## Administração

| ID | Regra de Negócio |
|---|---|
| RN-021 | A administração poderá suspender contas que violem os termos de utilização da plataforma. |
| RN-022 | A suspensão de um restaurante impedirá o recebimento de novos pedidos. |
| RN-023 | A suspensão de uma conta não deverá excluir seu histórico de transações. |
