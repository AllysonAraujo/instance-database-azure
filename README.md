# Configuração de Instância de Banco de Dados no Azure

## 📋 Sobre o Projeto

Este repositório documenta minha experiência prática no desafio de configuração de uma instância de Banco de Dados na plataforma Microsoft Azure, como parte do curso da DIO (Digital Innovation One). O objetivo é aplicar os conceitos aprendidos e documentar o processo de forma clara e estruturada.

## 🎯 Objetivos de Aprendizagem

- ✅ Aplicar os conceitos aprendidos em um ambiente prático
- ✅ Documentar processos técnicos de forma clara e estruturada
- ✅ Utilizar o GitHub como ferramenta para compartilhamento de documentação técnica
- ✅ Compreender os serviços de banco de dados do Azure
- ✅ Configurar e gerenciar instâncias de SQL Database/SQL Managed Instance

## 🔧 Tecnologias Utilizadas

- **Microsoft Azure**: Plataforma de nuvem
- **Azure SQL Database**: Serviço de banco de dados como serviço (DBaaS)
- **Azure SQL Managed Instance**: Instância gerenciada de SQL Server
- **Azure Portal**: Interface de gerenciamento
- **SQL Server Management Studio (SSMS)**: Ferramenta de administração
- **GitHub**: Controle de versão e documentação

## 📚 Conteúdo do Repositório

### 📖 Documentação

- [Guia de Configuração](#-guia-de-configuração)
- [Resumos das Aulas](#-resumos-das-aulas)
- [Dicas e Boas Práticas](#-dicas-e-boas-práticas)
- [Troubleshooting](#-troubleshooting)


## 🚀 Guia de Configuração

### 1. Pré-requisitos

- Conta ativa no Microsoft Azure
- Acesso ao Azure Portal
- Conhecimento básico de SQL Server
- SQL Server Management Studio (opcional)

### 2. Passos para Criar uma Instância de Banco de Dados

#### 2.1 Azure SQL Database

1. **Acessar o Azure Portal**
   - Entre em [portal.azure.com](https://portal.azure.com)
   - Faça login com suas credenciais

2. **Criar Recurso**
   - Clique em "Criar um recurso"
   - Procure por "SQL Database"
   - Selecione "SQL Database" e clique em "Criar"

3. **Configurações Básicas**
   - **Assinatura**: Selecione sua assinatura
   - **Grupo de recursos**: Criar novo ou usar existente
   - **Nome do banco de dados**: Digite um nome único
   - **Servidor**: Criar novo servidor ou usar existente

4. **Configuração do Servidor**
   - **Nome do servidor**: Nome único globalmente
   - **Localização**: Escolha a região mais próxima
   - **Método de autenticação**: SQL Authentication ou Azure AD
   - **Login do administrador**: Defina usuário e senha

5. **Configuração de Computação e Armazenamento**
   - Escolha o modelo de preços (Basic, Standard, Premium)
   - Configure vCores, armazenamento e backup

#### 2.2 Azure SQL Managed Instance

1. **Criar Managed Instance**
   - No Azure Portal, procure por "SQL Managed Instance"
   - Clique em "Criar"

2. **Configurações**
   - **Nome da instância**: Nome único
   - **Região**: Selecione a localização
   - **Tipo de computação**: General Purpose ou Business Critical
   - **Geração de hardware**: Gen4 ou Gen5

3. **Rede**
   - Configure VNet e Subnet
   - Defina configurações de segurança

## 📝 Resumos das Aulas

### Aula 1: Introdução aos Serviços de Banco de Dados do Azure

**Principais Conceitos:**
- Diferenças entre SQL Database, SQL Managed Instance e SQL Server em VMs
- Modelos de preços e escalabilidade
- Recursos de alta disponibilidade e recuperação de desastres

**Pontos Importantes:**
- SQL Database é ideal para aplicações modernas em nuvem
- Managed Instance oferece maior compatibilidade com SQL Server on-premises
- Backup automático e point-in-time restore incluídos

### Aula 2: Configuração Prática

**Processo Aprendido:**
- Navegação no Azure Portal
- Criação step-by-step de instâncias
- Configuração de firewall e regras de acesso
- String de conexão e testes de conectividade

## 💡 Dicas e Boas Práticas

### Segurança
- ✅ Sempre configure regras de firewall restritivas
- ✅ Use Azure AD Authentication quando possível
- ✅ Implemente Transparent Data Encryption (TDE)
- ✅ Configure auditoria e monitoramento

### Performance
- ✅ Escolha o tier de serviço adequado para sua carga de trabalho
- ✅ Configure índices apropriados
- ✅ Use Query Performance Insight para monitoramento
- ✅ Implemente connection pooling nas aplicações

### Custos
- ✅ Use Reserved Capacity para economizar em cargas estáveis
- ✅ Configure Auto-pause para databases de desenvolvimento
- ✅ Monitore o uso com Azure Cost Management
- ✅ Considere Elastic Pools para múltiplos databases

## 🔍 Troubleshooting

### Problemas Comuns

#### Erro de Conectividade
**Sintoma:** Não consegue conectar ao banco
**Solução:**
1. Verificar regras de firewall
2. Confirmar string de conexão
3. Validar credenciais de autenticação

#### Performance Lenta
**Sintoma:** Queries demoradas
**Solução:**
1. Analisar Query Performance Insight
2. Verificar índices faltantes
3. Considerar upgrade do tier de serviço

## 📊 Monitoramento e Métricas

### Métricas Importantes
- **CPU Percentage**: Uso de CPU da instância
- **Data IO Percentage**: Utilização de I/O de dados
- **Log IO Percentage**: Utilização de I/O de log
- **DTU Percentage**: Unidades de transação de banco de dados usadas

### Ferramentas de Monitoramento
- Azure Monitor
- SQL Analytics
- Query Performance Insight
- Azure SQL Database Advisor

## 🔗 Recursos Úteis

### Documentação Oficial Microsoft
- [Azure SQL Database Documentation](https://docs.microsoft.com/azure/sql-database/)
- [SQL Managed Instance Documentation](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [Azure SQL Best Practices](https://docs.microsoft.com/azure/sql-database/sql-database-best-practices)

### Ferramentas
- [Azure Portal](https://portal.azure.com)
- [Azure Data Studio](https://docs.microsoft.com/sql/azure-data-studio/)
- [SQL Server Management Studio](https://docs.microsoft.com/sql/ssms/)

### Tutoriais e Guias
- [Quickstart: Create Azure SQL Database](https://docs.microsoft.com/azure/sql-database/sql-database-single-database-get-started)
- [Connect and query Azure SQL Database](https://docs.microsoft.com/azure/sql-database/sql-database-connect-query)

## 🎓 Certificações Relacionadas

- **AZ-900**: Microsoft Azure Fundamentals
- **DP-900**: Microsoft Azure Data Fundamentals
- **AZ-104**: Microsoft Azure Administrator
- **DP-300**: Administering Relational Databases on Microsoft Azure

## 🏆 Resultados e Aprendizados

### O que foi alcançado:
- ✅ Configuração bem-sucedida de instância SQL Database
- ✅ Compreensão dos diferentes tiers de serviço
- ✅ Implementação de boas práticas de segurança
- ✅ Documentação completa do processo

### Próximos Passos:
- [ ] Implementar backup e restore strategies
- [ ] Configurar replicação geográfica
- [ ] Explorar Elastic Pools
- [ ] Integrar com aplicações

## 👨‍💻 Autor

**Allyson Araújo**
- GitHub: [@AllysonAraujo](https://github.com/AllysonAraujo)
- LinkedIn: [Allyson Araújo](https://linkedin.com/in/allysonaraujo)

### 📌 Nota sobre o Desafio DIO

Este repositório foi criado como parte do desafio "Configurando uma Instância de Banco de Dados na Azure" da Digital Innovation One (DIO). O objetivo é documentar o aprendizado e servir como material de apoio para estudos futuros sobre banco de dados em nuvem.
 
**Curso:** Trilha Azure - DIO  
**Instrutor:** Valéria 

---

⭐ Se este repositório te ajudou, não esqueça de dar uma estrela!
