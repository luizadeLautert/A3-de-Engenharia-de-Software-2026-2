# 2.1 REQUISITOS FUNCIONAIS

Para que o sistema consiga atingir os objetivos previamente definidos, seguem os requisitos funcionais, ou seja, as funções que o sistema deve ser capaz de realizar:

## 2.1.1 ADMINISTRATIVO

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RF-001 | Cadastro de usuários | O sistema deve permitir que consumidores, restaurantes e entregadores realizem seu cadastro na plataforma. |
| RF-002 | Autenticação | Com o cadastro realizado, o usuário deve ser capaz de realizar o login no sistema. |
| RF-003 | Recuperação de senha | O sistema deve possuir um mecanismo que permita ao usuário recuperar o acesso à sua conta. |
| RF-004 | Atualização de perfil | Deve ser possível ao usuário alterar os seus dados cadastrais. |
| RF-005 | Controle de acesso | As funcionalidades disponibilizadas ao usuário devem ser definidas com base no perfil deste e nas permissões a ele associadas. |
| RF-006 | Gerenciamento de estabelecimentos | Deve ser possível aos administradores consultar os restaurantes cadastrados na plataforma, bem como gerenciá-los. |
| RF-007 | Monitoramento de pedidos | Os administradores devem ser capazes de acompanhar os pedidos realizados através da plataforma. |
| RF-008 | Relatórios operacionais | O sistema deve disponibilizar relatórios referentes aos pedidos, às entregas e às demais atividades da plataforma. |

### 2.1.1.1 RESTAURANTES E CARDÁPIOS

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RF-009 | Consulta de restaurantes | O sistema deve apresentar ao consumidor os restaurantes disponíveis na região deste. |
| RF-010 | Filtro geográfico | Para a consulta dos estabelecimentos, o sistema deve utilizar como filtro o limite de atendimento de 5 km. |
| RF-011 | Visualização de cardápios | O sistema deve permitir que o consumidor consulte os produtos, bem como suas descrições e valores. |
| RF-012 | Gerenciamento de cardápios | Deve ser possível aos restaurantes cadastrar produtos em seus cardápios, alterá-los e removê-los. |
| RF-013 | Disponibilidade de produtos | Cabe aos restaurantes informar, através do sistema, quais dos seus produtos estão disponíveis. |

### 2.1.1.2 GERENCIAMENTO DE PEDIDOS

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RF-014 | Carrinho de compras | O consumidor deve ser capaz de adicionar produtos ao carrinho, bem como alterá-los e removê-los deste. |
| RF-015 | Confirmação de pedidos | O sistema deve permitir que o consumidor confirme o pedido, informando o endereço de entrega e a forma de pagamento. |
| RF-016 | Recebimento de pedidos | Os pedidos realizados pelos consumidores devem ser disponibilizados aos respectivos restaurantes. |
| RF-017 | Atualização de status | Deve ser possível aos restaurantes informar o andamento da preparação dos pedidos através da alteração do status destes. |
| RF-018 | Acompanhamento de pedidos | O consumidor deve ser capaz de consultar o status dos seus pedidos. |
| RF-019 | Histórico de pedidos | O sistema deve armazenar os pedidos realizados e permitir a consulta do histórico destes. |
| RF-031 | Cancelamento de pedidos | O sistema deve permitir que o consumidor cancele seu pedido antes que seja iniciada a preparação deste, registrando a alteração e, quando aplicável, iniciando o processo de reembolso. |

### 2.1.1.3 GERENCIAMENTO DE ENTREGAS

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RF-020 | Atribuição de entregas | O sistema deve permitir que os pedidos sejam atribuídos a entregadores que estejam disponíveis. |
| RF-021 | Consulta de entregas | Deve ser possível ao entregador consultar as entregas que lhe foram atribuídas. |
| RF-022 | Atualização de entregas | Cabe ao entregador registrar no sistema tanto a coleta do pedido quanto a conclusão da entrega. |
| RF-023 | Histórico de entregas | O sistema deve permitir a consulta do histórico das entregas realizadas. |
| RF-028 | Rastreamento em tempo real | Durante a entrega, deve ser possível ao consumidor acompanhar a localização do entregador em tempo real. |

### 2.1.1.4 PAGAMENTOS

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RF-024 | Seleção de pagamento | O consumidor deve ser capaz de escolher uma das formas de pagamento disponibilizadas pelo sistema. |
| RF-025 | Registro de pagamento | O sistema deve registrar o status do pagamento, de modo que este esteja associado ao respectivo pedido. |
| RF-026 | Confirmação de pagamento | O sistema deve informar se o pagamento foi confirmado ou se houve uma falha na realização deste. |
| RF-027 | Processamento de reembolsos | Caso seja cancelado um pedido cujo pagamento tenha sido realizado antecipadamente, o sistema deve solicitar o reembolso, registrar o status deste e informar o consumidor acerca do resultado. |
| RF-029 | Pagamento via Pix | O sistema deve permitir que o pagamento seja realizado através de Pix. |
| RF-030 | Conciliação financeira | Para os pagamentos realizados através de Pix, o sistema deve realizar a conciliação financeira dos restaurantes parceiros de forma automática e imediata. |
