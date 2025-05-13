# 🗄️ Criando uma Instância de Banco de Dados no Azure

Este repositório foi criado como parte de um desafio prático na DIO, com o objetivo de documentar a criação de uma instância de banco de dados na plataforma Microsoft Azure.

## 🎯 Objetivo

Praticar a criação de uma instância gerenciada de banco de dados no Azure, compreendendo as etapas de configuração.

## 🧭 Passo a Passo

### 1. Acessar o portal Azure

Acesse [https://portal.azure.com](https://portal.azure.com) e entre na sua conta.

![image](https://github.com/user-attachments/assets/2f716468-875d-4184-b0cb-274bc3271726)

---

### 2. Criar um novo recurso de banco de dados

Clique em **"Criar um recurso"** → **"Banco de dados"** → Escolha a opção desejada (ex: Banco de Dados SQL).

### 3. Preencher as configurações básicas

- **Grupo de recursos**: crie um novo ou use um existente
- **Nome do servidor**: ex: `meuservidor-sql`
- **Login do administrador**: `adminuser`
- **Senha segura**: contendo letras, números e símbolos

![image](https://github.com/user-attachments/assets/af29a78c-3e74-40fd-9a51-c08f852b7bf4)

---

### 4. Regras de firewall

Permita acesso a seu IP atual para conseguir se conectar à instância pelo SSMS, Azure Data Studio ou terminal.

---

### 5. Criar banco de dados

Configure o nome do banco de dados e selecione um plano de uso.

---

### 6. Conectar ao banco

Use o IP e credenciais criadas para conectar via alguma ferramenta cliente de SQL (como Azure Data Studio ou DBeaver).

```sql
-- Exemplo de conexão usando Azure Data Studio
Servidor: meuservidor-sql.database.windows.net
Usuário: adminuser
Senha: *********
Banco de dados: meudb
```

---

## 💡 Dicas
- Nunca exponha suas credenciais em um ambiente público
- Habilite acesso ao IP corretamente ou você não conseguirá se conectar
- Monitore o uso gratuito para evitar cobranças indesejadas
