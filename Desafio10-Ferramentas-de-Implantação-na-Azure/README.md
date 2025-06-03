# 🚀 Resumo do Lab: Ferramentas de Implantação na Microsoft Azure

## Sobre o Desafio

Este repositório foi criado como parte do desafio da DIO, com o objetivo de registrar os aprendizados sobre as **principais ferramentas de implantação no Azure**, utilizadas para provisionar, configurar e automatizar recursos de forma eficiente. Aqui está um resumo completo do que foi estudado e aplicado no laboratório.

## ✅ O que eu aprendi

Durante o lab, explorei diversas ferramentas e métodos que o Azure disponibiliza para facilitar e padronizar a implantação de recursos na nuvem. Os principais destaques foram:

### 🧰 Azure Portal

- Utilizei o **Portal do Azure** para realizar implantações manuais com interface gráfica.
- Criação de máquinas virtuais, contas de armazenamento e redes foi feita de forma prática.
- Entendi que o portal é ótimo para testes, mas não escalável para ambientes maiores.

### 🖥️ Azure CLI

- Aprendi a usar o **Azure Command-Line Interface (CLI)** para implantar recursos via terminal.
- Realizei login com `az login` e usei comandos como `az group create` e `az vm create`.
- A CLI permite **automação e scriptability**, sendo ideal para quem prefere linha de comando.

### 🧾 Azure PowerShell

- Estudei o uso do **PowerShell com módulos do Azure** para automação de tarefas.
- Executei comandos como `New-AzResourceGroup` e `New-AzVM`.
- A flexibilidade do PowerShell facilita o gerenciamento de múltiplos recursos com lógica condicional.

### 📦 Modelos ARM (Azure Resource Manager)

- Criei **templates ARM** para implantar recursos com base em arquivos JSON.
- Os modelos permitem reutilização, versionamento e padronização de ambientes.
- Implantação feita via Azure Portal, CLI ou PowerShell usando os mesmos arquivos.

### 🔄 Azure Bicep

- Conheci o **Azure Bicep**, linguagem mais simples e moderna que substitui o JSON dos ARM templates.
- Usei sintaxe declarativa para criar scripts de infraestrutura como código (IaC).
- Foco em **leitura facilitada**, reaproveitamento e integração com DevOps.

### 🧪 Azure DevOps & GitHub Actions (menção prática)

- Embora não tenham sido aplicadas diretamente no lab, compreendi que **Azure DevOps** e **GitHub Actions** são ferramentas robustas para CI/CD.
- Elas integram com os templates ARM ou Bicep, automatizando o pipeline de implantação com qualidade e versionamento.

## 💡 Considerações Finais

Aprender sobre as ferramentas de implantação do Azure me mostrou que existem várias formas de criar e gerenciar recursos, desde interfaces gráficas até infraestrutura como código. Cada ferramenta tem seu propósito, e o ideal é escolher aquela que melhor se adapta ao projeto e ao time.
