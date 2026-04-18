# Criar-o-diagrama-dimensional-star-schema-com-base-no-diagrama-relacional-disponibilizado

Desafio de Modelagem Dimensional - Star Schema (Foco: Professor)
Este repositório contém a resolução do desafio de modelagem de dados para um sistema acadêmico. O objetivo principal foi transformar um diagrama relacional em um esquema em estrela (Star Schema) voltado para a análise de dados dos professores.
🎯 Objetivo do Projeto
Criar um modelo dimensional que permita analisar a atuação dos professores, os cursos ministrados e os departamentos aos quais estão vinculados, facilitando a tomada de decisão e a geração de relatórios gerenciais.
Nota: Conforme os requisitos do desafio, dados relativos aos alunos foram desconsiderados nesta modelagem.
🛠️ Tecnologias Utilizadas
•	Modelagem Dimensional: Star Schema.
•	Ferramenta de Design: [Inserir o nome da ferramenta que você usou, ex: MySQL Workbench, DBDesigner, Draw.io].
🏗️ Estrutura do Modelo (Star Schema)
A modelagem foi dividida entre uma tabela central de fatos e tabelas de dimensão que fornecem o contexto:
1. Tabela Fato: Fato_Professor
Armazena as métricas e as chaves estrangeiras que conectam o contexto da análise. Contém informações sobre a carga horária, quantidade de disciplinas e associações principais.
2. Tabelas de Dimensão
•	Dim_Professor: Atributos detalhados do docente (nome, especialização, titulação).
•	Dim_Curso: Informações sobre os cursos oferecidos (nome do curso, modalidade, área de conhecimento).
•	Dim_Departamento: Detalhes sobre a unidade administrativa (nome do departamento, centro/campus).
•	Dim_Disciplina: Dados das matérias ministradas (nome, carga horária teórica/prática).
•	Dim_Data: Tabela de tempo criada para suprir a necessidade de análise temporal (granularidade: dia, mês, ano, semestre e trimestre).
📅 Modelagem da Dimensão Data
Como o modelo relacional original era limitado em datas, foram simulados campos para permitir análises como:
•	Data de oferta das disciplinas.
•	Data de início e conclusão de períodos letivos.
•	Histórico de oferta de cursos.
________________________________________
