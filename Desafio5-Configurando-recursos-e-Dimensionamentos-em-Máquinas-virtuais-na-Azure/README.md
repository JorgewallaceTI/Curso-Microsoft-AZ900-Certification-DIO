# ⚙️ Guia Completo: Configurando e Dimensionando Máquinas Virtuais no Azure

Este guia detalhado foi elaborado para ajudá-lo a criar, configurar e dimensionar suas Máquinas Virtuais (VMs) no Azure de forma eficiente, equilibrando desempenho e custo para diferentes tipos de carga de trabalho.

---

## ✅ Pré-requisitos

Antes de começar, certifique-se de:

- Ter uma conta ativa no [Azure](https://portal.azure.com)
- Ter permissões suficientes na assinatura
- Conhecer os requisitos de carga da aplicação

---

## 🌐 Passo 1: Acessar o Portal do Azure

1. Acesse [portal.azure.com](https://portal.azure.com)
2. No painel, procure por **"Máquinas Virtuais"** ou clique em **"Criar Recurso"**

---

## 🖥️ Passo 2: Criar a Máquina Virtual

1. Escolha a **assinatura** e o **grupo de recursos**
2. Defina:
   - **Nome da VM**
   - **Região**
   - **Sistema Operacional (Windows/Linux)**
   - **Imagem do sistema**
3. Configure as **credenciais de acesso**:
   - **Windows**: Usuário e senha
   - **Linux**: Chave SSH (recomendada)

---

## 📏 Passo 3: Configurar o Tamanho da VM

Escolha um tipo de instância:

- **Geral**: Cargas equilibradas
- **Otimizado para Memória**: Bancos de dados, caching
- **Otimizado para CPU**: Processos intensivos

### 📌 Dicas:

- Use o **Azure Advisor** para sugestões baseadas em consumo
- Configure **Autoescala** para escalar automaticamente com base no uso (CPU, memória)

---

## 💾 Passo 4: Configurar Armazenamento

Na aba **Discos**, escolha:

- **SSD Premium**: Alta performance
- **SSD Padrão**: Médio custo/desempenho
- **HDD Padrão**: Baixo custo

Adicione discos extras conforme necessidade.

---

## 🌐 Passo 5: Configurar a Rede

1. Conecte a uma **VNet existente** ou crie uma nova
2. Configure:
   - **Sub-rede**
   - **Grupo de Segurança de Rede (NSG)**: Permissões de entrada/saída
   - **Endereço IP Público** (opcional)

---

## 🔄 Passo 6: Escalabilidade e Dimensionamento

### ⚙️ Autoescala

- Defina métricas (CPU, memória)
- Configure mínimo/máximo de instâncias
- Reaja automaticamente à carga de trabalho

### 🛠️ Dimensionamento Manual

- Acesse a opção **"Dimensionar"**
- Altere tipo de VM, CPU, RAM conforme necessário

---

## 🔐 Passo 7: Segurança e Monitoramento

### Segurança

- **NSG**: Defina regras de firewall
- Use **credenciais fortes** e armazene em **Azure Key Vault**
- Mantenha o sistema atualizado

### Monitoramento

- **Azure Monitor**: Acompanhamento de métricas
- **Alertas personalizados**: Ex. uso de CPU acima de 80%
- **Logs de Diagnóstico**: Análise aprofundada

---

## ♻️ Passo 8: Backup e Recuperação

1. Acesse o painel de **Backup**
2. Configure:
   - **Backup automático**
   - **Políticas de retenção**
   - **Plano de recuperação**

---

## 🎉 Passo 9: Criar a Máquina Virtual

- Revise todas as configurações (rede, armazenamento, escalabilidade)
- Clique em **Criar**
- Aguarde a conclusão do provisionamento

---

## 🌐 Passo 10: Conectar-se à Máquina Virtual

- **Windows**: Use **RDP (Área de Trabalho Remota)**
- **Linux**: Use **SSH**

> Use o botão **Conectar** no portal do Azure para obter instruções específicas.

---

## 📊 Passo 11: Gerenciar e Otimizar

- Use o **Azure Monitor** para métricas em tempo real
- Ajuste dimensionamento conforme necessário
- Considere usar **Balanceador de Carga** para escalar horizontalmente

---

## ✅ Conclusão

Com este guia, você está preparado para provisionar, escalar e manter VMs otimizadas no Azure. Um bom dimensionamento garante eficiência operacional e controle de custos.

> Para mais detalhes, consulte a [documentação oficial do Azure](https://learn.microsoft.com/azure/virtual-machines/).
