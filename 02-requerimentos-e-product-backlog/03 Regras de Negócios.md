# 2.3 REGRAS DE NEGÓCIO

As regras de negócio, diferentemente dos requisitos que foram abordados anteriormente, estipulam as condições e restrições do negócio que devem ser respeitadas pelo sistema, de modo que, para o BairroDelivery, temos as seguintes regras:

## 2.3.1 USUÁRIOS

| **ID** | **Regra de Negócio** |
| --- | --- |
| RN-001 | Para cada conta cadastrada na plataforma, deve haver um endereço de e-mail único a ela associado. |
| RN-002 | Um usuário somente pode realizar as operações para as quais o seu perfil possui as devidas permissões. |
| RN-003 | Para que restaurantes e entregadores possam iniciar suas atividades na plataforma, o cadastro destes deve ser previamente aprovado pela administração. |

## 2.3.2 RESTAURANTES E CARDÁPIOS

| **ID** | **Regra de Negócio** |
| --- | --- |
| RN-004 | O atendimento de um restaurante se limita aos consumidores localizados em um raio de até 5 km. |
| RN-005 | Cabe a cada restaurante definir os valores de seus produtos, bem como a disponibilidade destes. |
| RN-006 | Caso um restaurante esteja fechado ou temporariamente indisponível, este não deve ser capaz de receber novos pedidos. |
| RN-007 | Caso um produto esteja indisponível, não deve ser possível adquiri-lo. |

## 2.3.3 PEDIDOS

| **ID** | **Regra de Negócio** |
| --- | --- |
| RN-008 | Um pedido deve estar associado a um único consumidor e a um único restaurante, de modo que, caso o consumidor queira adquirir produtos de restaurantes distintos, será necessário realizar pedidos independentes. |
| RN-009 | Para que haja um pedido, é necessário que este possua ao menos um produto. |
| RN-010 | O valor total do pedido é definido pela soma dos valores dos produtos e da taxa de entrega, sendo subtraídos desta soma os descontos aplicáveis, caso existam. |
| RN-011 | O endereço no qual será realizada a entrega deve estar dentro da área de atendimento do restaurante. |
| RN-012 | O consumidor pode cancelar o pedido contanto que ainda não tenha sido iniciada a preparação deste. |
| RN-013 | Uma vez confirmado o pedido, alterações nos valores dos produtos não devem alterar o valor anteriormente estabelecido para o pedido. |

## 2.3.4 PAGAMENTOS

| **ID** | **Regra de Negócio** |
| --- | --- |
| RN-014 | Para cada pedido, deve ser definida uma forma de pagamento. |
| RN-015 | Quando o pagamento for antecipado, o pedido somente poderá ser encaminhado para preparação posterior à confirmação do pagamento. |
| RN-016 | Caso um pedido com pagamento antecipado seja cancelado, este deve passar pelo processo de reembolso. |
| RN-024 | As taxas de intermediação devem ser reduzidas, sendo estas previamente informadas aos restaurantes e discriminadas nos registros financeiros, cabendo ao Product Owner aprovar a política e os valores a serem utilizados. |

## 2.3.5 ENTREGAS

| **ID** | **Regra de Negócio** |
| --- | --- |
| RN-017 | Para que um entregador possa receber solicitações de entrega, é necessário que possua um cadastro aprovado e que esteja disponível. |
| RN-018 | Cada entrega deve estar associada ao respectivo pedido e ao entregador responsável por realizá-la. |
| RN-019 | Para que seja iniciada a entrega de um pedido, é necessário que tenha sido concluída a preparação deste. |
| RN-020 | Somente posterior ao registro da coleta é que uma entrega pode ser marcada como concluída. |

## 2.3.6 ADMINISTRAÇÃO

| **ID** | **Regra de Negócio** |
| --- | --- |
| RN-021 | Caso uma conta viole os termos de utilização da plataforma, a administração pode suspendê-la. |
| RN-022 | Quando um restaurante for suspenso, este não deve ser capaz de receber novos pedidos. |
| RN-023 | A suspensão de uma conta não implica a exclusão do histórico de transações associado a ela. |
