# 2.4 DECOMPOSIÇÃO DO PROBLEMA

## 2.4.1 MÓDULOS DO SISTEMA

| **ID** | **Módulo** | **Responsabilidade** | **Requisitos Associados** |
| --- | --- | --- | --- |
| MOD-001 | Gerenciamento de Usuários | Gerenciar contas, autenticação, perfis e permissões. | RF-001 a RF-005 |
| MOD-002 | Restaurantes e Cardápios | Gerenciar estabelecimentos, produtos, preços e disponibilidade geográfica. | RF-009 a RF-013 |
| MOD-003 | Gerenciamento de Pedidos | Gerenciar carrinhos, pedidos, histórico, cancelamentos e status de preparação. | RF-014 a RF-019, RF-031 |
| MOD-004 | Gerenciamento de Entregas | Gerenciar a atribuição, coleta, rastreamento e conclusão das entregas. | RF-020 a RF-023, RF-028; RNF-024 |
| MOD-005 | Pagamentos | Gerenciar formas de pagamento, confirmação, reembolsos e conciliação financeira de transações Pix. | RF-024 a RF-027, RF-029, RF-030 |
| MOD-006 | Administração | Gerenciar usuários, estabelecimentos e indicadores operacionais. | RF-005 a RF-008; RNF-024 |

É importante ressaltar que o requisito de acessibilidade (RNF-010) não se refere somente a um módulo em específico, devendo ser respeitado nas interfaces de todos os módulos definidos.

## 2.4.2 DECOMPOSIÇÃO DOS MÓDULOS

### 2.4.2.1 GERENCIAMENTO DE USUÁRIOS

- Cadastro dos usuários no sistema;
- Autenticação dos usuários cadastrados;
- Recuperação da senha de acesso;
- Gerenciamento dos dados dos perfis;
- Controle das permissões associadas a cada perfil.

### 2.4.2.2 RESTAURANTES E CARDÁPIOS

- Consulta dos estabelecimentos;
- Filtragem dos estabelecimentos com base na localização geográfica;
- Consulta dos cardápios dos restaurantes;
- Gerenciamento dos produtos que compõem os cardápios;
- Controle da disponibilidade dos produtos.

### 2.4.2.3 GERENCIAMENTO DE PEDIDOS

- Gerenciamento dos produtos no carrinho;
- Confirmação dos pedidos realizados;
- Recebimento dos pedidos pelos restaurantes;
- Acompanhamento do andamento da preparação;
- Consulta do histórico de pedidos;
- Cancelamento de pedidos.

### 2.4.2.4 GERENCIAMENTO DE ENTREGAS

- Atribuição dos pedidos aos entregadores;
- Consulta das entregas atribuídas;
- Registro da coleta do pedido;
- Confirmação da conclusão da entrega;
- Consulta do histórico de entregas;
- Rastreamento da localização do entregador em tempo real.

### 2.4.2.5 PAGAMENTOS

- Escolha da forma de pagamento;
- Registro das transações realizadas;
- Confirmação dos pagamentos;
- Realização do processo de reembolso;
- Realização de pagamentos através de Pix;
- Conciliação financeira automática dos pagamentos realizados através de Pix.

### 2.4.2.6 ADMINISTRAÇÃO

- Gerenciamento das contas dos usuários;
- Gerenciamento dos estabelecimentos cadastrados;
- Acompanhamento das operações realizadas na plataforma;
- Emissão dos relatórios operacionais;
- Acompanhamento do tempo médio de entrega.

## 2.4.3 DEPENDÊNCIAS ENTRE MÓDULOS

| **Módulo** | **Dependências** |
| --- | --- |
| Gerenciamento de Usuários | Nenhuma dependência funcional direta. |
| Restaurantes e Cardápios | Gerenciamento de Usuários. |
| Gerenciamento de Pedidos | Gerenciamento de Usuários; Restaurantes e Cardápios; integração com Pagamentos para confirmação e reembolso. |
| Pagamentos | Gerenciamento de Pedidos. |
| Gerenciamento de Entregas | Gerenciamento de Usuários; Gerenciamento de Pedidos. |
| Administração | Todos os demais módulos. |
