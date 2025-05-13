# 🗄️ Criando uma Instância de Banco de Dados no Azure

Este repositório foi criado como parte de um desafio prático na DIO, com o objetivo de documentar a criação de uma instância de banco de dados na plataforma Microsoft Azure. Aqui você vai encontrar os principais passos, dicas e imagens do processo, para ajudar nos seus estudos ou futuras implementações. 🚀

## 🎯 Objetivo

Praticar a criação de uma instância gerenciada de banco de dados no Azure, com foco em:

- Compreender as etapas da configuração
- Documentar o processo de forma clara
- Consolidar conhecimentos sobre o uso da Azure

## 🧭 Passo a Passo

### 1. Acessar o portal Azure

Acesse [https://portal.azure.com](https://portal.azure.com) e entre na sua conta.

![Portal Azure](images/portal-db.png)

---

### 2. Criar um novo recurso de banco de dados

Clique em **"Criar um recurso"** → **"Banco de dados"** → Escolha a opção desejada (ex: Banco de Dados SQL).

### 3. Preencher as configurações básicas

- **Grupo de recursos**: crie um novo ou use um existente
- **Nome do servidor**: ex: `meuservidor-sql`
- **Login do administrador**: `adminuser`
- **Senha segura**: algo forte, contendo letras, números e símbolos

![Configuração SQL](images/sql-config.png)

---

### 4. Regras de firewall

Permita acesso a seu IP atual para conseguir se conectar à instância pelo SSMS, Azure Data Studio ou terminal.

---

### 5. Criar banco de dados

Configure o nome do banco de dados e selecione um plano de uso (idealmente gratuito ou com baixo custo para testes).

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

- Use nomes fáceis de lembrar e identificar
- Habilite acesso ao IP corretamente ou você não conseguirá se conectar
- Monitore o uso gratuito para evitar cobranças

---

## 📂 Estrutura do Projeto

```
📦 azure-db-lab/
├── README.md
├── images/
│   ├── portal-db.png
│   └── sql-config.png
```

---

Com isso, você conclui mais um passo rumo à sua especialização em nuvem. Salve esse repositório, compartilhe com colegas e continue praticando! ☁️🧠
