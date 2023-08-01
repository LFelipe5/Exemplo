# Documento de Visão

## Histórico de Revisões

| Data                |  Versão             |          Descrição  |  Autores            |
| :-----------------: | :-----------------: | :-----------------: | :-----------------: |
| 22/11/2022 | 01 | Versão inicial |  Luiz Felipe, Valtércio, Mayra e Renato Berna |
| - | - | - |  - |


## 1. Objetivo do projeto

O objetivo do projeto SIGSPORTS, Sistema de Gestão da CODESP, é facilitar e propôr mais eficiência quanto às atividades comuns que são praticadas na secretaria da CODESP, como gerenciar matrículas e turmas nos esportes. Facilitar as localizações dos espaços de modalidades e da codesp para os alunos. Melhorar atividades realizadas por professores.   

## 2. Descrição do problema

|     |      |
| --- | --- |
| **Problema**            | Informações não claras o suficientes de espaços de modalidades e da secretaria da CODESP. Ausência de métodos mais eficientes de controle de fluxo de alunos. Ausência de melhorias quanto a execução de atividades da secretaria da CODESP. |
| **Afeta**               | Alunos, Bolsistas, Professores e Secretaria da CODESP. |  
| **Impacta**             | Alunos não possuem a informação da localização dos espaços das modalidades ou da secretaria da CODESP. Professores não possuem ferramentas  que facilitam o controle de fluxo de alunos. Secretaria da CODESP não possui ferramentas que facilitam ou modernize atividades realizadas com muita frequência. |
| **Solução**             | Um sistema Web que possa solucionar esses problemas e viabilizar as necessidades da secretaria da CODESP. | 

## 3. Descrição dos usuários 

| Nome                |  Descrição          |   Responsabilidade  |
| -----------------   | -----------------   | -----------------   |
| CODESP| Coordenação de esportes. | Pessoas que fazem atividades na secretaria da CODEP | Gerenciar professores, modalidade de esportes e alunos. Fazem e autorizam o registro, matrícula de alunos em modalidades desejadas. |
| Professor | Pessoas responsáveis pela execução das práticas das modalidades. | Registrar aulas dos esportes. Realiza frequência dos alunos. Decidem a quantidade de vagas nesta modalidade de esportes.  |
| Aluno | Pessoas que frequentam as aulas de modalidade de esportes. | Tem acesso a localização das aulas de esportes. Tem acesso aos conteúdos relacionados com as modalidades. |
| Bolsista | Pessoas que fazem atividades indicadas pela secretaria da codesp. | Salvar e solicitar cadastro de alunos que são associados com modalidades. Inserir e atualizar localização das aulas de esportes. |

## 4. Descrição do ambiente dos usuários

- O ambiente é composto pela CODESP, ginásio, campos de futebol, piscinas, salas de esportes e demais ambientes para realização das práticas esportivas.
- As tarefas realizadas vão desde reuniões, aulas e outras práticas esportivas.
- A quantidade de alunos varia de acordo com o preenchimento de vagas das modalidades esportivas.


## 5. Principais necessidades dos usuários

- Dificuldade no acesso a localização da codesp e dos locais de práticas. Será disponibilizado as orientações para encontrar os locais de aulas.
- Dificuldade no acesso aos horários. Será disponibilizado os horários no sistema.
- Preenchimentos das vagas nos esportes. Será cadastrado no sistema a quantidade de vagas disponíveis aos alunos interessados e preenchimento de vagas.


## 6. Alternativas concorrentes

Atualmente, não se encontra concorrrentes. A comparação é dada por medidas analógicas.

## 7. Visão geral do produto

- A solução é imprescindível para o funcionamento da coordenação de esportes, pois através dela, pode-se otimizar o controle de matrículas e fluxo das presenças dos alunos nos esportes do IFRN. 
- Com o auxílio do sistema, os alunos e professores terão uma maior facilidade de encontrar os horários e a localização das áreas de realização das práticas de esporte. 

## 8. Requisitos funcionais

| Código              |  Nome               |          Descrição  |  Prioridade         |
| :-----------------: | :-----------------: | :-----------------: | :-----------------: |
| F001 | Criar turma| A CODESP ou Bolsista podem criar uma nova turma com suas especificações | Máxima |
| F002 | Listar turma | A CODESP ou Bolsista podem listar as turmas existentes | Máxima |
| F003 | Gerenciar turma | A CODESP ou Bolsista podem gerenciar as turmas criadas, seja editando ou excluindo | Moderada |
| F004 | Exportar turma | A CODESP ou Bolsista podem exportar um arquivo com informações da turma em formato PDF | Opcional |
| F005 | Emitir Declaração | A CODESP ou Bolsista podem emitir a declaração com dados da matricula e situação do aluno, esse aquivo será baixado em formato PDF | Opcional| 
| F006 | Matricular aluno | A CODESP ou Bolsista podem matricular um novo aluno em uma turma de sua preferencia | Máxima |
| F007 | Emprestimo de local | A CODESP ou Bolsista porem registrar uma reserva de um local como ginásio, quadra, piscina etc | Opcional |
| F008 | Emprestimo de material | A CODESP ou Bolsista podem registrar emprestimo de material como bola, raquetes etc | Opcional |
| F009 | Gerenciar frequencia | Um professor define o controle de fluxo de alunos durante as práticas de modalidade. | Moderada |
| F010| Desligamento de um aluno | Um professor, opcionalmente, possui a opção de remover um aluno de uma devida modalidade. | Moderada | 
| F011| Visualizar modalidades | Um aluno pode visualizar na landingpage as modalidades ofertadas pela codesp | Opcional |
| F012 | Visualizar localização | Um aluno pode visualizar na landingpage os locais de realização das modalidades ofertadas pela codesp | Opcional |

| Código              |  Nome               |          Descrição  |  Categoria          |  Classificação      |
| :-----------------: | :-----------------: | :-----------------: | :-----------------: | :-----------------: |
| NF01 | Controle de acesso a Usuário | Somente Bolsistas relacionadas com a CODESP e professores conseguirão obter acesso à a algumas funcionalidades da aplicação. | Confidencialidade | Obrigatório |
| NF02 | Diversidade de dispositivos | O sistema deverá funcionar em dispositivos diferentes sem perda de qualidade  | Adaptabilidade | Desejável |
| NF03 | Volume de usuários | O sistema deverá permitir um maior volume de usuários sem degradação do desempenho durante a execução da aplicação | Performance | Desejável |
| NF04 | Curva de aprendizado | As interfaces possuem ícones que reforçam o entendimento das funcionalidades. Com uma interface fácil de entender e intuitiva, um usuário consegue acessar as funcionalidades sem dificuldade de compreensão  | Aprendizagem | Obrigatório |
| NF05 | Uso simultâneo | Um número indeterminado de usuários conseguem acessar as mesmas funcionalidades da aplicação sem ter problemas de desempenho durante sua execução | Performance | Desejável |
| NF06 | Sistema eficiente | O sistema possuirá uma média de segundos para execução das funcionalidades | Performance | Obrigatório |
| NF07 | Exportar arquivos| O sistema deverá estar disponível a qualquer momento para poder exportar arquivos que possuem informações relevantes relacionadas ao sistema | Disponibilidade | Obrigatório |
| NF08 | Funcionamento limitado | O sistema deverá estar funcionando de maneira limitada em caso de conexão falha ao banco de dados remoto | Tolerância ao erro | Obrigatório |

