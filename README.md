# Resumo-do-lab
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO


# Guia de Aprendizagem: Git e GitHub

Este guia fornece instruções básicas para instalar e configurar o Git, criar um repositório, e enviar e baixar arquivos do GitHub.

## Instalação do Git

1. **Baixar o Git**:
   - Acesse o site oficial do Git: git-scm.com e fazer o Download para o seu sistema operacional.

2. **Instalar o Git**:
   - Execute o instalador baixado e siga as instruções na tela.
   - Durante a instalação, você pode escolher as configurações padrão.

## Configuração do Git

1. **Configurar o nome de usuário e email**:
   - Abra o terminal ou prompt de comando.
   - Execute os seguintes comandos, substituindo `seu_nome` e `seu_email` pelos seus dados:
     ```bash
     git config --global user.name "seu_nome"
     git config --global user.email "seu_email"
     ```

2. **Verificar a configuração**:
   - Execute o comando:
     ```bash
     git config --list
     ```

## Criar um Repositório

1. **Inicializar um repositório local**:
   - Navegue até a pasta do seu projeto no terminal.
   - Execute o comando:
     ```bash
     git init
     ```

2. **Adicionar arquivos ao repositório**:
   - Adicione os arquivos que deseja versionar:
     ```bash
     git add .
     ```

3. **Fazer o primeiro commit**:
   - Execute o comando:
     ```bash
     git commit -m "Primeiro commit"
     ```

## Enviar para o GitHub

1. **Criar um repositório no GitHub**:
   - Acesse o GitHub e crie um novo repositório.

2. **Conectar o repositório local ao GitHub**:
   - No terminal, execute os comandos, substituindo `URL_DO_REPOSITORIO` pela URL do seu repositório no GitHub:
     ```bash
     git remote add origin URL_DO_REPOSITORIO
     git branch -M main
     git push -u origin main
     ```

## Baixar do GitHub

1. **Clonar um repositório existente**:
   - No terminal, execute o comando, substituindo `URL_DO_REPOSITORIO` pela URL do repositório que deseja clonar:
     ```bash
     git clone URL_DO_REPOSITORIO
     ```

## Contribuir com Alterações

1. **Fazer alterações e enviar para o GitHub**:
   - Após fazer alterações nos arquivos, adicione e faça commit das mudanças:
     ```bash
     git add .
     git commit -m "Descrição das alterações"
     git push
     ```
# Sobre Azure

1. **Neste tópico apendi sobre, escalabilidade, elasticidade, segurança, governança no Azure.
2. **Foi estudado sobre modelos de nuvem Iaas, Paas E Saas

   1. IaaS (Infrastructure as a Service): Fornece infraestrutura de TI virtualizada, como servidores, redes, armazenamento e sistemas operacionais. As empresas têm controle total sobre a infraestrutura, mas o provedor cuida do hardware subjacente. Exemplo: Amazon Web Services (AWS) EC2.

   2. PaaS (Platform as a Service): Oferece uma plataforma que permite aos desenvolvedores criar, gerenciar e implantar aplicativos sem se preocupar com a infraestrutura. A infraestrutura subjacente e o sistema operacional são gerenciados pelo provedor. Exemplo: Google App Engine, Microsoft Azure.

   3. SaaS (Software as a Service): O software é entregue via internet e é totalmente gerenciado pelo provedor. Os usuários não precisam se preocupar com a manutenção, infraestrutura ou desenvolvimento do software, apenas utilizam a aplicação. Exemplo: Google Workspace, Microsoft 365.
  
# Módulo 2: Componentes de Arquitetura do Azure

## Tópicos abordados

- **Regiões e Zonas de Disponibilidade**
  - Distribuição geográfica dos datacenters do Azure para garantir alta disponibilidade e recuperação de desastres.

- **Assinaturas e Grupos de Recursos**
  - Organização de recursos em grupos para melhor gerenciamento e controle de custos.

- **Datacenters do Azure**
  - Infraestrutura global que suporta os serviços do Azure, com foco em resiliência e segurança.

- **Assinaturas**
  - Modelos de contratação e faturamento que permitem o uso de diferentes serviços na plataforma Azure.

- **Grupos de Gerenciamento**
  - Estrutura hierárquica que facilita o gerenciamento de várias assinaturas, agrupando-as de acordo com a necessidade de controle e governança.

- **Hierarquia de Grupos de Recursos, Assinaturas e Grupos de Gerenciamento**
  - Organização lógica que define como os recursos são alocados, gerenciados e monitorados no ambiente Azure.

- **Regiões Soberanas do Azure**
  - Regiões específicas que atendem a requisitos de conformidade e soberania de dados em diferentes países e regiões.

## Atividades Práticas

- Criação de um **Grupo de Recursos**.
- Configuração de uma **Rede Virtual**.


