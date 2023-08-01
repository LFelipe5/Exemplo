# CDU002 Listar Turmas. 

- **Ator principal**: Bolsista.
- **Atores secundários**: CODESP 
- **Resumo**: Um bolsista consegue acessar a funcionalidade de listar turmas para exibir todas as turmas já cadastradas
- **Pré-condição**: Passar pela autenticação da API do Suap.
- **Pós-Condição**: O sistema deve mostrar uma lista com as turmas criadas.

## Fluxo Principal
| Ações do ator | Ações do sistema |
| :-----------------: | :-----------------: | 
| 1 - Bolsista acessa o sistema e inicializa a autenticação de credenciais |  Sistema se comunica com a API externa do SUAP e em seguida, redireciona para o dashboard | 
| 2 - O bolsista clica na opção listar turmas no dashboard |  O sistema redireciona para a página de listar turmas, em seguida | 
| 3 - O bolsista acessa todas as turmas disponíveis | O sistema consegue recuperar todas as turmas por meio do API do backend | 
 

## Fluxo de Exceção - Erro no banco de dados
| Ações do ator | Ações do sistema |
| :-----------------: | :-----------------: | 
| 1 - Bolsista acessa o sistema e inicializa a autenticação de credenciais | Sistema se comunica com a API externa do SUAP e em seguida, redireciona para o dashboard | 
| 2 - O usuário não consegue acessar as funcionalidades e ver recuperar os dados | Por conta da falha com a conexão do banco de dados, o sistema perde a capacidade de ter o acesso aos dados já registrados e assim gerando uma mensagem de erro do tipo 404 | 
