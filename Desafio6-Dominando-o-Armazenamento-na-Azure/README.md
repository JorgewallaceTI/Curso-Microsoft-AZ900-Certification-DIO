# 🗄️ Guia Completo de Armazenamento no Azure | Migração e Gerenciamento de Dados

Este guia abrangente foi criado para ajudá-lo a configurar, gerenciar e migrar dados no Azure, utilizando os serviços de armazenamento como **Blobs**, **Arquivos**, **Tabelas** e **Filas**. Siga este passo a passo para otimizar sua experiência com o armazenamento no Azure.

---

## ✅ Pré-requisitos

Antes de começar, garanta que você possui:

- Uma conta ativa no [Azure](https://portal.azure.com)
- Permissões para criar e gerenciar recursos de armazenamento

---

## 🌐 1. Acessar o Portal do Azure

1. Acesse [portal.azure.com](https://portal.azure.com)
2. No menu lateral esquerdo, clique em **"Criar um recurso"**

---

## ➕ 2. Criar e Configurar uma Conta de Armazenamento

### 🔧 Iniciar Criação

1. Pesquise por **"Conta de Armazenamento"**
2. Clique em **Criar**
3. Preencha os campos:

- **Assinatura**: Selecione a desejada
- **Grupo de Recursos**: Selecione ou crie um novo
- **Nome da Conta**: Deve ser único (3–24 caracteres minúsculos)
- **Região**: Escolha a mais próxima dos usuários
- **Desempenho**: Padrão ou Premium
- **Tipo de Conta**: General Purpose v2
- **Replicação**: LRS, GRS, ZRS, conforme o caso

### ⚙️ Configurações Avançadas

- Ativar **Transferência Segura (HTTPS)**
- Habilitar **compartilhamentos de arquivos grandes** para Azure Files
- Ativar **Hierarchical Namespace** para Azure Data Lake Storage Gen2

### 🔒 Configurações de Rede e Segurança

- Método de conexão: **Público** ou **Privado**
- Regras de firewall e redes virtuais
- Ativar **Criptografia** para os dados

> Finalize com **"Revisar + Criar"** e clique em **"Criar"**

---

## 📦 3. Configurar Armazenamento Blob

1. Vá até **Serviços de Armazenamento > Containers**
2. Clique em **Adicionar**
3. Defina o **nível de acesso**:
   - Privado
   - Público (Somente leitura)

4. Carregue arquivos diretamente via:
   - Portal
   - Azure CLI
   - Azure Storage Explorer

---

## 📁 4. Criar Compartilhamento de Arquivos

1. Vá até **Compartilhamentos de Arquivos**
2. Clique em **Adicionar**
3. Defina:
   - **Nome do compartilhamento**
   - **Tamanho**
4. Monte em uma **VM ou servidor** via protocolo **SMB**

---

## 📊 5. Utilização do Armazenamento de Tabelas

1. Vá até a seção **Tabelas**
2. Adicione uma nova tabela
3. Gerencie os dados usando:
   - **Azure SDK**
   - **API REST**

---

## 📬 6. Gerenciar Armazenamento de Filas

1. Vá até a seção **Filas**
2. Crie uma nova fila
3. Configure:
   - **Permissões de acesso**
   - Consumo via **API REST** ou **SDK**

---

## 🔄 7. Migrar Dados para o Azure

### 🧭 Criar Projeto de Migração

- Use o **Azure Migrate** para migrações organizadas

### 📥 Instalar AzCopy

- [Download do AzCopy](https://learn.microsoft.com/azure/storage/common/storage-use-azcopy-v10)

### 🔐 Autenticar com o Azure

- Autentique com credenciais seguras usando **Azure CLI**

---

## 🔍 8. Monitoramento e Alertas

- Use o **Azure Monitor** para acompanhar o uso
- Configure **alertas automáticos** para:
  - Falhas
  - Limites de capacidade
  - Anomalias de tráfego

---

## 💾 9. Backups e Replicação

- Configure o **Backup do Azure**
- Ative **Geo-Redundância (GRS)** para alta disponibilidade
- Use políticas de retenção e restauração

---

## ✅ Conclusão

Dominar o armazenamento no Azure envolve:

- Configuração adequada
- Monitoramento contínuo
- Migração estratégica
- Segurança e governança de dados

> Para mais detalhes, acesse a [documentação oficial do Azure Storage](https://learn.microsoft.com/azure/storage/).
