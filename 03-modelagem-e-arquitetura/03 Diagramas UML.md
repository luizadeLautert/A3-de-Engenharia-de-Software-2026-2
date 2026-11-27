# 3.3 DIAGRAMAS UML

## 3.3.1 DIAGRAMA DE CASOS DE USO

![Diagrama de casos de uso](diagramas/casos%20de%20uso.png)

No diagrama acima, temos quatro atores que utilizam diretamente do sistema (consumidor, restaurante, entregador e administrador), sendo que cada um possui suas próprias permissões. Além dos quatro atores mencionados, temos o provedor Pix, um ator externo que interage com o sistema nos processos de pagamento, reembolso e conciliação.

## 3.3.2 DIAGRAMA DE CLASSES

![Diagrama de classes](diagramas/classes.png)

Como podemos ver no diagrama, cada pedido é associado a um único consumidor e a um único restaurante, enquanto os itens são partes que compõem o pedido, sendo que cada item possui uma referência ao produto e armazena o valor deste no momento da compra. Um pedido pode ter diversas tentativas de pagamento, porém somente uma entrega. A associação de um usuário como consumidor ou entregador é definida pelo perfil deste.

## 3.3.3 DIAGRAMA DE SEQUÊNCIA — PEDIDO COM PIX

![Diagrama de sequência](diagramas/sequencia.png)

No caso exemplo do diagrama acima, o pagamento é realizado através de Pix, de modo que o pedido somente é encaminhado ao restaurante quando o pagamento for confirmado, caso haja uma falha no pagamento, o pedido não será liberado. Além disso, caso o provedor encaminhe a confirmação mais de uma vez, não deve ocorrer uma segunda conciliação; caso o consumidor cancele o pedido antes do início da preparação, cabe ao Model iniciar o processo de reembolso, quando aplicável.

## 3.3.4 DIAGRAMA DE ATIVIDADES — CICLO DO PEDIDO

![Diagrama de atividades](diagramas/atividades.png)

O diagrama acima representa as etapas pelas quais passa um pedido cujo pagamento é realizado antecipadamente através de Pix. Nota-se que o consumidor pode cancelar o pedido antes que seja iniciada a preparação deste; o rastreamento do entregador começa quando se inicia a entrega propriamente dita e é encerrado quando esta for concluída.
