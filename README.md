# Projeto de Conexão com Banco de Dados - Teste de Caixa Branca

Este projeto tem como objetivo verificar e testar um código de conexão com banco de dados utilizando o padrão de teste **caixa branca**. O código foi analisado em busca de possíveis **erros** e **melhorias**, conforme o solicitado pelo exercício da disciplina.

## 💻 Descrição do Projeto

O código fornecido é responsável por realizar a conexão com um banco de dados MySQL e verificar as credenciais de um usuário (login e senha). Ele faz isso por meio de uma consulta SQL e exibe o nome do usuário caso as credenciais sejam válidas.

---

## 🛠️ **Erros Identificados e Melhorias Sugeridas**

Aqui estão os erros detectados durante o **Teste Estático** e as **melhorias** propostas:

### 1. **Driver MySQL Desatualizado**

- **Erro Identificado:**
  Na linha onde o driver de conexão é carregado:
  ```java
  Class.forName("com.mysql.Driver.Manager").newInstance();
