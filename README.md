
# Azure 

## Introdução

Bem-vindo ao meu repositório de anotações sobre Azure! Este repositório contém minhas anotações, dicas e referências sobre os serviços e ferramentas oferecidos pela Microsoft Azure.

## Índice

- [Introdução ao Azure](#introdução-ao-azure)
- [Serviços Principais do Azure](#serviços-principais-do-azure)
  - [Computação](#computação)
  - [Armazenamento](#armazenamento)
  - [Redes](#redes)
  - [Banco de Dados](#banco-de-dados)
- [Ferramentas de Gerenciamento](#ferramentas-de-gerenciamento)
- [Segurança e Conformidade](#segurança-e-conformidade)
- [Referências](#referências)

## Introdução ao Azure

Microsoft Azure é uma plataforma de computação em nuvem que oferece uma ampla gama de serviços para desenvolvimento, gerenciamento e implantação de aplicativos através de uma rede global de data centers. Azure permite a criação de soluções escaláveis, seguras e eficientes.

## Serviços Principais do Azure

### Computação

- **Máquinas Virtuais (VMs)**: Instâncias de computação escaláveis sob demanda.
- **App Services**: Hospedagem para aplicativos web e APIs.
- **Azure Functions**: Computação sem servidor para execução de código sob demanda.

### Armazenamento

- **Blob Storage**: Armazenamento de objetos para dados não estruturados.
- **File Storage**: Compartilhamento de arquivos gerenciados.
- **Queue Storage**: Armazenamento de mensagens em fila para comunicação assíncrona.

### Redes

- **Virtual Network (VNet)**: Redes privadas no Azure.
- **Load Balancer**: Distribuição de tráfego para alta disponibilidade.
- **VPN Gateway**: Conexões seguras entre redes locais e o Azure.

### Banco de Dados

- **Azure SQL Database**: Banco de dados gerenciado baseado no SQL Server.
- **Cosmos DB**: Banco de dados NoSQL distribuído globalmente.
- **Azure Database for MySQL/PostgreSQL**: Bancos de dados relacionais gerenciados.

## Ferramentas de Gerenciamento

- **Azure Portal**: Interface web para gerenciamento de serviços Azure.
- **Azure CLI**: Interface de linha de comando para gerenciamento e automação.
- **Azure Resource Manager (ARM)**: Implantação e gerenciamento de recursos.

## Segurança e Conformidade

- **Azure Security Center**: Gerenciamento de segurança unificado.
- **Azure Policy**: Gestão e imposição de políticas de conformidade.
- **Azure AD**: Gerenciamento de identidades e acessos.

## Referências

- [Documentação Oficial do Azure](https://docs.microsoft.com/en-us/azure/)
- [Tutoriais do Azure](https://docs.microsoft.com/en-us/learn/azure/)
- [Blog do Azure](https://azure.microsoft.com/en-us/blog/)

---

## Criação de Máquinas Virtuais

### Passo a Passo para Criar uma Máquina Virtual no Azure

1. **Acesse o Portal do Azure**:
   - Navegue até o [Azure Portal](https://portal.azure.com/) e faça login com suas credenciais.

2. **Criação de um Novo Recurso**:
   - No menu esquerdo, clique em **"Create a resource"**.
   - Na barra de pesquisa, digite **"Virtual Machine"** e selecione a opção correspondente.

3. **Configuração Básica**:
   - No painel de criação da VM, preencha as informações básicas:
     - **Subscription**: Selecione sua assinatura do Azure.
     - **Resource Group**: Crie um novo ou selecione um grupo de recursos existente.
     - **Virtual Machine Name**: Dê um nome à sua VM.
     - **Region**: Escolha a região mais próxima de você ou que atenda melhor às suas necessidades.
     - **Availability Options**: Selecione uma opção de disponibilidade, se necessário.

4. **Escolha da Imagem**:
   - Em **Image**, escolha o sistema operacional que deseja instalar (ex.: Windows Server, Ubuntu).

5. **Tamanho da Máquina Virtual**:
   - Em **Size**, escolha o tamanho da VM (número de CPUs, memória). Utilize a opção "See all sizes" para visualizar todas as opções disponíveis.

6. **Configurações de Administração**:
   - Configure as credenciais de login:
     - **Authentication Type**: Escolha entre senha ou chave SSH.
     - **Username**: Insira o nome do usuário.
     - **Password/SSH Key**: Insira a senha ou carregue a chave SSH.

7. **Discos**:
   - Configure os discos de armazenamento:
     - **OS disk type**: Escolha o tipo de disco para o sistema operacional (Standard HDD, Standard SSD, Premium SSD).
     - Adicione discos adicionais, se necessário.

8. **Rede**:
   - Configure as opções de rede:
     - **Virtual Network**: Selecione uma rede virtual existente ou crie uma nova.
     - **Subnet**: Escolha a sub-rede.
     - **Public IP**: Configure o IP público, se necessário.
     - **NIC Network Security Group**: Configure as regras de segurança de rede.

9. **Revisão e Criação**:
   - Revise todas as configurações e clique em **"Review + create"**.
   - Após a validação das configurações, clique em **"Create"** para iniciar a criação da VM.

10. **Acesso à Máquina Virtual**:
    - Após a criação, navegue até a VM no portal do Azure.
    - Utilize o endereço IP público e as credenciais configuradas para acessar a VM via RDP (Windows) ou SSH (Linux).

---
## Calculadora de Custos do Azure

### Passo a Passo para Usar a Calculadora de Custos do Azure

1. **Acesse a Calculadora de Custos do Azure**:
   - Navegue até a [Calculadora de Preços do Azure](https://azure.microsoft.com/en-us/pricing/calculator/) no seu navegador.

2. **Adicionar Produtos**:
   - Na página inicial da calculadora, você verá uma barra de pesquisa. Digite o nome do serviço que deseja adicionar (por exemplo, Virtual Machine).
   - Selecione o serviço nos resultados da pesquisa e ele será adicionado à calculadora.

3. **Configurar Serviços**:
   - Para cada serviço adicionado, configure as opções específicas de acordo com suas necessidades:
     - **Região**: Escolha a região onde o serviço será utilizado.
     - **Tipo de Instância**: Selecione o tipo e tamanho da instância (para VMs).
     - **Opções de Pagamento**: Escolha o modelo de pagamento (Pay-As-You-Go, Reserved, etc.).
     - **Quantidade**: Insira a quantidade de recursos que você planeja usar.

4. **Visualizar Estimativa de Custos**:
   - Conforme você adiciona e configura serviços, a calculadora exibirá uma estimativa de custos na parte inferior da página.
   - Você pode ver os custos mensais e anuais estimados para cada serviço individualmente e o total combinado.

5. **Salvar e Compartilhar Estimativas**:
   - Você pode salvar a estimativa de custos para referência futura clicando em **"Export"** no canto superior direito e escolhendo a opção de formato (Excel, PDF).
   - Para compartilhar a estimativa com colegas ou clientes, clique em **"Share"** e copie o link gerado.

6. **Revisar e Ajustar**:
   - Revise sua estimativa regularmente e ajuste as configurações conforme necessário para garantir que você esteja dentro do orçamento e aproveitando ao máximo os serviços do Azure.

### Dicas para Uso Eficiente da Calculadora de Custos

- **Explore Diferentes Configurações**: Teste diferentes configurações para ver como elas afetam o custo total.
- **Comparar Regiões**: Alguns serviços podem ser mais baratos em determinadas regiões.
- **Reservas e Descontos**: Aproveite as opções de reservas e programas de descontos oferecidos pelo Azure para reduzir custos.

### Referências Adicionais

- [Documentação da Calculadora de Preços do Azure](https://docs.microsoft.com/en-us/azure/cost-management-billing/costs-overview)
- [Azure Pricing Overview](https://azure.microsoft.com/en-us/pricing/)

---
## Componentes de Arquitetura do Azure

### Introdução

A arquitetura do Azure é composta por diversos componentes que trabalham juntos para fornecer soluções de nuvem escaláveis, seguras e eficientes. Compreender esses componentes é essencial para planejar, projetar e implementar sistemas robustos na plataforma Azure.

### Principais Componentes

1. **Grupos de Recursos (Resource Groups)**
   - Contêiner lógico que agrupa recursos relacionados para facilitar a gestão e organização.
   - Permite gerenciar, monitorar e aplicar políticas de segurança a todos os recursos dentro do grupo.

2. **Máquinas Virtuais (Virtual Machines)**
   - Instâncias de computação que podem ser configuradas com diferentes sistemas operacionais e tamanhos.
   - Utilizadas para hospedar aplicativos, bancos de dados, e serviços em nuvem.

3. **Armazenamento (Storage)**
   - **Blob Storage**: Armazenamento de objetos para dados não estruturados.
   - **Disk Storage**: Discos gerenciados para VMs.
   - **File Storage**: Compartilhamento de arquivos acessível via SMB.
   - **Queue Storage**: Armazenamento de mensagens em fila para comunicação assíncrona.

4. **Redes Virtuais (Virtual Networks)**
   - Rede privada no Azure que permite a comunicação segura entre recursos.
   - Suporta sub-redes, configurações de segurança, e VPNs.

5. **Gateways de VPN (VPN Gateways)**
   - Permitem a conectividade segura entre redes locais e a nuvem Azure.
   - Suportam conexões site-to-site, point-to-site, e express route.

6. **Balançadores de Carga (Load Balancers)**
   - Distribuem tráfego de rede entre várias VMs ou serviços para alta disponibilidade e escalabilidade.
   - Suportam tráfego de entrada e de saída.

7. **Serviço de Aplicativos (App Services)**
   - Plataforma de hospedagem para aplicativos web, APIs e serviços móveis.
   - Suporta várias linguagens de programação e integrações contínuas.

8. **Banco de Dados Gerenciados**
   - **Azure SQL Database**: Banco de dados relacional baseado no SQL Server.
   - **Cosmos DB**: Banco de dados NoSQL distribuído globalmente.
   - **Azure Database for MySQL/PostgreSQL**: Bancos de dados relacionais gerenciados.

9. **Azure Functions**
   - Serviço de computação sem servidor que executa código sob demanda em resposta a eventos.
   - Ideal para tarefas automatizadas e processos de integração contínua.

10. **Monitoramento e Diagnóstico**
    - **Azure Monitor**: Serviço de monitoramento que coleta, analisa e age sobre métricas e logs de recursos do Azure.
    - **Application Insights**: Serviço de análise de desempenho de aplicativos que detecta anomalias e fornece diagnósticos detalhados.

### Ferramentas de Gestão

- **Azure Portal**: Interface web para criação e gerenciamento de recursos.
- **Azure CLI**: Ferramenta de linha de comando para automação e gerenciamento.
- **Azure Resource Manager (ARM)**: Interface que permite a implantação de recursos por meio de templates JSON.

### Referências Adicionais

- [Documentação de Arquitetura do Azure](https://docs.microsoft.com/en-us/azure/architecture/)
- [Modelos de Arquitetura no Azure](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/)

---

