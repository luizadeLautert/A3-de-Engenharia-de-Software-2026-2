# 3.2 PERSISTÊNCIA, SEGURANÇA E INTEGRAÇÕES

- Banco de dados relacional: para que seja preservada a integridade das relações entre pedidos, itens, pagamentos e entregas, serão utilizadas transações atômicas nas alterações críticas;
- Pix: para a comunicação com o provedor, será utilizado um adaptador, sendo a confirmação recebida através de um webhook autenticado, utiliza-se o identificador da transação para impedir que esta seja processada mais de uma vez e para acompanhar tanto a conciliação quanto os reembolsos;
- Geolocalização: o cálculo da distância será realizado utilizando-se das coordenadas geográficas, sendo que somente o consumidor associado ao pedido poderá rastrear o entregador enquanto a entrega estiver em andamento;
- Segurança: serão utilizados TLS, hash de senhas com salt, controle de acesso conforme as permissões dos perfis, logs sem dados sensíveis e backups, sendo importante ressaltar que a retenção dos dados deve respeitar a LGPD;
- Acessibilidade: deve ser possível navegar através do teclado, bem como utilizar leitores de tela, sendo necessário garantir o contraste adequado, o foco visível e uma alternativa textual ao mapa.
