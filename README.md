CENTRO UNIVERSITÁRIO LA SALLE DO RIO DE JANEIRO - Unilasalle - RJ
Sistemas de Informação
Sistema Web para Gerenciamento de Resgate e Adoção de Animais – Arca Proteção
Integrantes do Grupo:
Caique Menezes Graupera Lourenço – 10223050
Diego Carvalho Bahia – 1023247
Eduardo de Lima Varandas Nogueira – 1022838
Lucas Deano – 1022872





Niterói
Junho/2026

Resumo
O presente trabalho apresenta o desenvolvimento de um sistema web para a instituição Arca Proteção, organização voltada ao resgate, tratamento e adoção de animais em situação de abandono. Atualmente, a instituição realiza o gerenciamento das informações de forma manual, utilizando planilhas e documentos físicos, o que dificulta a organização dos dados e o acompanhamento dos processos internos.
O sistema proposto tem como objetivo centralizar as informações relacionadas aos animais resgatados, tratamentos veterinários, adotantes e histórico de adoções, além de disponibilizar uma página pública para divulgação dos animais disponíveis para adoção.
A aplicação será desenvolvida utilizando o framework Django, com banco de dados SQLite, oferecendo uma solução organizada, segura e de fácil manutenção. Espera-se que o sistema contribua para melhorar a gestão da instituição, reduzir falhas no armazenamento de informações e facilitar o processo de adoção responsável.
Palavras-chave: sistema web, adoção de animais, Django, gerenciamento, instituição de proteção animal.







Abstract
This paper presents the development of a web system for Arca Proteção, an organization focused on the rescue, treatment, and adoption of abandoned animals. Currently, the institution manages information manually through spreadsheets and physical documents, which makes data organization and internal process monitoring difficult.
The proposed system aims to centralize information related to rescued animals, veterinary treatments, adopters, and adoption history, in addition to providing a public page to display animals available for adoption.
The application will be developed using the Django framework and SQLite database, providing an organized, secure, and easy-to-maintain solution. The system is expected to improve the institution’s management, reduce information storage failures, and facilitate the responsible adoption process.
Keywords: web system, animal adoption, Django, management, animal protection institution.








Sumário
1.0 INTRODUÇÃO:
 1.1 Objetivo
 1.1.1 Objetivo Geral
 1.1.2 Objetivos Específicos
 1.2 Justificativa
 1.3 Organização do Trabalho
2.0 LEVANTAMENTO DE REQUISITOS:
 2.1 Contextualização
 2.2 Descrição
 2.2.1 Requisitos Funcionais
 2.2.2 Requisitos Não Funcionais
 2.3 Arquitetura
 2.4 Cronograma
3.0 ANÁLISE:
 3.1 Diagrama de Classe Conceitual
 3.2 Diagrama de Caso de Uso
 3.3 Lista de Eventos
 3.3.1 Descrição de Caso de Uso
 3.3.1.2 Caso de Uso: Cadastro de Animal
 3.3.1.3 Descrição
 3.3.1.4 Pré-condições
4.0 ANEXOS:
 4.1 Print das Telas
 4.2 Evidências
Lista de Ilustrações
Figura 1 – Arquitetura do Sistema
Figura 2 – Diagrama de Caso de Uso
Figura 3 – Diagrama de Classe Conceitual
Figura 4 – Tela de Cadastro de Animais
Figura 5 – Tela de Animais Disponíveis para Adoção

Lista de Abreviaturas e Siglas
RF – Requisito Funcional
RNF – Requisito Não Funcional
SQL – Structured Query Language
HTML – HyperText Markup Language
CSS – Cascading Style Sheets
1.0 INTRODUÇÃO:
A tecnologia tem se tornado uma importante ferramenta de apoio para organizações que necessitam gerenciar informações de maneira eficiente e segura. Instituições voltadas à proteção animal frequentemente enfrentam dificuldades relacionadas ao armazenamento e controle de dados, principalmente quando utilizam métodos manuais de organização.
A Arca Proteção atua no resgate e tratamento de animais abandonados, promovendo posteriormente a adoção responsável desses animais. Atualmente, a instituição realiza seus registros utilizando planilhas e documentos físicos, o que dificulta o acompanhamento das informações e reduz a eficiência dos processos internos.
Diante desse cenário, surge a necessidade de desenvolver um sistema web capaz de centralizar e organizar todas as informações da instituição, facilitando o gerenciamento dos animais resgatados, tratamentos veterinários e processos de adoção.
1.1 Objetivo
1.1.1 Objetivo Geral
Desenvolver um sistema web para auxiliar a instituição Arca Proteção no gerenciamento de animais resgatados, tratamentos veterinários e processos de adoção.
1.1.2 Objetivos Específicos
Permitir o cadastro de animais resgatados;
Registrar informações detalhadas sobre os animais;
Controlar tratamentos veterinários;
Gerenciar o cadastro de adotantes;
Registrar processos de adoção;
Disponibilizar uma página pública para divulgação dos animais;
Centralizar as informações da instituição em um único sistema.
1.2 Justificativa
A ausência de um sistema informatizado dificulta a organização das informações da instituição, aumentando o risco de perda de dados e tornando os processos mais lentos. Além disso, a falta de divulgação digital reduz as chances de adoção dos animais resgatados.
O desenvolvimento do sistema permitirá melhorar o controle das informações, agilizar os processos internos e ampliar a divulgação dos animais disponíveis para adoção.
1.3 Organização do Trabalho
O presente trabalho está dividido em quatro capítulos principais. O primeiro apresenta a introdução, objetivos e justificativa do projeto. O segundo aborda o levantamento de requisitos e a arquitetura do sistema. O terceiro apresenta a análise do sistema, incluindo diagramas e casos de uso. Por fim, o quarto capítulo reúne anexos e evidências do desenvolvimento.
2.0 LEVANTAMENTO DE REQUISITOS:
2.1 Contextualização
A instituição Arca Proteção realiza o resgate e tratamento de animais em situação de abandono, oferecendo suporte veterinário e promovendo adoções responsáveis.
Atualmente, a gestão das informações é feita manualmente, utilizando planilhas e documentos físicos, dificultando a organização e o acompanhamento dos processos.
Dessa forma, identificou-se a necessidade de desenvolver uma plataforma digital que permita centralizar as informações da instituição e melhorar o gerenciamento das atividades.
2.2 Descrição
O sistema será desenvolvido como uma aplicação web utilizando Django e SQLite.
A aplicação permitirá:
Cadastro de animais resgatados;
Controle de tratamentos veterinários;
Cadastro de adotantes;
Registro de adoções;
Divulgação de animais disponíveis para adoção.
2.2.1 Requisitos Funcionais
RF01 – Permitir cadastro de animais resgatados;
RF02 – Registrar informações detalhadas dos animais;
RF03 – Registrar data e local do resgate;
RF04 – Registrar tratamentos veterinários;
RF05 – Alterar status do animal;
RF06 – Permitir cadastro de adotantes;
RF07 – Registrar processos de adoção;
RF08 – Consultar histórico de adoções;
RF09 – Disponibilizar página pública para adoção;
RF10 – Editar informações cadastradas;
RF11 – Excluir registros.
2.2.2 Requisitos Não Funcionais
RNF01 – O sistema deverá possuir interface simples e intuitiva;
RNF02 – O sistema deverá armazenar os dados com segurança;
RNF03 – O sistema deverá funcionar em navegadores modernos;
RNF04 – O sistema deverá apresentar boa performance nas consultas;
RNF05 – O sistema deverá possuir fácil manutenção.
2.3 Arquitetura
O sistema será baseado em arquitetura cliente-servidor dividida em três camadas:
Camada de Apresentação
Responsável pela interface com o usuário.
Tecnologias utilizadas:
HTML
CSS
JavaScript

Camada de Aplicação
Responsável pela lógica do sistema.
Tecnologia utilizada:
Django
Camada de Dados
Responsável pelo armazenamento das informações.
Tecnologia utilizada:
SQLite
2.4 Cronograma
Etapa
Atividade
Período
1
Levantamento de requisitos
Semana 1
2
Modelagem do banco de dados
Semana 2
3
Configuração do ambiente Django
Semana 3
4
Desenvolvimento das funcionalidades principais
Semana 4
5
Implementação do banco de dados SQLite
Semana 5
6
Desenvolvimento da interface do sistema
Semana 6
7
Testes e correção de erros
Semana 7
8
Finalização e documentação do projeto
Semana 8




3.0 ANÁLISE:
3.1 Diagrama de Classe Conceitual
O sistema possuirá as seguintes entidades principais:
Animal
Tratamento
Adotante
Adoção
Os relacionamentos entre essas entidades permitirão controlar o histórico completo dos animais desde o momento do resgate até a adoção.
3.2 Diagrama de Caso de Uso
Os principais casos de uso identificados foram:
Cadastrar animal;
Atualizar informações;
Registrar tratamento veterinário;
Cadastrar adotante;
Registrar adoção;
Consultar histórico de adoções;
Visualizar animais disponíveis para adoção.





3.3 Lista de Eventos

Evento
Descrição
Cadastro de Animal


Registro de novo animal resgatado
Atualização de Status
Alteração da situação do animal
Cadastro de Tratamento
Registro de atendimento veterinário
Cadastro de Adotante
Registro de pessoa interessada
Processo de Adoção
Finalização da adoção


3.3.1 Descrição de Caso de Uso
3.3.1.2 Caso de Uso: Cadastro de Animal
3.3.1.3 Descrição
O responsável pela instituição realiza o cadastro de um novo animal resgatado no sistema, preenchendo informações como nome, espécie, raça, idade aproximada, sexo, estado de saúde, local e data do resgate.
3.3.1.4 Pré-condições
O usuário deve estar autenticado no sistema;
O sistema deve estar conectado ao banco de dados.


4.0 ANEXOS:
4.1 Print das Telas
Tela inicial do sistema;
Tela de cadastro de animais;
Tela de tratamentos veterinários;
Tela de adoção;
Página pública de adoção.
4.2 Evidências
Prints do funcionamento do sistema;
Testes realizados;
Registro de cadastro de animais;
Evidências de consultas e adoções cadastradas.

