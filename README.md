# 🦷 Sistema de Gestão Odontológica
**Serratec – Centro de Educação Profissional**  
**Disciplina:** Banco de Dados  
**Semestre:** 2025/2  
**Criado por: Alexandre Lício, Amanda Lisbôa, Kayo Rentes, Lucas Gomes e Simone Martins.**

## Descrição do Projeto

Este projeto tem como objetivo desenvolver um banco de dados para uma clínica odontológica.
O sistema contempla pacientes, dentistas, atendentes, consultas, procedimentos odontológicos e horários de atendimento, permitindo o gerenciamento de consultas, histórico de atendimentos e controle administrativo.
O trabalho foi realizado em grupo, seguindo as instruções do professor, com a implementação de tabelas, relacionamentos, inserção de dados, atualizações, exclusões, índices, views e consultas SQL.

## Tecnologias Utilizadas

* **PostgreSQL** (comandos DDL, DML, DQL)
* **DBeaver** para gerenciamento do banco de dados
* **Git/GitHub** para versionamento e colaboração em equipe

## Estrutura do Banco de Dados
### Tabelas Criadas
* **Pacientes →** dados pessoais e de contato dos pacientes.
* **Dentistas →** informações dos dentistas e suas especialidades.
* **Consultas →** agenda de consultas, status e prescrições.
* **Procedimentos_odontologicos →** lista de procedimentos disponíveis na clínica.
* **Consultas_procedimentos →** relacionamento entre consultas e procedimentos realizados.
* **Atendentes →** cadastro dos atendentes do consultório.
* **Horarios →** horários de atendimento disponíveis para cada dentista.

### Relacionamentos
* Um paciente pode ter várias consultas.
* Um dentista pode atender várias consultas.
* Uma consulta pode conter vários procedimentos.
* Os horários estão vinculados diretamente a um dentista.

## Funcionalidades Implementadas
### Inserções
* Dados fictícios para pacientes, dentistas, atendentes, procedimentos odontológicos, consultas e horários.
    * **Exemplos:** heróis da Marvel como pacientes (Tony Stark, Steve Rogers etc.) e dentistas fictícios.

### Atualizações (UPDATE)
* Atualização de telefone e endereço de pacientes.
* Alteração de descrição de consultas.
* Cancelamento de consultas com base em regras de negócio. 

### Exclusões (DELETE)
* Remoção de consultas canceladas.
* Remoção de horários de domingo.
* Exclusão de atendentes específicos.

### Índices (INDEX)
* Índice em consultas por dentista, paciente e data.
* Índice em consultas_procedimentos por procedimento.

### Views
* `lista_consultas` → lista de consultas com paciente, dentista e procedimentos, ordenadas por data.

### Consultas Analíticas

*Quantidade de consultas por especialidade.
*Quantidade de consultas por dentista (ordem decrescente).
*Pacientes com maior número de consultas.
*Cálculo da média de consultas por dentista

### Integrantes e Responsabilidades

* **Amanda →** Consultas SQL analíticas, cancelamento de consultas, documentação (README).
* **Kayo →** Criação das tabelas, quantidade de consultas por dentista, exclusão de atendentes. e criou  modelo Lógico
* **Lucas →** Inserts de procedimentos, updates em pacientes, consultas e criou o modelo Conceitual.
* **Simone →** Inserts em dentistas e atendentes, índices, exclusão de horários, média de consultas por dentista.
* **Alexandre →** Inserts em pacientes e consultas, exclusão de consultas canceladas.

## Como Executar

1. Clone este repositório:

   ```bash
   https://github.com/AmandaLisboa-Ramos/odonto_sys
   ```
2. Abra o projeto no **DBeaver** ou em outro cliente PostgreSQL.
3. Execute os scripts SQL de criação das tabelas.
4. Execute os scripts de inserção de dados.
5. Utilize os comandos de consulta, atualização e relatórios conforme documentado.

## Modelos do Banco de Dados

### Modelo Conceitual
![Modelo Conceitual](./Modelos_Conceitual_e_Logico/modelo_logico.png)

### Modelo Lógico
![Modelo Lógico](./Modelos_Conceitual_e_Logico/modelo_logico.png)


## Conclusão

O projeto atendeu aos requisitos propostos, implementando um sistema de gerenciamento de clínica odontológica com tabelas relacionadas, inserções de dados, atualizações, exclusões, relatórios e views. O trabalho em equipe foi essencial para a conclusão do projeto, unindo conhecimentos técnicos e colaboração para alcançar o resultado final.
