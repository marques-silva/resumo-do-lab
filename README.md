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

# Módulo 2: Arquitetura e Serviços do Azure

## Computação e Rede

### Tipos de Computação
- Hospedagem de aplicativos
- Redes virtuais

### Domínio de Objetivo
- Comparar tipos de computação, incluindo instâncias de contêiner, máquinas virtuais e funções.
- Descrever os recursos exigidos para as máquinas virtuais.
- Definir pontos de extremidade públicos e privados.
- Descrever as opções de máquina virtual, incluindo VMs, conjuntos de dimensionamento de máquinas virtuais, conjuntos de disponibilidade de máquinas virtuais e a Área de Trabalho Virtual do Azure.

## Serviços de Computação do Azure
A Computação do Azure é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

### Máquinas Virtuais do Azure
- As máquinas virtuais do Azure (VMs) são emulações de software de computadores físicos.
- Incluem processador virtual, memória, armazenamento e rede.
- Oferecem IaaS com personalização e controle total.

### Conjuntos de Dimensionamento de VMs
Os conjuntos de dimensionamento oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente.
- **Escalar horizontalmente** quando o recurso precisar aumentar.
- **Reduzir horizontalmente** quando o recurso precisar diminuir.

### Conjuntos de Disponibilidade de VM

## Área de Trabalho Virtual do Azure
A Área de Trabalho Virtual do Azure é uma virtualização de área de trabalho e aplicativo executada na nuvem.
- Crie um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway.
- Reduza o risco de que o recurso seja deixado para trás.
- Implantações reais de várias sessões.

## Serviços de Contêineres do Azure
Os contêineres do Azure fornecem um ambiente leve e virtualizado que não exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda.
- **Instâncias de Contêiner do Azure:** uma oferta de PaaS que executa um contêiner ou pod de contêineres no Azure.
- **Aplicativos de Contêiner do Azure:** uma oferta de PaaS que pode balancear a carga e escalar.
- **Serviço de Kubernetes do Azure:** um serviço de orquestração para contêineres com arquiteturas distribuídas e grandes volumes de contêineres.

## Azure Functions
Azure Functions é uma oferta de PaaS que dá suporte a operações de computação sem servidor. O código baseado em eventos é executado quando chamado, sem exigir uma infraestrutura de servidor durante períodos inativos.

## Comparar Opções de Computação do Azure
### Máquinas Virtuais
- Servidor baseado em nuvem que dá suporte a ambientes Windows ou Linux.
- Útil para migrações de lift-and-shift para a nuvem.
- Pacote do sistema operacional completo, incluindo o sistema operacional do host.

### Área de Trabalho Virtual
- Fornece uma experiência de área de trabalho do Windows baseada em nuvem.
- Aplicativos dedicados para conexão e uso ou acessíveis de qualquer navegador moderno.
- O logon de vários clientes permite que vários usuários façam logon no mesmo computador ao mesmo tempo.

### Contêineres
- Ambiente leve e em miniatura adequado para a execução de microsserviços.
- Projetado para escalabilidade e resiliência por meio da orquestração.
- Os aplicativos e serviços são empacotados em um contêiner que fica na parte superior do sistema operacional do host. Vários contêineres podem coexistir em um sistema operacional do host.

## Serviços de Aplicativo do Azure
Os Serviços de Aplicativos do Azure consistem em uma plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos Web e APIs rapidamente.
- Trabalha com .NET, .NET Core, Node.js, Java, Python ou PHP.
- Oferta de PaaS com requisitos de nível corporativo de desempenho, segurança e conformidade.

## Serviços de Rede do Azure
- A Rede Virtual do Azure (VNet) permite que os recursos do Azure se comuniquem uns com os outros, com a Internet e com redes locais.
- Pontos de extremidade públicos, acessíveis de qualquer lugar na Internet.
- Pontos de extremidade privados, acessíveis somente de dentro da sua rede.

As sub-redes virtuais segmentam sua rede para atender às suas necessidades. O emparelhamento de rede conecta suas redes privadas diretamente.

### Gateway de VPN
O Gateway de VPN é usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela Internet pública.

### ExpressRoute
O ExpressRoute estende as redes locais para o Azure por meio de uma conexão privada facilitada por um provedor de conectividade.

### DNS do Azure
- Confiabilidade e desempenho aproveitando uma rede global de servidores de nome DNS usando a rede Anycast.
- A segurança do DNS do Azure baseia-se no gerenciador de recursos do Azure, habilitando o controle de acesso baseado em função e o monitoramento e registro em log.
- Facilidade de uso para gerenciar seus recursos externos e do Azure com um único serviço DNS.
- Redes virtuais personalizáveis permitem que você use nomes de domínio privados e totalmente personalizados em suas redes virtuais privadas.
- Os registros de alias dão suporte a conjuntos de registros de alias para apontar diretamente para um recurso do Azure.


# Armazenamento

- Serviços de armazenamento
- Opções de redundância
- Gerenciamento e migração de arquivos

# Contas de Armazenamento

- Deve ter um nome globalmente exclusivo.
- Fornecer acesso à Internet em todo o mundo.
- Determinar os serviços de armazenamento e as opções de redundância.

# Redundância de armazenamento
| Configuração de redeundância | Implantação | Durabilidade |
| --- | --- | --- |
| LRS (Armazenamento com redundância local) | Datacenter individual na Região primária | 11 noves |
| ZRS (Armazenamento com redundância de zona) | Três zonas de disponibilidade na regiâo primária | 12 noves |
| GRS (Armazenamento com redundância geográfica) | Datacenter único no primário e região secundária | 16 noves |
| GZRS (Armazenamento com redundância de zona geográfica) | Três zonas de disponibilidade na região primária e um único datacenter na região secundária | 16 noves |

# Serviços de armazenamento do Azure

- **Blob do Azure**: otimizado para o armazenamento de quantidades massivas de dados não estruturados, como texto ou dados binários.
- **Disco do Azure**: fornece discos para máquinas virtuais, aplicativos e outros serviços acessarem e utilizarem.
- **Fila do Azure**: serviço de armazenamento de mensagens que fornece armazenamento e recuperação para grandes quantidades de mensagens, cada uma com até 64 KB.
- **Arquivos do Azure**: configura um compartilhamento de arquivos de rede altamente disponível que pode ser utilizado usando o protocolo Bloco de Mensagens do Servidor.
- **Tabelas do Azure**: fornece uma opção de chave/atributo para o armazenamento de dados estruturados não relacionais com um design sem esquema.

# Pontos de extremidade públicos do serviço de armazenamento


![image](https://github.com/user-attachments/assets/b8f5a46e-67ea-4a6d-8233-cb90046d5d57)


# Camadas de acesso de armazenamento do Azure

![image](https://github.com/user-attachments/assets/030426ac-31ca-4ef4-bb0f-52d4989808f1)


# Migrações para o Azure

## Azure Data Box

- Armazenar até 80 terabytes de dados.
- Mova os backups de recuperação de desastre para o Azure.
- Proteja seus dados em uma caixa robusta durante o trânsito.
- Migre dados do Azure para conformidade ou necessidades regulatórias.
- Migre dados para o Azure de locais remotos com conectividade limitada ou sem conectividade.

![image](https://github.com/user-attachments/assets/ff4abaea-ab35-43e1-8e75-b5d91d5a295a)


# Opções de gerenciamento de arquivos

## AzCopy

- Utilitário de linha de comando.
- Copiar blobs ou arquivos de ou para sua conta de armazenamento.
- Sincronização em uma direção.

## Gerenciador de Armazenamento do Azure

- Interface gráfica do usuário (de modo semelhante ao Windows Explorer).
- Compatível com Windows, MacOS e Linux.

## Sincronização de Arquivos do Azure

- Sincroniza os arquivos do Azure e locais de forma bidirecional.
- A camada de nuvem mantém os arquivos acessados com frequência no local, enquanto libera espaço.


