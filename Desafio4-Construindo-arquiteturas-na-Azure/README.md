# 🚀 Guia Prático: Criação e Gerenciamento de Infraestrutura no Microsoft Azure

Este repositório contém um passo a passo completo para planejar, implementar e gerenciar uma infraestrutura moderna e segura utilizando os serviços do Microsoft Azure. Ideal para estudantes, profissionais de TI e desenvolvedores que querem colocar projetos em produção com organização e boas práticas.

---

## 🧠 1. Planejamento da Arquitetura

Antes de iniciar, avalie:

- Quais serviços do Azure você vai usar? (VMs, Banco de Dados, etc.)
- Como os componentes se comunicam entre si?
- Necessidade de alta disponibilidade ou escalabilidade?
- Requisitos de conformidade ou segurança?

👉 Utilize o [Azure Well-Architected Framework](https://learn.microsoft.com/azure/architecture/framework/) como base de boas práticas.

---

## 📁 2. Criação do Grupo de Recursos

1. No [Portal Azure](https://portal.azure.com), busque por **"Grupos de Recursos"**.
2. Clique em **Criar**.
3. Preencha:
   - **Nome do grupo**
   - **Região**
4. Clique em **Revisar + Criar** e depois em **Criar**.

---

## 🌐 3. Configuração da Rede Virtual (VNet)

1. Acesse **"Rede Virtual"** no portal.
2. Clique em **Criar** e informe:
   - Nome da rede
   - Região
   - Faixa de IPs (ex: `10.0.0.0/16`)
   - Sub-rede (ex: `10.0.0.0/24`)
3. Finalize em **Revisar + Criar**.

---

## 🔐 4. Definição de Regras de Segurança

1. Procure por **"Grupo de Segurança de Rede (NSG)"**.
2. Crie regras:
   - Libere tráfego HTTP/HTTPS
   - Bloqueie portas desnecessárias
3. Associe o NSG à sub-rede ou interface da VM.

---

## 💻 5. Provisionamento de Máquinas Virtuais

1. No portal, pesquise por **"Máquinas Virtuais"** > Criar.
2. Escolha:
   - Sistema operacional
   - Tamanho e região
   - Usuário e senha
3. Conecte à VNet e aplique o NSG.
4. Finalize em **Criar**.

---

## ⚖️ 6. Balanceador de Carga (Opcional)

1. Procure por **"Balanceador de Carga"**.
2. Clique em **Criar** e escolha:
   - **Público** (tráfego externo) ou **Interno** (rede privada)
3. Defina as regras de distribuição.
4. Associe às suas VMs.

---

## 🗄️ 7. Banco de Dados no Azure

1. Acesse o menu **Banco de Dados SQL / MySQL / PostgreSQL**.
2. Configure:
   - Nome e credenciais
   - Desempenho e escalabilidade
3. Conecte à mesma VNet para segurança adicional.

---

## 🔍 8. Monitoramento e Alertas

1. Vá até **"Monitor"** no portal.
2. Ative logs e diagnósticos para os recursos.
3. Crie alertas (ex: CPU alta, falha de login).
4. Use **Azure Log Analytics** para analisar tudo em um só lugar.

---

## ♻️ 9. Backup e Redundância

1. Ative o **Azure Backup** para VMs e bancos de dados.
2. Configure política de retenção.
3. Para dados críticos, habilite **Replicação Geográfica**.

---

## 🔄 10. Otimização Contínua

- Use o **Azure Cost Management** para revisar gastos.
- Automatize tarefas com **Azure Automation / Runbooks**.
- Reavalie configurações de segurança periodicamente.

---

## ✅ Conclusão

Com esse guia, você terá uma base sólida para executar projetos no Azure de forma segura, escalável e econômica. Mantenha sua infraestrutura sob controle com boas práticas de monitoramento, segurança e organização.
