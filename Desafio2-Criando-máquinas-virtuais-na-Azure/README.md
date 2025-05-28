# 🚀 Desafio DIO - Criação de uma Máquina Virtual no Azure

## 🎯 Objetivo

Este projeto tem como objetivo aplicar os conhecimentos adquiridos sobre a plataforma Microsoft Azure, especificamente no processo de criação e configuração de uma Máquina Virtual (VM). Além disso, este repositório servirá como material de apoio para estudos e futuras implementações.

## 📚 Tecnologias e Ferramentas Utilizadas

- Microsoft Azure (Portal Web)  
- GitHub  
- Markdown  
- Sistemas Operacionais (Windows Server / Ubuntu)  
- RDP e SSH para acesso remoto  

## 🛠️ Passo a Passo: Criando uma Máquina Virtual no Azure

### 1. Pré-requisitos

Antes de iniciar, você deve ter:  
- Uma conta ativa no Azure  
- Acesso ao [Portal do Azure](https://portal.azure.com)  

### 2. Acessando o Portal do Azure

- Faça login no Portal do Azure  
- No painel principal, pesquise por "Máquinas Virtuais" e selecione a opção correspondente  

### 3. Criando a Máquina Virtual

- Clique em "Criar" > "Máquina Virtual"  
- Preencha as informações solicitadas no assistente de criação:  

#### Informações Básicas  
- **Assinatura**: Escolha a vinculada à sua conta  
- **Grupo de Recursos**: Crie ou selecione um existente  
- **Nome da VM**: Escolha um nome identificável  
- **Região**: Ex.: Leste dos EUA, Europa Ocidental  

#### Imagem e Tamanho  
- **Imagem do SO**: Windows Server, Ubuntu, etc.  
- **Tamanho**: Escolha com base nas necessidades de CPU/RAM  

#### Autenticação e Acesso  
- **Nome de usuário administrador**: defina um nome de fácil identificação  
- **Método de autenticação**:  
  - *Senha*: escolha uma senha forte  
  - *Chave SSH*: mais segura, recomendada para Linux  
- **Portas de acesso permitidas**:  
  - RDP (porta 3389) para VMs com Windows  
  - SSH (porta 22) para VMs com Linux  

### 4. Configuração de Armazenamento

- **Tipo de disco do SO**: SSD Premium, SSD Padrão ou HDD Padrão  
- **Discos adicionais**: Opcional, dependendo da aplicação  

### 5. Configuração de Rede

- **Rede Virtual** e **Sub-rede**: Use existente ou crie nova  
- **Endereço IP público**: Habilite para acesso externo  
- **Grupo de Segurança de Rede (NSG)**: Defina regras de entrada e saída  

### 6. Revisar e Criar

- Clique em “Revisar + Criar”  
- Verifique as configurações e clique em “Criar”  

### 7. Acessando a Máquina Virtual

Após a implantação:  
- Vá em "Máquinas Virtuais"  
- Selecione sua VM e clique em **Conectar**  

#### Windows:  
- Baixe o arquivo `.rdp` e abra via Remote Desktop  

#### Linux:  
- Use o comando SSH fornecido no portal  

## 💡 Dicas e Boas Práticas

- Desligue a VM quando não estiver usando para evitar custos  
- Prefira tamanhos de VM mais simples para testes (ex.: B1s)  
- Mantenha o firewall e o NSG sempre configurados com o mínimo necessário  
- Use **Chave SSH** em vez de senha para maior segurança em VMs Linux  

## 📎 Referências

- [Documentação Oficial do Azure - Máquinas Virtuais](https://learn.microsoft.com/pt-br/azure/virtual-machines/)  
- [Portal do Azure](https://portal.azure.com/)  

## ✅ Conclusão

Este repositório foi criado como parte do **desafio do curso AZ-900 da DIO**, com o intuito de reforçar o aprendizado prático sobre máquinas virtuais no Azure, além de incentivar a documentação técnica e o uso do GitHub em projetos reais.
