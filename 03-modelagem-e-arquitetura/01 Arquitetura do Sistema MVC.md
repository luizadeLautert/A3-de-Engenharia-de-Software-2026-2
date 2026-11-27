# 3.1 ARQUITETURA DO SISTEMA — MVC

Para o nosso sistema, foi escolhido o padrão Model–View–Controller (MVC), aplicado a uma arquitetura de monólito modular; o padrão MVC divide as responsabilidades do sistema entre três componentes, de modo que uma alteração na interface, por exemplo, não necessariamente exige uma alteração nas regras de negócio. Já a escolha do monólito modular parte da possibilidade de dividirmos o sistema nos módulos previamente definidos sem que, inicialmente, seja necessário utilizar microserviços.

| **Componente** | **Responsabilidade** | **Limites** |
| --- | --- | --- |
| Model | Entidades, regras de negócio, serviços de domínio e interfaces de persistência. | Não depende da interface gráfica nem de controladores HTTP. |
| View | Interfaces web e móvel, formulários, mapas e apresentação de estados. | Não acessa diretamente banco de dados nem decide regras de negócio. |
| Controller | Recebe solicitações, valida formato, autenticação e autorização, delega ao Model e devolve resposta. | Não contém regras de negócio nem consultas SQL diretas. |
| Infraestrutura | Persistência, adaptadores Pix, mapas, notificações e observabilidade. | Implementa interfaces do domínio; detalhes externos não contaminam o Model. |

![Arquitetura MVC](diagramas/mvc.png)

Quando um usuário realiza uma operação na View, esta encaminha uma solicitação HTTPS ao Controller, que verifica a identidade do usuário e os dados recebidos e invoca a função do Model correspondente à operação desejada, cabendo ao Model verificar se a operação respeita as regras de negócio previamente estabelecidas, como as referentes ao raio de cobertura, à disponibilidade e à alteração do status dos pedidos; o resultado é então retornado à View pelo Controller. A persistência dos dados e a comunicação com serviços externos são de responsabilidade da infraestrutura. Dito isso, é importante ressaltar que uma mesma confirmação de Pix não pode ser processada duas vezes.
