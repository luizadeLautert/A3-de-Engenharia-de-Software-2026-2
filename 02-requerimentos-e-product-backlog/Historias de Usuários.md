## Consumidores

| ID | História de Usuário | Requisitos Associados |
|---|---|---|
| HU-001 | Como consumidor, quero criar uma conta para utilizar a plataforma. | RF-001 |
| HU-002 | Como consumidor, quero acessar minha conta para realizar pedidos. | RF-002 |
| HU-003 | Como consumidor, quero recuperar minha senha para restabelecer meu acesso. | RF-003 |
| HU-004 | Como consumidor, quero atualizar meus dados cadastrais para manter minhas informações corretas. | RF-004 |
| HU-005 | Como consumidor, quero visualizar restaurantes próximos para encontrar estabelecimentos que atendam minha região. | RF-006, RF-007 |
| HU-006 | Como consumidor, quero consultar cardápios para escolher os produtos que desejo adquirir. | RF-008 |
| HU-007 | Como consumidor, quero gerenciar meu carrinho para organizar os produtos antes de confirmar o pedido. | RF-011 |
| HU-008 | Como consumidor, quero selecionar uma forma de pagamento para concluir minha compra. | RF-012, RF-021 |
| HU-009 | Como consumidor, quero acompanhar o status do meu pedido para saber quando será entregue. | RF-015 |
| HU-010 | Como consumidor, quero consultar meu histórico de pedidos para visualizar compras anteriores. | RF-016 |

## Restaurantes

| ID | História de Usuário | Requisitos Associados |
|---|---|---|
| HU-011 | Como restaurante, quero gerenciar meu cardápio para manter meus produtos e preços atualizados. | RF-009 |
| HU-012 | Como restaurante, quero alterar a disponibilidade dos produtos para evitar pedidos de itens indisponíveis. | RF-010 |
| HU-013 | Como restaurante, quero receber os pedidos realizados pelos consumidores para iniciar sua preparação. | RF-013 |
| HU-014 | Como restaurante, quero atualizar o status dos pedidos para informar os consumidores sobre o andamento da preparação. | RF-014 |
| HU-015 | Como restaurante, quero consultar meu histórico de pedidos para acompanhar minhas vendas. | RF-016 |

## Entregadores

| ID | História de Usuário | Requisitos Associados |
|---|---|---|
| HU-016 | Como entregador, quero visualizar as entregas atribuídas a mim para organizar minhas atividades. | RF-017, RF-018 |
| HU-017 | Como entregador, quero registrar a coleta do pedido para informar o início da entrega. | RF-019 |
| HU-018 | Como entregador, quero confirmar a conclusão da entrega para finalizar minha atividade. | RF-019 |
| HU-019 | Como entregador, quero consultar meu histórico de entregas para acompanhar minhas atividades anteriores. | RF-020 |

## Administradores

| ID | História de Usuário | Requisitos Associados |
|---|---|---|
| HU-020 | Como administrador, quero gerenciar as contas dos usuários para controlar o acesso à plataforma. | RF-005, RF-024 |
| HU-021 | Como administrador, quero gerenciar os restaurantes cadastrados para garantir o cumprimento das regras da plataforma. | RF-025 |
| HU-022 | Como administrador, quero monitorar os pedidos para acompanhar as operações do sistema. | RF-026 |
| HU-023 | Como administrador, quero consultar relatórios operacionais para avaliar o desempenho da plataforma. | RF-027 |

## Critérios de Aceitação

### HU-005 — Consulta de restaurantes próximos

- O sistema deve considerar o endereço de entrega do consumidor.
- Somente restaurantes dentro do raio de 5 km devem ser apresentados.
- Restaurantes indisponíveis não devem aceitar novos pedidos.

### HU-007 — Gerenciamento do carrinho

- O consumidor deve poder adicionar e remover produtos.
- O consumidor deve poder alterar a quantidade dos produtos.
- O carrinho deve apresentar o valor atualizado dos produtos.
- Todos os produtos devem pertencer ao mesmo restaurante.

### HU-008 — Seleção da forma de pagamento

- O sistema deve apresentar as formas de pagamento disponíveis.
- O consumidor deve selecionar uma forma de pagamento antes de confirmar o pedido.
- O sistema deve informar a confirmação ou falha do pagamento.

### HU-014 — Atualização do status do pedido

- Somente usuários autorizados poderão atualizar o status.
- O consumidor deverá ser informado sobre as alterações.
- O histórico das alterações deverá ser preservado.

### HU-018 — Conclusão da entrega

- A entrega deverá estar associada ao entregador autenticado.
- A coleta deverá ter sido registrada anteriormente.
- O status do pedido deverá ser atualizado para entregue.
