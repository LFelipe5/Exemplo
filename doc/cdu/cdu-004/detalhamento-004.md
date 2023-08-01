# CDU04. Exportar turma

- **Ator principal**: Bolsista.
- **Atores secundários**: Codesp.
- **Resumo**: O bolsista(Ou ocasionalmente alguém da codesp) acessa uma turma específica e gera um arquivo contendo todos as informações de uma turma.
- **Pré-condição**: É preciso ter uma turma criada no banco de dados
- **Pós-Condição**: O sistema irá gerar um arquivo para download contendo todas as informações esperadas.

## Fluxo Principal

| Ações do Ator                                                                       | Ações do sistema                                                                                              |
| :---------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------ |
| 1 - Bolsista acessa o sistema e realiza o login autenticado pelo SUAP                                                       | Com a autenticação do feita, o bolsista é direcionado para o dashboard                                                                                  |
| 2 - O bolsista acessa a funcionalidade  Listar turmas e escolhe a turma desejada                                             | O sistema redireciona para a página de listar turmas e depois, novamente, é redirecionada para a página de uma turma específica |
| 3 - Bolsista clica no botão de exportar turma                                 |  Sistema gera um arquivo contendo toda as informações de uma turma   |



