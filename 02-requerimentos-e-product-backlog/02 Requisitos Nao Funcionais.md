# 2.2 REQUISITOS NÃO FUNCIONAIS

Além das funções previamente estabelecidas, precisamos definir as condições referentes à qualidade e ao funcionamento do sistema, nomeadas requisitos não funcionais; seguem os requisitos definidos para o nosso sistema:

## 2.2.1 DESEMPENHO

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RNF-001 | Tempo de resposta | O tempo de resposta do sistema deve ser de até 2 segundos para, no mínimo, 95% das solicitações realizadas. |
| RNF-002 | Capacidade | O sistema deve suportar a utilização simultânea por, pelo menos, 5.000 usuários. |
| RNF-003 | Atualização de pedidos | Quando ocorrer uma alteração no status de um pedido, esta deve ser disponibilizada aos usuários em até 5 segundos. |
| RNF-024 | Tempo médio de entrega | Considerando os pedidos realizados dentro do raio de cobertura de 5 km, a média do tempo decorrido entre a confirmação dos pedidos e a conclusão das respectivas entregas deve ser inferior a 35 minutos. |

### 2.2.1.1 SEGURANÇA

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RNF-004 | Criptografia | A comunicação entre cliente e servidor deve ser realizada utilizando-se de TLS (HTTPS), de modo a proteger os dados em trânsito. |
| RNF-005 | Armazenamento de senhas | Para o armazenamento das senhas, devem ser utilizados algoritmos seguros de hash com salt. |
| RNF-006 | Autorização | O acesso aos recursos do sistema deve respeitar as permissões referentes ao perfil do usuário. |
| RNF-007 | Privacidade | O tratamento dos dados pessoais deve respeitar o que é estabelecido pela Lei Geral de Proteção de Dados (LGPD). |
| RNF-008 | Segurança de pagamentos | Dados sensíveis referentes a cartões bancários não devem ser armazenados diretamente pelo sistema. |

### 2.2.1.2 USABILIDADE E ACESSIBILIDADE

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RNF-009 | Responsividade | A interface do sistema deve se adaptar tanto a dispositivos móveis e tablets quanto a computadores. |
| RNF-010 | Acessibilidade | A interface deve respeitar os critérios de acessibilidade estabelecidos pela WCAG 2.2, nível AA. |
| RNF-011 | Consistência visual | Deve-se manter uma consistência entre as diversas interfaces do sistema no que diz respeito à navegação, à terminologia e aos componentes visuais. |
| RNF-012 | Idioma | O idioma utilizado na interface deve ser o português brasileiro. |

### 2.2.1.3 DISPONIBILIDADE E CONFIABILIDADE

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RNF-013 | Disponibilidade | A disponibilidade mensal do sistema deve ser de, no mínimo, 99,5%. |
| RNF-014 | Backup | Os dados do sistema devem passar pelo processo de backup de forma automática a cada 24 horas. |
| RNF-015 | Recuperação | Caso ocorra uma falha crítica, deve ser possível restabelecer as operações do sistema em até 4 horas. |
| RNF-016 | Integridade | Mesmo quando realizadas operações de forma simultânea, o sistema deve preservar a consistência dos dados. |

### 2.2.1.4 MANUTENIBILIDADE

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RNF-017 | Modularidade | Os componentes do sistema devem possuir responsabilidades bem delimitadas, de modo a manter um baixo acoplamento entre eles. |
| RNF-018 | Arquitetura | O padrão arquitetural a ser utilizado no sistema deve ser o MVC. |
| RNF-019 | Documentação | A documentação técnica referente aos componentes do sistema e às interfaces destes deve ser mantida atualizada. |
| RNF-020 | Versionamento | Tanto o código-fonte quanto a documentação do sistema devem ser versionados através do Git. |

### 2.2.1.5 COMPATIBILIDADE E ESCALABILIDADE

| **ID** | **Requisito** | **Descrição** |
| --- | --- | --- |
| RNF-021 | Compatibilidade | O sistema deve ser compatível com as duas versões estáveis mais recentes de cada um dos seguintes navegadores: Chrome, Firefox, Edge e Safari. |
| RNF-022 | Escalabilidade | Conforme aumente a demanda pelo sistema, deve ser possível ampliar a capacidade de processamento e armazenamento da infraestrutura. |
| RNF-023 | Interoperabilidade | Para a comunicação do sistema com serviços externos, devem ser utilizadas interfaces documentadas, bem como protocolos padronizados. |
