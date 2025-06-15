# 🔧 Esquema-conceitual-para-o-contexto-de-oficina-mecanica

Este repositório contém o **modelo lógico de banco de dados** desenvolvido com base no desafio da DIO: **"Refinando um Projeto Conceitual de Banco de Dados - Oficina Mecânica"**.

## 📚 Descrição do Projeto

O projeto tem como objetivo modelar um sistema de controle e gerenciamento de **ordens de serviço (OS)** para uma **oficina mecânica**, a partir de uma narrativa fornecida no desafio. O modelo contempla todas as entidades, relacionamentos e atributos essenciais para representar o funcionamento do sistema da oficina.

## 🧱 Entidades Principais

- **Cliente**: dados cadastrais dos clientes.
- **Veículo**: informações sobre os veículos levados à oficina.
- **Mecânico**: profissionais da oficina, com suas especialidades.
- **Equipe**: agrupamento de mecânicos para atendimento de OS.
- **Ordem de Serviço (OS)**: registro das manutenções ou revisões solicitadas.
- **Serviço**: tipos de serviços prestados pela oficina.
- **Peça**: peças utilizadas na manutenção dos veículos.

## 🔗 Relacionamentos Modelados

- Um **cliente** pode ter vários **veículos**.
- Cada **veículo** pode gerar várias **ordens de serviço**.
- Cada **OS** é atribuída a uma **equipe de mecânicos**.
- Uma **equipe** pode ter vários **mecânicos** (relacionamento N:N).
- Uma **OS** pode incluir vários **serviços** e utilizar várias **peças** (ambos com relacionamento N:N).

## 🛠️ Ferramentas Utilizadas

- [MySQL Workbench](https://www.mysql.com/products/workbench/): ferramenta utilizada para criar o modelo lógico (arquivo `.mwb`).

## 📝 Observações

Algumas decisões foram tomadas com base no contexto do desafio, como:

- Criação da entidade **Equipe** para organizar os mecânicos.
- Uso de tabelas associativas para relacionamentos N:N, como:
  - **equipe_mecanico**
  - **os_servico**
  - **os_peca**

Essas decisões visam tornar o modelo mais próximo de uma aplicação real.

## 🚀 Objetivo do Projeto

- Consolidar o aprendizado em modelagem de dados.
- Representar um sistema realista de forma lógica e estruturada.
- Preparar o modelo para futura implementação em um SGBD relacional.

---

📚 Projeto realizado como parte do curso na [DIO](https://www.dio.me/): *Refinando um Projeto Conceitual de Banco de Dados - Oficina Mecânica*.





