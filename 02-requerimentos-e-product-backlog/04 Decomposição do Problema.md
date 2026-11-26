## Módulos do Sistema

| ID | Módulo | Responsabilidade | Requisitos Associados |
|---|---|---|---|
| MOD-001 | Gerenciamento de Usuários | Gerenciar contas, autenticação, perfis e permissões. | RF-001 a RF-005 |
| MOD-002 | Restaurantes e Cardápios | Gerenciar estabelecimentos, produtos, preços e disponibilidade geográfica. | RF-006 a RF-010 |
| MOD-003 | Gerenciamento de Pedidos | Gerenciar carrinhos, pedidos, histórico e status de preparação. | RF-011 a RF-016 |
| MOD-004 | Gerenciamento de Entregas | Gerenciar a atribuição, coleta e conclusão das entregas. | RF-017 a RF-020 |
| MOD-005 | Pagamentos | Gerenciar formas de pagamento e confirmação de transações. | RF-021 a RF-023 |
| MOD-006 | Administração | Gerenciar usuários, estabelecimentos e indicadores operacionais. | RF-024 a RF-027 |

## Decomposição dos Módulos

### Gerenciamento de Usuários

- Cadastro de usuários.
- Autenticação.
- Recuperação de senha.
- Gerenciamento de perfis.
- Controle de permissões.

### Restaurantes e Cardápios

- Consulta de estabelecimentos.
- Filtragem geográfica.
- Consulta de cardápios.
- Gerenciamento de produtos.
- Controle de disponibilidade.

### Gerenciamento de Pedidos

- Gerenciamento do carrinho.
- Confirmação de pedidos.
- Recebimento de pedidos.
- Acompanhamento da preparação.
- Histórico de pedidos.

### Gerenciamento de Entregas

- Atribuição de entregadores.
- Consulta de entregas.
- Registro de coleta.
- Confirmação de entrega.
- Histórico de entregas.

### Pagamentos

- Seleção da forma de pagamento.
- Registro de transações.
- Confirmação de pagamentos.
- Processamento de reembolsos.

### Administração

- Gerenciamento de contas.
- Gerenciamento de estabelecimentos.
- Monitoramento de operações.
- Emissão de relatórios.

## Dependências entre Módulos

| Módulo | Dependências |
|---|---|
| Gerenciamento de Usuários | Nenhuma dependência funcional direta. |
| Restaurantes e Cardápios | Gerenciamento de Usuários. |
| Gerenciamento de Pedidos | Gerenciamento de Usuários; Restaurantes e Cardápios. |
| Pagamentos | Gerenciamento de Pedidos. |
| Gerenciamento de Entregas | Gerenciamento de Usuários; Gerenciamento de Pedidos. |
| Administração | Todos os demais módulos. |
