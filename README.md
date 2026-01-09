# 🛠️ Sistema de Oficina Mecânica – Modelo Conceitual

Este repositório contém o **modelo conceitual de banco de dados** para um sistema de gerenciamento de **oficina mecânica**, desenvolvido como parte de um desafio da **Formação SQL da DIO**.

O objetivo do projeto é representar, de forma estruturada, o fluxo completo de atendimento de veículos em uma oficina, desde a abertura da ordem de serviço até a entrega do veículo reparado.

---

## 📌 Visão Geral do Projeto

O modelo contempla as principais entidades e relacionamentos envolvidos no processo operacional de uma oficina mecânica, incluindo:

- Cadastro de veículos
- Abertura e fechamento de ordens de serviço
- Diagnósticos técnicos
- Revisões e execuções de serviços
- Controle de prazos, valores e pagamento
- Entrega do veículo ao cliente

O diagrama foi elaborado seguindo boas práticas de modelagem conceitual, com cardinalidades bem definidas e chaves primárias e estrangeiras identificadas.

---

## 🧩 Entidades Principais

### 🚗 Veículo
Armazena informações básicas do veículo atendido na oficina.
- Modelo
- Ano
- Quilometragem

### 📄 Ordem de Serviço (OS)
Representa o atendimento do veículo.
- OS Aberta
- OS Fechada
- Revisão
- Diagnóstico

### 🔍 Diagnóstico
Detalha a análise técnica realizada no veículo.
- Análise
- Valor do serviço
- Prazo
- Forma de pagamento

### 🔧 Revisão
Registra os serviços executados durante o reparo.
- Execução
- Prazo

### ✅ Veículo Reparado
Indica a finalização do serviço.
- Revisão de entrega
- Lavagem

### 📦 Veículo Entregue
Marca a conclusão do processo com a entrega ao cliente.

---

## 🔗 Relacionamentos

- Um **veículo** pode possuir várias **ordens de serviço**
- Uma **ordem de serviço** pode conter múltiplos **diagnósticos** e **revisões**
- Cada **veículo reparado** está associado a uma **OS fechada**
- O **veículo entregue** representa o encerramento do ciclo de atendimento

---

## 🎯 Objetivo Educacional

Este projeto tem como finalidade:
- Praticar modelagem conceitual de banco de dados
- Aplicar conceitos de cardinalidade e normalização
- Preparar a base para implementação futura em SQL

---

## 🧠 Tecnologias e Conceitos Utilizados

- Modelagem Conceitual
- Diagrama Entidade-Relacionamento (DER)
- Banco de Dados Relacional
- SQL (conceitual)

---

## 📚 Referência

Projeto desenvolvido como parte do laboratório:
**Construindo um Esquema Conceitual do Zero – DIO**

---

## 👤 Autor

**Leonardo**  
Estudante da Formação SQL – DIO

---

Sinta-se à vontade para contribuir, sugerir melhorias ou utilizar este modelo como base para seus próprios projetos!
