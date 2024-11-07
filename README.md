# Documento de Requisitos de Sistema
### Sistema de Gestão Para Universidade
### Versão 2.0 (Segunda Versão)
---
### Introdução.
Esse sistema é voltado para empresas que pretedem atuar no ramo educacional e  integrar todos os setores, desde a portaria até aplicações de avaliações em todas as unidades e para todos os cursos oferecidos. Disponibiliza também aos gestores informações relevantes que possa auxiliá-los na sua tomada de decisão. Pensado para atuar em plataforma web, permite aos usuários também para dispositivos móveis.
### Convenções e abreviações.
Sistema; Caso de Uso; Diagrama; Funcionais; Diagrama de Classe, Rf; Rnf; Pf; Pj.
### Identificação dos requisitos.
Serão utilizados como identificador dos requisitos a forma padão, RF001 para
requisitos funcionais e RNF001 para requisitos não funcionais, no formato incremental
e com descrições objetivas.
### Identificação dos requisitos.
Como padrão de prioridade vamos utilizar as seguintes notações, ***essencial, importante e desejável.*** Esses padrões servirão para identificar o grão de importância para cada requisito a ser desenvolvido. ***Essencial*** vamos utilizar para identificar que sem esses requisitos o sistema não pode ser instalado ou a etapa seguinte do sistema dependerá desses requisitos. Os requisitos ***importantes*** fazem parte do sistema, mas podem ser implementados nas etapas seguintes sem comprometer a instalação do sistema. Os requisitos ***desejáveis*** são aqueles que não comprometem a funcionalidade do sistema, podem ser instalados posteriormente e garantem qualidade, usabilidade e desempenho. Também será utilizado a forma padrão Pf para pessoa física e Pj para pessoa jurídica.
### Descrição geral do sistema.
O objetivo desse projeto é desenvolver um sistema para gestão educacional que
disponibilize os seguintes requisitos ao usuários. No ***cadastro para empresa pessoa jurídica*** o administrador dever
informar o ***cnpj, a inscrição estadual, a inscrição municipal e ramo de atividade*** da
empresa. Uma empresa do ramo educacional possui várias filiais e essas filiais devem
ser identificadas pelo ***código da unidade, descrições e o responsável pela unidade***.
Todos os ***departamentos*** também serão cadastrados e cada departamento terá o seu
***código de identificação, descrição do departamento e o responsável por cada
departamento***. As empresas poderão ter um ou mais ***telefones cadastrados*** e no seu
cadastro deverá conter, ***número do telefone, o código da cidade, código do país e o
titular da conta***. Cada ***unidade*** deve ter seu próprio ***endereço que serão cadastrados*** com os
seguintes dados: ***cep, rua, bairro, cidade, estado e país***. No ***cadastro para pessoa
física*** deve conter a ***cpf, rg, nome, sobrenome, email e data de nascimento***. Uma
pessoa pode ser um ***aluno, um professor, um fornecedor ou até mesmo um visitante***.
Caso essa pessoa seja um ***fornecedor o cadastrado*** deve conter os seguintes
atributos ***matrícula, data do cadastro, descrição dos produtos, valor do produto e
tipo do fornecedor***. Um fornecedor pode ser uma pessoais física e os seus atributos
deverão estar contidos como ***cadastro pessoa física***. O fornecedor para estar ativo deve
fornecer um ou mais produtos e esses ***produtos devem ser cadastrados*** e identificados
pelo ***código, descrição do produto, valor do produto, validade do produto
e nome do fabricante***. Uma pessoa também pode ser um aluno e, para o ***cadastro de
alunos*** será solicitado ***cpf, rg, nome, sobrenome, data de nascimento, sexo e data do
cadastro***. O sistema deve permitir que o aluno realize sua ***matrícula*** onde, cada aluno
deve informar o ***cpf, nome do curso, polo, endereço de e-mail, período e
turma***. Os seus dados pessoais devem estar previamente cadastrados no ***cadastro
pessoa física***. Durante o período de provas os alunos devem ***escolher as datas para suas avaliações***
previamente. Os alunos para ***agendar suas avaliações*** devem informar ***nome da matéria a data da
avaliação, horário e unidade***. A nota obtida deve ser igual ou
maior que a nota mínima para aprovação do curso. Um ***professor*** para fazer parte do quadro de colaboradores deve estar ***cadastrado*** e, para realização do ***cadastro de professores*** o sistema deve solicitar o ***número do cpf, data da realização do cadastro, unidade desejada e formação acadêmica***.

### Requisitos funcionais do sistema.

| Id          | Descrição   | Prioridade | 
| ----------- | ----------- |----------- | 
| RF001   | O sistema deve fornecer um formulário para cadastro de pessoa física  |Essecial|
| RF002   | O sistema deve fornecer um formulário para cadastro de pessoa jurídica  |Essecial|
| RF003   | O sistema deve fornecer um formulário para cadastro de professores Pf  |Essecial|
| RF004   | O sistema deve fornecer um formulário para cadastro de professores PJ  |Essecial|
| RF005   | O sistema deve fornecer um formulário para cadastro de fornecedores Pf  |Essecial|
| RF006   | O sistema deve fornecer um formulário para cadastro de fornecedores PJ  |Essecial|
| RF007   | O Sistema deve fornecer um formulário para cadastro de alunos           |Essecial|
| RF008   | O sistema deve disponibilizar um formulário para cadastro de departamentos |Importante|
| RF009   | O sistema deve fornecer um formulário para cadastro de produtos  |Importante|
| RF010   | O sistema deve fornecer um formulário para cadastro dos cursos  |Importante|
| RF011   | O sistema deve fornecer um formulário para cadastro das unidades  |Importante|
| RF012   | O sistema deve fornecer um formulário para cadastro das disciplinas |Importante|
| RF013   | O sistema deve fornecer um formulário para cadastro de matrículas |Importante|

### Requisitos não funcionais e de qualidade do sistema.
| Id     | Descrição | Categoria     | 
| ----------- | ----------- |-----------| 
| RNF001   | Caso o cadastro já tenha sido efetuado o sistema deve retornar a mensagem "Já existe um cadastro com esse cpf/cnpj"   |Confiabilidade|
| RNF002   | O Sistema não deve permitir acesso para usuário que não esteja logado  |Usuabilidade|
| RNF003   | O sistema não deve aceitar dados do tipo texto em campo numérico |Usuabilidade|
| RNF004   | Ao finalizar o cadastro o sistema deve retornar uma mensagem de confirmação  |Usuabilidade|
| RNF005   | Todos os dados trafegados deverão ser encriptados |Segurança|
| RNF006   | A interface deve ter navegação padronizada, assim como elementos visuais padronizados por guia de estilo  |Usuabilidade|
| RNF007   | O sistema deve ficar disponível 99,9% do tempo |Confiabilidade|
| RNF008   | O sistema deve ser capaz de lidar com altas demandas como em datas para matrículas e rematrículas |Escalabilidade|
| RNF009   | O sistema deve permitir que o usuário utilize a tecla ***ENTER*** para confimação dos dados  |Usuabilidade|
| RNF010   | O sistema deve permitir que o usuário utilize a tecla ***TAB*** para mudar de campo  |Usuabilidade|
| RNF011   | Após a confirmação dos dados cadastrados o cursor do mouse deve retornar para o campo inicial |Usuabilidade|
| RNF012   | Os campos CNPJ/CPF devem conter formatações e validações  |Segurança|

### Diagrama de caso de uso.
![](CasoDeUsoCadastroUsuarios.png)

### Diagrama de classe UML
![](DiagramaDeClasse.png)

### Descrições dos casos de uso.
| Nome do cenário: Cadastro de pessoa <br> Atores: <br> Pré-condição | [UC001] Cadastro <br> Cliente, Funcionario, Adm <br> Não está cadastrado |
| :---        |          ---: |
| ***Fluxo Principal***      |   |
| 1. O Sistema exibe a tela de cadastro pessoa física <br> 2. O usuário digita o número do Cpf <br> 3. O usuário digita o número do Rg <br> 4. O usuário digita o nome <br> 5. O usuário digita o sobrenome <br> 6. O usuário digita o e-mail <br> 7. O usuário digita a data de nascimento <br> 8. O usuário seleciona o sexo <br>9. O usuário confirma os dados informados <br> 10. O sistema salva os dados <br> 11. O sistema exibe a mensagem (fluxo alternativo 1) ||
| ***Fluxo Alternantivo 1 - Editar dados cadastrados***      | |
| 1. O Sistema exibe a tela de cadastro pessoa física <br> 2. O usuário digita o número do Cpf <br> 3. O sistema exibe a mensagem usuário já cadastrado <br> 4. O sistema carrega os dados do usuário na tela <br> 5. O sistema habilita os campos para edição <br> 6. O usuário confirma as alterações <br> 7. O sistema salva as alterações <br> 8. O sistema exibe a mensagem (Fluxo Alternativo – 1) |  |
| ***Fluxo Alternantivo 2 - Dados inválidos***      |   |
| 1. O Sistema exibe a tela de cadastro pessoa física <br> 2. O usuário digita o número do Cpf <br> 2. O sistema exibe a mensagem dados inválidos; <br> 3. O sistema retorna ao passo 2 do fluxo alternativo 1 <br>| And more |
| ***Pós condições***      |   |
| 1. O Sistema exibe os dados cadastrados com o número do registro <br> 2. O sistema envia os cadastro para impreessão | |

