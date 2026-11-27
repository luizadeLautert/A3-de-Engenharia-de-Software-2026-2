# 2.5 HISTÓRIAS DE USUÁRIO

## 2.5.1 CONSUMIDORES

| **ID** | **História de Usuário** | **Requisitos Associados** |
| --- | --- | --- |
| HU-001 | Como consumidor, quero criar uma conta, de modo a utilizar a plataforma. | RF-001 |
| HU-002 | Como consumidor, quero acessar minha conta, de modo a realizar pedidos. | RF-002 |
| HU-003 | Como consumidor, quero recuperar minha senha para restabelecer meu acesso. | RF-003 |
| HU-004 | Como consumidor, quero atualizar meus dados cadastrais para manter minhas informações corretas. | RF-004 |
| HU-005 | Como consumidor, quero visualizar restaurantes próximos para encontrar estabelecimentos que atendam minha região. | RF-009, RF-010 |
| HU-006 | Como consumidor, quero consultar cardápios, de modo a escolher os produtos que desejo adquirir. | RF-011 |
| HU-007 | Como consumidor, quero gerenciar meu carrinho, de modo a organizar os produtos antes de confirmar o pedido. | RF-014 |
| HU-008 | Como consumidor, quero selecionar uma forma de pagamento para concluir minha compra. | RF-015, RF-024, RF-025, RF-026 |
| HU-009 | Como consumidor, quero acompanhar o status do meu pedido para saber quando será entregue. | RF-018 |
| HU-010 | Como consumidor, quero consultar meu histórico de pedidos para visualizar compras anteriores. | RF-019 |
| HU-024 | Como consumidor, quero acompanhar a localização do entregador em tempo real para saber onde está meu pedido durante a entrega. | RF-028 |
| HU-025 | Como consumidor, quero pagar meu pedido via Pix, de modo a concluir a compra de forma rápida. | RF-029, RF-025, RF-026 |
| HU-027 | Como consumidor com deficiência, quero utilizar a plataforma de forma acessível para realizar pedidos com autonomia. | RNF-010 |
| HU-029 | Como consumidor, quero acompanhar o reembolso de um pedido cancelado, de modo a saber se o valor foi devolvido. | RF-027 |
| HU-030 | Como consumidor, quero cancelar um pedido antes da preparação para desistir da compra quando necessário. | RF-031 |

## 2.5.2 RESTAURANTES

| **ID** | **História de Usuário** | **Requisitos Associados** |
| --- | --- | --- |
| HU-011 | Como restaurante, quero gerenciar meu cardápio, de modo a manter meus produtos e preços atualizados. | RF-012 |
| HU-012 | Como restaurante, quero alterar a disponibilidade dos produtos para evitar pedidos de itens indisponíveis. | RF-013 |
| HU-013 | Como restaurante, quero receber os pedidos realizados pelos consumidores para iniciar sua preparação. | RF-016 |
| HU-014 | Como restaurante, quero atualizar o status dos pedidos, de modo a informar os consumidores sobre o andamento da preparação. | RF-017 |
| HU-015 | Como restaurante, quero consultar meu histórico de pedidos para acompanhar minhas vendas. | RF-019 |
| HU-026 | Como restaurante, quero que os pagamentos via Pix sejam conciliados automaticamente, de modo a acompanhar os valores recebidos sem conferência manual. | RF-030 |

## 2.5.3 ENTREGADORES

| **ID** | **História de Usuário** | **Requisitos Associados** |
| --- | --- | --- |
| HU-016 | Como entregador, quero visualizar as entregas atribuídas a mim, de modo a organizar minhas atividades. | RF-020, RF-021 |
| HU-017 | Como entregador, quero registrar a coleta do pedido, de modo a informar o início da entrega. | RF-022 |
| HU-018 | Como entregador, quero confirmar a conclusão da entrega para finalizar minha atividade. | RF-022 |
| HU-019 | Como entregador, quero consultar meu histórico de entregas para acompanhar minhas atividades anteriores. | RF-023 |

## 2.5.4 ADMINISTRADORES

| **ID** | **História de Usuário** | **Requisitos Associados** |
| --- | --- | --- |
| HU-020 | Como administrador, quero gerenciar as contas dos usuários para controlar o acesso à plataforma. | RF-005 |
| HU-021 | Como administrador, quero gerenciar os restaurantes cadastrados para garantir o cumprimento das regras da plataforma. | RF-006 |
| HU-022 | Como administrador, quero monitorar os pedidos, de modo a acompanhar as operações do sistema. | RF-007 |
| HU-023 | Como administrador, quero consultar relatórios operacionais para avaliar o desempenho da plataforma. | RF-008 |
| HU-028 | Como administrador, quero acompanhar o tempo médio de entrega para verificar o cumprimento da meta de menos de 35 minutos. | RF-008, RNF-024 |

## 2.5.5 CRITÉRIOS DE ACEITAÇÃO

### 2.5.5.1 HU-001 — CADASTRO

- Devem ser validados os campos obrigatórios do cadastro, bem como a unicidade do e-mail informado;
- Quando se tratar do cadastro de um restaurante ou entregador, a conta deve permanecer pendente até que seja aprovada pela administração.

### 2.5.5.2 HU-002 — AUTENTICAÇÃO

- Com as credenciais válidas, deve ser possível ao usuário acessar o sistema conforme as permissões do seu perfil;
- Caso as credenciais sejam inválidas, o sistema não deve criar uma sessão ou expor informações referentes à conta.

### 2.5.5.3 HU-003 — RECUPERAÇÃO DE SENHA

- Deve ser possível ao usuário solicitar a recuperação da senha através do e-mail previamente cadastrado;
- O link ou código utilizado para a recuperação deve possuir um prazo de validade, podendo ser utilizado uma única vez.

### 2.5.5.4 HU-004 — ATUALIZAÇÃO DE PERFIL

- O usuário autenticado deve ser capaz de alterar os seus próprios dados;
- Caso sejam informados dados inválidos ou um e-mail já associado a outra conta, estes não devem ser aceitos.

### 2.5.5.5 HU-005 — CONSULTA DE RESTAURANTES PRÓXIMOS

- Para a consulta dos restaurantes, o sistema deve considerar o endereço de entrega informado pelo consumidor;
- Somente devem ser apresentados os restaurantes que estiverem dentro do raio de 5 km;
- Caso um restaurante esteja indisponível, este não deve aceitar novos pedidos.

### 2.5.5.6 HU-006 — CONSULTA DE CARDÁPIO

- No cardápio, devem constar os produtos, bem como a descrição, o valor e a disponibilidade destes;
- Caso um produto esteja indisponível, não deve ser possível adicioná-lo ao carrinho.

### 2.5.5.7 HU-007 — GERENCIAMENTO DO CARRINHO

- Deve ser possível ao consumidor adicionar produtos ao carrinho e removê-los deste;
- Deve ser possível alterar a quantia de cada produto presente no carrinho;
- Conforme sejam realizadas alterações no carrinho, o valor dos produtos deve ser atualizado;
- Todos os produtos que compõem um pedido devem pertencer ao mesmo restaurante, de modo que compras em restaurantes distintos exijam pedidos independentes (RN-008).

### 2.5.5.8 HU-008 — SELEÇÃO DA FORMA DE PAGAMENTO

- Devem ser apresentadas ao consumidor as formas de pagamento disponíveis e o valor total do pedido, incluindo a taxa de entrega;
- Para que o pedido seja confirmado, o consumidor deve ter definido uma forma de pagamento;
- O sistema deve informar se o pagamento foi confirmado ou se houve uma falha.

### 2.5.5.9 HU-009 — ACOMPANHAMENTO DE PEDIDOS

- O consumidor somente deve ser capaz de consultar os seus próprios pedidos;
- Quando houver uma alteração no status do pedido, esta deve ser disponibilizada em até 5 segundos.

### 2.5.5.10 HU-010 — HISTÓRICO DO CONSUMIDOR

- O sistema deve apresentar somente os pedidos associados ao consumidor autenticado;
- Em cada registro, devem constar a data, o valor e o status do pedido, preservando-se os valores originais.

### 2.5.5.11 HU-011 — GERENCIAMENTO DE CARDÁPIO

- O restaurante autorizado deve ser capaz de cadastrar, alterar e remover os seus próprios produtos;
- O valor atribuído a um produto deve ser válido e, caso este seja alterado posteriormente, a alteração não deve afetar os pedidos já confirmados.

### 2.5.5.12 HU-012 — DISPONIBILIDADE

- Deve ser possível ao restaurante alterar a disponibilidade dos seus próprios produtos;
- Caso um produto esteja indisponível, não deve ser possível adquiri-lo em novos pedidos.

### 2.5.5.13 HU-013 — RECEBIMENTO DE PEDIDOS

- O restaurante deve receber somente os pedidos destinados ao seu estabelecimento;
- Quando se tratar de um pedido com pagamento antecipado, este somente deve ser disponibilizado posterior à confirmação do pagamento.

### 2.5.5.14 HU-014 — ATUALIZAÇÃO DO STATUS DO PEDIDO

- Somente os usuários que possuírem as devidas permissões devem ser capazes de alterar o status do pedido;
- O consumidor deve ser informado das alterações realizadas;
- O sistema deve preservar o histórico das alterações de status.

### 2.5.5.15 HU-015 — HISTÓRICO DO RESTAURANTE

- O restaurante somente deve ser capaz de consultar os pedidos associados ao seu estabelecimento;
- Devem ser preservados no histórico os valores, as datas e os status registrados.

### 2.5.5.16 HU-016 — CONSULTA DE ENTREGAS

- Somente devem ser atribuídas entregas a entregadores aprovados e disponíveis;
- O entregador deve ser capaz de consultar somente as entregas que lhe foram atribuídas.

### 2.5.5.17 HU-017 — REGISTRO DE COLETA

- O registro da coleta somente pode ser realizado pelo entregador responsável pelo pedido;
- Para registrar a coleta, a preparação do pedido deve estar concluída, passando então o status deste a “em entrega”.

### 2.5.5.18 HU-018 — CONCLUSÃO DA ENTREGA

- A entrega deve estar associada ao entregador que está autenticado no sistema;
- A coleta do pedido deve ter sido previamente registrada;
- Com a conclusão da entrega, o status do pedido deve passar a “entregue”.

### 2.5.5.19 HU-019 — HISTÓRICO DE ENTREGAS

- O entregador deve possuir acesso somente ao histórico das suas próprias entregas;
- Em cada registro, devem constar o pedido, a data e o status de conclusão.

### 2.5.5.20 HU-020 — CONTROLE DE CONTAS

- Somente administradores devem ser capazes de alterar as permissões dos usuários ou suspender suas contas;
- Caso uma conta seja suspensa, as operações restritas devem ser impedidas, porém, deve-se preservar o histórico desta.

### 2.5.5.21 HU-021 — GERENCIAMENTO DE RESTAURANTES

- Deve ser possível aos administradores aprovar, consultar e suspender os restaurantes;
- Caso um restaurante esteja suspenso, este não deve receber novos pedidos.

### 2.5.5.22 HU-022 — MONITORAMENTO ADMINISTRATIVO

- O administrador deve ser capaz de consultar os pedidos utilizando como filtros o status, o estabelecimento e o período;
- O acesso a esse painel deve se limitar ao perfil administrativo.

### 2.5.5.23 HU-023 — RELATÓRIOS OPERACIONAIS

- Deve ser possível ao administrador consultar a quantia de pedidos e entregas em um determinado período;
- Os indicadores, dentre eles o tempo médio de entrega, devem ser calculados com base nos registros armazenados pelo sistema.

### 2.5.5.24 HU-024 — RASTREAMENTO EM TEMPO REAL

- Durante a entrega, deve ser possível ao consumidor visualizar a localização do entregador associado ao seu pedido;
- A localização deve ser atualizada de forma automática, sem que o consumidor precise recarregar a interface;
- Com a conclusão da entrega, deve ser encerrado o rastreamento do entregador.

### 2.5.5.25 HU-025 — PAGAMENTO VIA PIX

- O Pix deve constar entre as formas de pagamento disponibilizadas pelo sistema;
- A transação realizada através de Pix deve estar associada ao respectivo pedido, sendo registrado o status desta;
- Caso o pagamento seja antecipado, o pedido somente deve ser encaminhado para preparação posterior à confirmação do pagamento.

### 2.5.5.26 HU-026 — CONCILIAÇÃO FINANCEIRA VIA PIX

- Com o pagamento confirmado, o sistema deve realizar a conciliação da transação com o respectivo pedido e restaurante de forma automática;
- A conciliação deve ser realizada imediatamente após a confirmação do pagamento, sem que haja necessidade de intervenção manual;
- No registro da conciliação, devem constar o valor da transação e o pedido correspondente, sendo que não devem ser gerados registros duplicados.

### 2.5.5.27 HU-027 — ACESSIBILIDADE

- As interfaces devem respeitar os critérios aplicáveis da WCAG 2.2, nível AA;
- Deve ser possível utilizar tanto o teclado quanto tecnologias assistivas para consultar cardápios, realizar pedidos e efetuar pagamentos;
- Os elementos que compõem as interfaces devem possuir rótulos acessíveis, contraste adequado e foco visível.

### 2.5.5.28 HU-028 — TEMPO MÉDIO DE ENTREGA

- Devem ser registrados tanto o horário de confirmação do pedido quanto o de conclusão da entrega;
- Com ambos os horários registrados, deve ser possível calcular no relatório a média do intervalo entre estes, considerando as entregas concluídas dentro do raio de cobertura no período avaliado;
- O indicador deve permitir verificar se a média calculada é inferior a 35 minutos.

### 2.5.5.29 HU-029 — REEMBOLSO

- Caso seja cancelado um pedido cujo pagamento antecipado tenha sido confirmado, deve ser gerada uma solicitação de reembolso associada à respectiva transação;
- O sistema deve registrar o status do reembolso (pendente, concluído ou falha), impedir a duplicidade deste e informar o consumidor.

### 2.5.5.30 HU-030 — CANCELAMENTO

- Somente o consumidor titular deve ser capaz de cancelar o pedido, contanto que ainda não tenha sido iniciada a preparação deste;
- O status do pedido deve passar a “cancelado” e, caso o pagamento tenha sido realizado antecipadamente, inicia-se o processo de reembolso;
- Caso a preparação do pedido já tenha sido iniciada, o sistema não deve aceitar o cancelamento por parte do consumidor.
