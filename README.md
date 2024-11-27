
# Azure Bootcamp 

## Introdução

Bem-vindo ao meu repositório de anotações do Bootcamp de Azure! Este repositório contém minhas anotações, dicas e referências sobre os serviços e ferramentas oferecidos pela Microsoft Azure.

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
