# CDU001 Criar Turma. 

- **Ator principal**: Bolsista.
- **Atores secundários**: CODESP	 
- **Resumo**: Um bolsista(E ocasionalmente CODESP) acessa a funcionalidade de criar turma para registrar uma turma de esporte no sistema.
- **Pré-condição**: Passar pela autenticação da API do Suap.
- **Pós-Condição**: O sistema redicionará para dashboard mostrando todas as turmas registradas.

## Fluxo Principal
| Ações do ator | Ações do sistema |
| :-----------------: | :-----------------: | 
| 1 - Bolsista acessa o sistema e inicializa a autenticação de credenciais |  Sistema se comunica com a API externa do SUAP e em seguida, redireciona para o dashboard |
| 2 - O usuário clica na opção criar turma no dashboard |  Sistema exibe um formulário com as informações da turma para serem preenchidas |
| 3 - O bolsista acessa a opção da funcionalidade de criar Turma |  Sistema redireciona para a página de criação de turma |
| 4 - O bolsista preenche todas as informações necessárias para a criação de uma turma(Professor/Nome da turma/ Modalidade/ Categoria/ Turno/ Horários/ Dias/ Vagas) |  Com o preenchimento do formulário, o sistema irá concluir a ação e redirecionar para o dashboard |


## Fluxo de Exceção 
| Ações do ator | Ações do sistema |
| :-----------------: | :-----------------: | 
| 1 - Bolsista acessa o sistema e inicializa a autenticação de credenciais |  Sistema se comunica com a API externa do SUAP e em seguida, redireciona para o dashboard |
| 2 - O usuário não consegue acessar as funcionalidades e ver recuperar os dados | Por conta da falha com a conexão do banco de dados, o sistema perde a capacidade de ter o acesso aos dados já registrados e assim gerando uma mensagem de erro do tipo 404 |
