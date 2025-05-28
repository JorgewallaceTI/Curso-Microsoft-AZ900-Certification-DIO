# 🗃️ Desafio DIO - Configuração de um Banco de Dados SQL no Azure

## 🎯 Finalidade

Este guia tem como proposta orientar o processo de criação e configuração de um banco de dados SQL no ambiente Azure, de maneira prática e objetiva. Ao final, você terá um banco funcional e entenderá como acessá-lo com ferramentas adequadas.

## 🔧 Etapas para Criar seu Banco de Dados no Azure

### 1. Criando sua Conta na Plataforma Azure 🌐

Antes de começar, verifique se você já possui uma conta no [Portal do Azure](https://portal.azure.com). Caso não tenha, será necessário criar uma gratuitamente. Após isso, entre com suas credenciais no portal.

### 2. Localizando o Serviço de Banco de Dados 🖥️

Já dentro do portal:
- Use a barra de busca superior para pesquisar por **"SQL Database"**
- Escolha a opção correspondente ao **Banco de Dados SQL**
- Clique em **Criar** para iniciar a configuração

### 3. Definindo Informações Iniciais 📋

Durante a configuração, preencha os seguintes campos:

- **Nome do banco de dados**: algo fácil de identificar
- **Assinatura**: selecione a conta vinculada ao serviço
- **Grupo de recursos**: selecione um já existente ou crie um novo para organização
- **Servidor**:
  - Caso ainda não tenha, crie um novo servidor
  - Escolha um nome exclusivo, região mais próxima, nome de usuário e uma senha forte

### 4. Selecionando o Plano de Serviço 🔧

Agora escolha o tipo de serviço de acordo com sua necessidade:

- **Básico**: indicado para testes ou aplicações simples
- **Standard**: ideal para projetos com uso moderado
- **Premium** e **Hyperscale**: para demandas de alto desempenho ou grande volume de dados

Você pode optar pelo modelo **DTU** (unidades de desempenho) ou **vCore** (núcleos virtuais), conforme o tipo de carga esperada.

### 5. Configurando o Acesso à Rede 🌐

Determine como o banco poderá ser acessado:

- **Conexão pública**: libera o acesso por meio da internet
- **Conexão privada**: restringe o acesso à rede do Azure

Em seguida:
- Habilite o firewall para incluir seu IP atual
- Configure outras regras se necessário, permitindo ou bloqueando outros IPs

### 6. Protegendo o Banco de Dados 🔐

Recomendações de segurança:

- Ative a **Autenticação via Azure Active Directory** (AAD), se aplicável
- Use o **Defender para SQL** para proteger contra ameaças em tempo real
- Habilite **auditoria e monitoramento** para registrar alterações e acessos

### 7. Estratégia de Backup e Redundância 🛡️

Defina como os backups serão feitos:

- **Geo-redundância**: armazena cópias em diferentes regiões
- **Redundância local**: mantém as cópias na mesma localização

Escolha de acordo com sua necessidade de recuperação de desastres.

### 8. Revisão e Criação 🔍

Com tudo configurado:
- Clique em **Revisar + Criar**
- Confirme os dados preenchidos
- Clique em **Criar** e aguarde a implantação da instância

O processo pode levar alguns minutos até que esteja concluído.

### 9. Conectando ao Banco de Dados 🚀

Para acessar seu banco de dados:

1. Vá até **SQL Databases** no menu lateral do portal
2. Escolha o banco recém-criado
3. Copie o **nome do servidor**
4. Abra o **SSMS** ou o **Azure Data Studio**
5. Insira o nome do servidor, o usuário administrador e a senha definida anteriormente
6. Conecte-se ao banco e comece a explorar, executar comandos e estruturar tabelas

## 💡 Dicas Extras

- Mantenha o acesso restrito apenas a IPs confiáveis
- Utilize autenticação com chave e não apenas por senha, sempre que possível
- Para testes, utilize planos com menor custo
- Utilize ferramentas de monitoramento integradas para acompanhar o desempenho

## 📌 Recursos Adicionais

- [Documentação oficial do Azure SQL](https://learn.microsoft.com/pt-br/azure/azure-sql/)
- [Guia de Segurança no Azure SQL](https://learn.microsoft.com/pt-br/azure/azure-sql/database/security-overview)

## ✅ Conclusão

Com esse passo a passo, foi possível criar um banco de dados funcional no Azure, entender os principais parâmetros de configuração e conectividade, além de aplicar boas práticas de segurança e desempenho.
