# 🌎 CRUD de Países - C# & SQL Server

Este é um mini sistema de Gerenciamento de Países desenvolvido em **C# (Windows Forms)** utilizando o **SQL Server**. 

## 🚀 Funcionalidades

- **Cadastrar:** Adiciona novos países (Código, Nome, População e Área).
- **Consultar:** Busca informações detalhadas através do código do país.
- **Atualizar:** Permite a edição de dados de registros já existentes.
- **Excluir:** Remove registros do banco de dados com confirmação de segurança.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** C# (.NET Framework)
* **Interface:** Windows Forms (WinForms)
* **Banco de Dados:** SQL Server

---

## 📋 Pré-requisitos e Instalação

O projeto foi configurado para rodar em qualquer máquina, basta seguir estes dois passos:

### 1. Preparar o Banco de Dados
Abra o seu **SQL Server Management Studio (SSMS)** e execute o script abaixo para criar a estrutura necessária:

```sql
CREATE DATABASE crudpaises;


USE crudpaises;


CREATE TABLE paises (
    id_pais int not null primary key IDENTITY(1,1),
    cod_pais int,
    nome varchar(50),
    populacao int,
    area_total decimal(18, 2)
);

```
Clone este repositório.

Abra o arquivo .sln no Visual Studio.

Inserir: Preencha os dados e clique em cadastrar.

Pesquisar: Digite o código no campo de busca para carregar os dados nos campos principais.

Atualizar/Excluir: Após carregar um país pela busca, você pode editar seus dados ou removê-lo do sistema.




