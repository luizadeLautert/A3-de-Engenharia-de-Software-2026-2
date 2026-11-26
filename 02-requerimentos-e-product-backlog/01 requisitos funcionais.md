Documento desenvolvido para levantar e explicar os requisitos funcionais esperados no sistema e regras de negocio associadas.

# Requisitos Funcionais
##  Administrativo
| ID | Requisito | Descrição |
|---|---|---|
| RF-001 | Cadastro de usuários | O sistema deve permitir o cadastro de consumidores, restaurantes e entregadores. |
| RF-002 | Autenticação | O sistema deve permitir que usuários cadastrados realizem login. |
| RF-003 | Recuperação de senha | O sistema deve disponibilizar um mecanismo de recuperação de acesso. |
| RF-004 | Atualização de perfil | O sistema deve permitir a atualização dos dados cadastrais. |
| RF-005 | Controle de acesso | O sistema deve disponibilizar funcionalidades conforme o perfil e as permissões do usuário. |
| RF-006 | Gerenciamento de estabelecimentos | Os administradores devem poder consultar e gerenciar restaurantes cadastrados. |
| RF-007 | Monitoramento de pedidos | Os administradores devem poder acompanhar os pedidos realizados na plataforma. |
| RF-008 | Relatórios operacionais | O sistema deve disponibilizar relatórios sobre pedidos, entregas e atividades da plataforma. |
### Restaurantes e Cardápios

| ID | Requisito | Descrição |
|---|---|---|
| RF-009 | Consulta de restaurantes | O sistema deve apresentar restaurantes disponíveis na região do consumidor. |
| RF-010 | Filtro geográfico | O sistema deve filtrar os estabelecimentos conforme o limite de atendimento de 5 km. |
| RF-011 | Visualização de cardápios | O sistema deve permitir a consulta de produtos, descrições e preços. |
| RF-012 | Gerenciamento de cardápios | Os restaurantes devem poder cadastrar, editar e remover produtos. |
| RF-013 | Disponibilidade de produtos | Os restaurantes devem poder informar a disponibilidade de seus produtos. |

### Gerenciamento de Pedidos

| ID | Requisito | Descrição |
|---|---|---|
| RF-014 | Carrinho de compras | O consumidor deve poder adicionar, alterar e remover produtos do carrinho. |
| RF-015 | Confirmação de pedidos | O sistema deve permitir a confirmação de pedidos com endereço e forma de pagamento. |
| RF-016 | Recebimento de pedidos | Os restaurantes devem receber os pedidos realizados pelos consumidores. |
| RF-017 | Atualização de status | Os restaurantes devem poder atualizar o andamento da preparação dos pedidos. |
| RF-018 | Acompanhamento de pedidos | O consumidor deve poder consultar o status de seus pedidos. |
| RF-019 | Histórico de pedidos | O sistema deve armazenar e disponibilizar o histórico de pedidos. |

### Gerenciamento de Entregas

| ID | Requisito | Descrição |
|---|---|---|
| RF-020 | Atribuição de entregas | O sistema deve permitir a atribuição de pedidos a entregadores disponíveis. |
| RF-021 | Consulta de entregas | O entregador deve poder visualizar as entregas atribuídas. |
| RF-022 | Atualização de entregas | O entregador deve poder registrar a coleta e a conclusão de uma entrega. |
| RF-023 | Histórico de entregas | O sistema deve disponibilizar o histórico de entregas realizadas. |

### Pagamentos

| ID | Requisito | Descrição |
|---|---|---|
| RF-024 | Seleção de pagamento | O consumidor deve poder selecionar uma forma de pagamento disponível. |
| RF-025 | Registro de pagamento | O sistema deve registrar o status do pagamento associado ao pedido. |
| RF-026 | Confirmação de pagamento | O sistema deve informar a confirmação ou falha do pagamento. |


