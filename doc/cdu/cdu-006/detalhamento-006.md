# CDU01. Matricular Aluno

- **Ator principal**: Bolsista.
- **Atores secundários**: Não há atores secundários.
- **Resumo**: O bolsista preenche as informações necessárias para a matricula de um aluno em uma turma específica seja feita.
- **Pré-condição**: A turma teria que ter vaga disponível para matricular aluno.
- **Pós-Condição**: O sistema irá criar no banco de dados um aluno em uma turma com as especificações definidas no momento da criação.

## Fluxo Principal

| Ações do Ator                                                                        | Ações do sistema                                                                                                               |
| :----------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| 1 - Bolsista acessa o sistema                                                        | Sistema exibe a tela inicial                                                                                                   |
| 2 - Bolsista seleciona a seção "listar turmas"                                       | Sistema encaminha o usuário para uma tela que irá listar todas as turmas já criadas, juntamente a um botão de matricular aluno |
| 3 - Bolsista clica no botão de matricular aluno                                      | Sistema encaminha o usuário para página de cadastro (formulário com informções de especificação do aluno)                      |
| 4 - Bolsista preenche o formulário (Nome Completo/Curso/Matrícula/Numero p/ Contato) | sistema exibe ao fim do formulário um botão de matricular aluno                                                                |
| 5 - bolsista clica no botão de matricular aluno                                      | Sistema exibe mensagem de que um novo aluno foi matriculado                                                                    |

## Fluxo Alternativo 01 - Listar

| Ações do ator                                   | Ações do sistema                                                                                                                           |
| :---------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- |
| 1 - Bolsista acessa o sistema                   | Sistema exibe a tela inicial                                                                                                               |
| 2 - Bolsista seleciona a seção " Listar turmas" | Sistema encaminha o usuário para uma tela que irá listar todas as turmas já criadas, juntamente a um botão de criar nova turma             |
| 3 - Bolsista Clica em uma turma específica      | Sistema encaminha o usuário para uma tela que irá listar os dados da turma específica junto com a listagem de todos os alunos matriculados |

## Fluxo Alternativo 02 - Editar

| Ações do ator                                  | Ações do sistema                                                                                                                           |
| :--------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- |
| 1 - Bolsista acessa o sistema                  | Sistema exibe a tela inicial                                                                                                               |
| 2 - Bolsista seleciona a seção "listar turmas" | Sistema encaminha o usuário para uma tela que irá listar todas as turmas já criadas, juntamente a um botão de criar nova turma             |
| 3 - Bolsista Clica em uma turma específica     | Sistema encaminha o usuário para uma tela que irá listar os dados da turma específica junto com a listagem de todos os alunos matriculados |

| 4 - Bolsista clica no botão de 3 pontos e depois em editar | Sistema reabre o formulário para editar os dados cadastrados anteriormente |
| 5 - Bolsista edita as informações que deseja | Sistema exibe ao fim do formulário um botão de salvar alterações |
| 6 - bolsista clica no botão salvar | Sistema exibe mensagem de que as edições foram salvas |

## Fluxo Alternativo 03 - Excluir

| Ações do ator                                  | Ações do sistema                                                                                                                           |
| :--------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- |
| 1 - Bolsista acessa o sistema                  | Sistema exibe a tela inicial                                                                                                               |
| 2 - Bolsista seleciona a seção "listar turmas" | Sistema encaminha o usuário para uma tela que irá listar todas as turmas já criadas, juntamente a um botão de criar nova turma             |
| 3 - Bolsista Clica em uma turma específica     | Sistema encaminha o usuário para uma tela que irá listar os dados da turma específica junto com a listagem de todos os alunos matriculados |

| 4 - Bolsista clica no botão de 3 pontos e depois em excluir turma | Sistema exibe a mensagem de de confirmação para excluir a turma e um botão de confirmar |
| 5 - Bolsista clica no botão de confirmar | Sistema exibe a mensagem de que a turma foi excluida |

## Fluxo Exceção 01 - Dados obrigatórios não preenchidos

| Ações do Ator                                                               | Ações do sistema                                                                                                                           |
| :-------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- |
| 1 - Bolsista acessa o sistema                                               | Sistema exibe a tela inicial                                                                                                               |
| 2 - Bolsista seleciona a seção "listar turmas"                              | Sistema encaminha o usuário para uma tela que irá listar todas as turmas já criadas, juntamente a um botão de criar nova turma             |
| 3 - Bolsista Clica em uma turma específica                                  | Sistema encaminha o usuário para uma tela que irá listar os dados da turma específica junto com a listagem de todos os alunos matriculados |
| 4 - Bolsista clica no botão de matricular aluno                             | Sistema encaminha o usuário para página de cadastro (formulário com informções de especificação da turma)                                  |
| 5 - Bolsista preenche o formulário (Nome Completo/Curso/Matricula/Telefone) | sistema exibe ao fim do formulário um botão de cadastrar turma                                                                             |
| 6 - bolsista clica no botão de cadastrar turma                              | Sistema exibe mensagem de que não foram preenchidos todos os campos obrigatórios                                                           |

## Fluxo Exceção 02 - Turma já está cheia

| Ações do Ator                                  | Ações do sistema                                                                                                                           |
| :--------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- |
| 1 - Bolsista acessa o sistema                  | Sistema exibe a tela inicial                                                                                                               |
| 2 - Bolsista seleciona a seção "listar turmas" | Sistema encaminha o usuário para uma tela que irá listar todas as turmas já criadas, juntamente a um botão de criar nova turma             |
| 3 - Bolsista Clica em uma turma específica     | Sistema encaminha o usuário para uma tela que irá listar os dados da turma específica junto com a listagem de todos os alunos matriculados |
| 4 - Bolsista Clica para matricular aluno       | sistema exibe uma mensagem que não existe vagas disponiveis para aquela turma                                                              |
