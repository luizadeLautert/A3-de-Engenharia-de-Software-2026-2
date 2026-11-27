# 4.3 SPRINT PLANNING E SPRINT BACKLOG

No início de cada Sprint, o Product Owner e os Developers devem analisar os itens do Product Backlog, considerando suas prioridades, as dependências entre eles e a capacidade da equipe; posterior a isso, cabe aos Developers selecionar os itens que serão abordados na Sprint e dividi-los nas atividades necessárias para sua realização. Segue a divisão inicial, que deverá ser validada no Sprint Planning:

## 4.3.1 SPRINT 1 — BASE DE USUÁRIOS, CATÁLOGO, CARRINHO E ACESSIBILIDADE INICIAL

| **Item** | **Trabalho previsto** | **SP** |
| --- | --- | --- |
| PB-001 | Formulário de cadastro, validação de e-mail e aprovação de perfis. | 5 |
| PB-002 | Login, sessão e tratamento de credenciais inválidas. | 5 |
| PB-003 | Permissões por perfil e testes de acesso negado. | 5 |
| PB-004 | Aprovação, consulta e suspensão de restaurantes. | 5 |
| PB-005 | CRUD de produtos, preços e associação ao estabelecimento. | 8 |
| PB-006 | Alterar disponibilidade e impedir compras indisponíveis. | 3 |
| PB-007 | Calcular raio de atendimento e listar restaurantes elegíveis. | 8 |
| PB-008 | Exibir cardápios, preços e disponibilidade. | 3 |
| PB-009 | Adicionar/remover itens, quantidades e recalcular total. | 5 |
| PB-018 | Implementar recuperação com token temporário de uso único. | 3 |
| PB-019 | Editar perfil e validar dados cadastrais. | 3 |
| PB-029 | Criar componentes acessíveis e testar teclado, foco e leitor de tela. | 8 |

## 4.3.2 SPRINT 2 — PEDIDO, PIX, CONCILIAÇÃO E CANCELAMENTO/REEMBOLSO

| **Item** | **Trabalho previsto** | **SP** |
| --- | --- | --- |
| PB-010 | Validar endereço, disponibilidade, restaurante único e valor. | 5 |
| PB-011 | Registrar status de pagamentos e tratar falhas. | 13 |
| PB-012 | Liberar pedidos confirmados ao restaurante correto. | 5 |
| PB-013 | Implementar transições de status e histórico de mudanças. | 5 |
| PB-025 | Cancelar antes da preparação e acionar reembolso. | 5 |
| PB-027 | Gerar cobrança Pix e validar webhook de confirmação. | 8 |
| PB-028 | Conciliar pagamento, pedido e restaurante de forma idempotente. | 8 |
| PB-024 | Solicitar devolução ao provedor e tratar status/duplicidade. | 8 |

## 4.3.3 SPRINT 3 — ENTREGA, RASTREAMENTO E HISTÓRICOS

| **Item** | **Trabalho previsto** | **SP** |
| --- | --- | --- |
| PB-014 | Selecionar entregador aprovado e disponível. | 8 |
| PB-015 | Registrar coleta e impedir coleta prematura. | 3 |
| PB-016 | Registrar conclusão e horário da entrega. | 3 |
| PB-017 | Exibir status atualizado ao consumidor. | 5 |
| PB-020 | Consultar histórico por consumidor/restaurante. | 5 |
| PB-021 | Consultar histórico do entregador autorizado. | 3 |
| PB-026 | Atualizar posição durante a entrega e restringir acesso. | 13 |

## 4.3.4 SPRINT 4 — ADMINISTRAÇÃO, INDICADORES, INTEGRAÇÃO, TESTES E PREPARAÇÃO DA RELEASE

| **Item** | **Trabalho previsto** | **SP** |
| --- | --- | --- |
| PB-022 | Painel administrativo com filtros de pedidos. | 5 |
| PB-023 | Consolidar indicadores por período e validar cálculos. | 8 |
| PB-030 | Calcular média de entrega por período, com horários persistidos. | 5 |
