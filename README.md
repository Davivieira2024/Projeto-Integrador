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

| Id     | Descrição | Prioridade     | 
| ----------- | ----------- |-----------| 
| RF001   | O sistema deve fornecer um formulário para cadastro para pessoa física  |Essecial|
| RF002   | O sistema de fornecer um formulário para cadastro para pessoa jurídica  |Essecial|
| RF003   | O sistema deve fornecer um formulário para cadastro para professores Pf  |Essecial|
| RF004   | O sistema deve fornecer um formulário para cadastro para professores PJ  |Essecial|
| RF005   | O sistema deve fornecer um formulário para cadastro de fornecedores Pf  |Essecial|
| RF006   | O sistema deve fornecer um formulário para cadastro de fornecedores PJ  |Essecial|
| RF007   | O Sistema deve fornecer um formulário para cadastro de alunos           |Essecial|
| RF008   | O sistema deve disponibilizar um formulário para cadastro de departamentos |Importante|
| RF009   | O sistema deve fornecer um formulário para cadastro de produtos  |Importante|
| RF010   | O sistema deve fornecer um formulário para cadastro de departamentos  |Importante|
| RF011   | O sistema deve fornecer um formulário para cadastro de endereços  |Importante|

### Requisitos não funcionais do sistema.
| Id     | Descrição | Prioridade     | 
| ----------- | ----------- |-----------| 
| RNF001   | O sistema deve fornecer um formulário para cadastro para pessoa física  |Essecial|
| RNF002   | O sistema de fornecer um formulário para cadastro para pessoa jurídica  |Essecial|
| RNF003   | O sistema deve fornecer um formulário para cadastro para professores Pf  |Essecial|
| RNF004   | O sistema deve fornecer um formulário para cadastro para professores PJ  |Essecial|
| RNF005   | O sistema deve fornecer um formulário para cadastro de fornecedores Pf  |Essecial|
| RNF006   | O sistema deve fornecer um formulário para cadastro de fornecedores PJ  |Essecial|
| RNF007   | O Sistema deve fornecer um formulário para cadastro de alunos           |Essecial|
| RNF008   | O sistema deve disponibilizar um formulário para cadastro de departamentos |Importante|
| RNF009   | O sistema deve fornecer um formulário para cadastro de produtos  |Importante|
| RNF010   | O sistema deve fornecer um formulário para cadastro de departamentos  |Importante|
| RNF011   | O sistema deve fornecer um formulário para cadastro de endereços  |Importante|


