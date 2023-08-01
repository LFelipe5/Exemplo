# CDU01. Emitir Declaração

- **Ator principal**: Bolsista.
- **Atores secundários**: Codesp.
- **Resumo**: O bolsista(Ou ocasionalmente alguém da codesp) acessa uma turma específica, depois escolhe um aluno para emitir uma declaração de estado de matrícula.
- **Pré-condição**: É preciso ter uma turma criada no banco de dados e também um aluno registrado na mesma.
- **Pós-Condição**: O sistema irá gerar um arquivo para download contendo as informações necessárias para emissão de matrícula.

## Fluxo Principal

| Ações do Ator                                                                       | Ações do sistema                                                                                              |
| :---------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------ |
| 1 - Bolsista acessa o sistema e realiza o login autenticado pelo SUAP                                                       | Com a autenticação do feita, o bolsista é direcionado para o dashboard                                                                                  |
| 2 - O bolsista acessa a funcionalidade  Listar turmas e escolhe a turma desejada                                             | O sistema redireciona para a página de listar turmas e depois, novamente, é redirecionada para a página de uma turma específica |
| 3 - Na página de turma, bolsista escolhe um aluno para clicar no botão de declaração |  Sistema gera um arquivo contendo toda as informações necessárias para emitir uma declaração   |



