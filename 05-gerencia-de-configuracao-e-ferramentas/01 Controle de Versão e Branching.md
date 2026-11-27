# 5.1 CONTROLE DE VERSÃO E BRANCHING

O repositório do BairroDelivery no GitHub é dividido em pastas referentes às diversas etapas do projeto. Para o controle de versão, será utilizada uma branch nomeada main, que representa a versão estável do sistema, enquanto serão criadas outras branches para a realização das atividades, sendo que, posterior à revisão, estas serão integradas através de pull requests, sendo necessário configurar a proteção da branch main no GitHub.

- A branch main representa a versão estável e revisada do sistema, enquanto feature/PB-xxx-descricao será utilizada para o desenvolvimento de funcionalidades, fix/PB-xxx-descricao para correções e docs/descricao para a documentação;
- Os commits devem ser pequenos e descrever o que foi alterado, conforme os exemplos: feat: implementar cadastro (PB-001), fix: validar raio de entrega (PB-007) e docs: atualizar arquitetura;
- No pull request, deve-se informar o que foi alterado, o item do Product Backlog associado e as evidências dos testes realizados, sendo necessário revisar as alterações e resolver os conflitos antes do merge;
- Para identificar a primeira versão homologada, utiliza-se a tag v1.0.0. É importante ressaltar que não devem ser armazenados no repositório credenciais, tokens ou dados pessoais.
