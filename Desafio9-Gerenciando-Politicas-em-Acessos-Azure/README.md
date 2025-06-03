# 🔐 Resumo do Lab: Gerenciando Políticas de Acesso no Microsoft Azure

## Sobre o Desafio

Este repositório foi criado como parte do desafio da DIO, com o objetivo de consolidar os aprendizados sobre como **gerenciar políticas e permissões de acesso** no Azure de maneira segura, eficiente e alinhada às boas práticas de governança. Aqui você encontrará um resumo claro do que estudei e apliquei durante o laboratório.

## ✅ O que eu aprendi

Durante o desenvolvimento do lab, tive a oportunidade de explorar **recursos fundamentais de controle de acesso** no Azure. Estes são os principais tópicos abordados:

### 🧑‍💼 RBAC – Controle de Acesso Baseado em Funções

- Entendi como o RBAC permite o controle preciso sobre **quem pode fazer o quê** em cada recurso do Azure.
- Aprendi a **atribuir funções** (como Leitor, Colaborador ou Proprietário) a usuários, grupos e identidades gerenciadas.
- Executei testes para validar o acesso concedido e garanti o **princípio do menor privilégio**.

### 📜 Azure Policy

- Explorei o serviço **Azure Policy** para aplicar regras e impor padrões organizacionais em recursos.
- Criei e atribuí políticas para restringir a criação de recursos fora da região permitida.
- Avaliei a **compliance** dos recursos já existentes em relação às políticas aplicadas.

### 🔒 Acesso Condicional

- Conheci os **acessos condicionais** no Microsoft Entra ID, com base em critérios como localização, tipo de dispositivo e risco de login.
- Criei políticas que exigem **autenticação multifator (MFA)** em determinadas situações.
- Implementei bloqueios de acesso baseados em regras e contexto de login.

### 🛡️ Boas Práticas de Segurança

- Organizar usuários em **grupos de segurança** e aplicar permissões em nível de grupo.
- Evitar a concessão de permissões amplas ou indefinidas.
- Monitorar alterações em políticas de acesso com **auditoria via Azure Monitor**.

## 💡 Considerações Finais

Esse laboratório me ajudou a entender que o gerenciamento de acesso é uma **parte crítica da segurança em nuvem**. Aprender a aplicar políticas, atribuir funções com precisão e garantir conformidade reforça a segurança da infraestrutura e reduz riscos operacionais.
