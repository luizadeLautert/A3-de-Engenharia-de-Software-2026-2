Documento desenvolvido para levantar e explicar os requisitos não funcionais esperados no sistema.
# Requisitos Não Funcionais — BairroDelivery
### Desempenho

| ID | Requisito | Descrição |
|---|---|---|
| RNF-001 | Tempo de resposta | O sistema deve responder a 95% das solicitações em até 2 segundos. |
| RNF-002 | Capacidade | O sistema deve suportar pelo menos 5000 usuários simultâneos. |
| RNF-003 | Atualização de pedidos | As alterações no status dos pedidos devem ser disponibilizadas aos usuários em até 5 segundos. |

### Segurança

| ID | Requisito | Descrição |
|---|---|---|
| RNF-004 | Criptografia | A comunicação entre o cliente e o servidor deve utilizar criptografia de ponta-a-ponta. |
| RNF-005 | Armazenamento de senhas | As senhas devem ser armazenadas utilizando algoritmos seguros de hash com salt. |
| RNF-006 | Autorização | O acesso aos recursos do sistema deve respeitar as permissões associadas ao perfil do usuário. |
| RNF-007 | Privacidade | O tratamento dos dados pessoais deve estar em conformidade com a Lei Geral de Proteção de Dados (LGPD). |
| RNF-008 | Segurança de pagamentos | O sistema não deve armazenar diretamente dados sensíveis de cartões bancários. |

### Usabilidade e Acessibilidade

| ID | Requisito | Descrição |
|---|---|---|
| RNF-009 | Responsividade | A interface deve adaptar-se a dispositivos móveis, tablets e computadores. |
| RNF-010 | Acessibilidade | A interface deve atender aos critérios de acessibilidade WCAG 2.2, nível AA. |
| RNF-011 | Consistência visual | As interfaces devem manter padrões consistentes de navegação, terminologia e componentes visuais. |
| RNF-012 | Idioma | A interface deve ser disponibilizada em português brasileiro. |

### Disponibilidade e Confiabilidade

| ID | Requisito | Descrição |
|---|---|---|
| RNF-013 | Disponibilidade | O sistema deve apresentar disponibilidade mensal mínima de 99,5%. |
| RNF-014 | Backup | Os dados do sistema devem ser submetidos a backups automáticos a cada 24 horas. |
| RNF-015 | Recuperação | O sistema deve permitir a recuperação das operações em até 4 horas após uma falha crítica. |
| RNF-016 | Integridade | O sistema deve preservar a consistência dos dados durante operações simultâneas. |

### Manutenibilidade

| ID | Requisito | Descrição |
|---|---|---|
| RNF-017 | Modularidade | O sistema deve possuir componentes com responsabilidades bem definidas e baixo acoplamento. |
| RNF-018 | Arquitetura | O sistema deve seguir o padrão arquitetural MVC. |
| RNF-019 | Documentação | Os componentes e interfaces do sistema devem possuir documentação técnica atualizada. |
| RNF-020 | Versionamento | O código-fonte e a documentação devem ser versionados utilizando Git. |

### Compatibilidade e Escalabilidade

| ID | Requisito | Descrição |
|---|---|---|
| RNF-021 | Compatibilidade | O sistema deve ser compatível com as duas versões estáveis mais recentes dos navegadores Chrome, Firefox, Edge e Safari. |
| RNF-022 | Escalabilidade | A infraestrutura deve permitir a ampliação da capacidade de processamento e armazenamento conforme o crescimento da demanda. |
| RNF-023 | Interoperabilidade | A comunicação com serviços externos deve utilizar interfaces documentadas e protocolos padronizados. |
