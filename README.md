# 🧾 Sistema de Gestão de Estoque para Pequenos Negócios

> **Versão:** 1.0  
> **Data:** Outubro de 2025  
> **Autores:** Aylla Christinne Feitosa Rodrigues, Bruno Ataídes Ferreira, Fernanda Cordeiro dos Santos Ferreira, Júlio César Freitas Bueno de Moraes, Lucas Lacerda da Silva, Paulo Henrique Santos Lima  

---

## 📘 Sumário

- [1. Visão Geral](#-1-visão-geral)
- [2. Escopo do Sistema](#-2-escopo-do-sistema)
- [3. Requisitos Funcionais](#-3-requisitos-funcionais)
- [4. Requisitos Não Funcionais](#-4-requisitos-não-funcionais)
- [5. Histórias de Usuário](#-5-histórias-de-usuário)
- [6. Business Model Canvas (BMC)](#-6-business-model-canvas-bmc)
- [7. Arquitetura — Modelo C4](#-7-arquitetura--modelo-c4)

---

## 📘 1. Visão Geral

O **Sistema de Gestão de Estoque (SGE)** tem como objetivo **digitalizar e organizar o controle de estoque** de pequenos comerciantes e empreendedores informais, reduzindo perdas e aumentando a eficiência operacional.

### 🎯 Objetivos
- Reduzir **10% dos custos** associados à perda de produtos vencidos.  
- Melhorar a **competitividade** dos pequenos negócios.  
- Controlar o **fluxo de caixa e movimentação de estoque** via dashboards.  
- Permitir **acesso multiplataforma (web e mobile)**.  

### 🚀 Benefícios
- Diminuição de desperdícios por validade.  
- Relatórios e alertas automatizados.  
- Interface simples e intuitiva.  
- Acesso remoto seguro e em tempo real.  

---

## 🧩 2. Escopo do Sistema

### Produto
Um **Sistema de Gestão de Estoque multiplataforma**, voltado para micro e pequenos empreendedores, com alertas automáticos, relatórios e controle detalhado de produtos.

### Público-Alvo
- Pequenos comerciantes  
- Prestadores de serviços  
- Empreendedores informais  

### Benefícios Esperados
- Redução de perdas por vencimento.  
- Controle centralizado de estoque e finanças.  
- Interface intuitiva e responsiva.  
- Disponibilidade web e mobile.

---

## ⚙️ 3. Requisitos Funcionais

| Código | Descrição | Justificativa |
|--------|------------|----------------|
| **HU1** | Cadastro detalhado de produtos (nome, validade, quantidade). | Evitar venda de produtos vencidos. |
| **HU2** | Controle de movimentações (entradas e saídas). | Acompanhar o fluxo e detectar discrepâncias. |
| **HU3** | Alertas automáticos de validade. | Reduzir perdas financeiras. |
| **HU4** | Notificações de estoque baixo. | Evitar falta de produtos. |
| **HU5** | Relatórios de movimentação e finanças. | Planejamento de capital de giro. |
| **HU6** | Acesso via web e mobile. | Gerenciamento em qualquer lugar. |
| **HU7** | Atualizar/desativar produtos. | Evitar erros e manter dados atualizados. |
| **HU8** | Configurar nível mínimo de estoque. | Automatizar alertas de reposição. |
| **HU9** | Gerenciar dados do usuário (nome, e-mail, senha). | Segurança e personalização. |
| **HU10** | Consultar histórico filtrável de movimentações. | Auditoria e análise. |
| **HU11** | Leitura de código de barras/QR. | Agilidade e redução de erros. |
| **HU12** | Importar/exportar dados (CSV, Excel, PDF). | Integração externa e backup manual. |

---

## 🧱 4. Requisitos Não Funcionais

| Categoria | Descrição |
|------------|------------|
| **Usabilidade** | Interface intuitiva e amigável. |
| **Disponibilidade** | 24/7 com redundância em nuvem. |
| **Segurança** | Criptografia de dados e autenticação segura. |
| **Desempenho** | Resposta < 3s nas operações comuns. |
| **Escalabilidade** | Suporte ao crescimento gradual do negócio. |
| **Compatibilidade** | Suporte a navegadores modernos e dispositivos móveis. |
| **Portabilidade** | Arquitetura web modular (frontend, backend, DB em nuvem). |
| **Manutenibilidade** | Código limpo, modular e documentado. |
| **Confiabilidade** | Backups automáticos e restauração garantida. |
| **Acessibilidade** | Conformidade com padrões W3C e layout responsivo. |

---

## 📝 5. Histórias de Usuário

**HU1 — Cadastro detalhado de produtos**
> **Como** comerciante, **quero** cadastrar produtos informando nome, validade e quantidade, **pois assim** mantenho o estoque organizado e evito vender itens vencidos.

**HU2 — Controle de movimentações de estoque**
> **Como** prestador de serviços, **quero** registrar entradas e saídas de produtos, **de modo que** eu consiga acompanhar o fluxo de mercadorias e identificar discrepâncias rapidamente.

**HU3 — Alertas sobre a validade dos produtos**
> **Como** empreendedor informal, **quero** receber alertas de produtos próximos do vencimento, **pois isso** me ajuda a realizar promoções antecipadas e reduzir perdas financeiras.

**HU4 — Notificação automática de estoque baixo**
> **Como** comerciante, **quero** receber notificações quando o estoque de um produto estiver baixo, **para que** eu faça o pedido de reposição antes de faltar para o cliente.

**HU5 — Relatórios básicos de movimentação e finanças**
> **Como** prestador de serviços, **quero** acessar relatórios de movimentação e finanças, **pois assim** consigo avaliar minhas vendas e planejar melhor o capital de giro.

**HU6 — Acesso multiplataforma ao sistema**
> **Como** empreendedor informal que se desloca entre loja e fornecedores, **quero** acessar o sistema pelo celular ou computador, **de modo que** eu possa gerenciar o estoque em qualquer lugar e tempo.

**HU7 — Atualizar ou desativar produtos**
> **Como** comerciante, **quero** atualizar as informações dos produtos já cadastrados (como nome, validade e quantidade) ou desativá-los quando não estiverem mais disponíveis, **para** manter o estoque sempre correto e evitar erros na venda de itens indisponíveis ou desatualizados.

**HU8 — Configurar o nível mínimo de estoque**
> **Como** comerciante, **quero** definir o nível mínimo de cada produto em estoque, **para que** o sistema consiga emitir alertas de reposição automaticamente e eu não perca vendas por falta de mercadorias.

**HU9 — Gerenciar dados do usuário**
> **Como** prestador de serviços, **quero** atualizar minhas informações de cadastro (como nome, e-mail e senha), **para** manter meus dados seguros e garantir acesso contínuo ao sistema.

**HU10 — Consultar histórico de movimentações**
> **Como** comerciante, **quero** ver o histórico filtrável de entradas/saídas por produto/período/usuário, **para** auditoria e solução de discrepâncias.

**HU11 — Leitura de código de barras/QR**
> **Como** comerciante, **quero** dar entrada/saída usando leitor/câmera, **para** agilizar o processo e reduzir erros.

**HU12 — Exportar e importar dados do estoque**
> **Como** prestador de serviços, **quero** exportar relatórios (PDF/Excel) e importar planilhas (CSV), **para** análise externa e carga inicial rápida.

---

## 💼 6. Business Model Canvas (BMC)

### 📊 Modelo de Negócio — Sistema de Gestão de Estoque

![BMC](https://github.com/pauloh48/prti-projeto-design-software/blob/main/bmc.png)

> 💡 **Resumo Estratégico:** > O sistema visa democratizar o acesso à automação de estoque, oferecendo um produto simples, econômico e escalável, com potencial de expansão via planos pagos e integrações empresariais.

---

## 🧭 7. Arquitetura — Modelo C4

### 🧩 Contexto (texto)

| **Origem** | **Destino** | **Relação** |
| --------------------------------------- | ----------------------------------- | ----------------------------------------------------------------------------- |
| **Pequeno Comerciante** | Sistema de Gestão de Estoque        | Cadastra produtos, consulta estoque e relatórios, e configura níveis mínimos. |
| **Operador/Atendente** | Sistema de Gestão de Estoque        | Registra entradas e saídas de produtos; importa e exporta dados.              |
| **Leitor/Câmera (Código de Barras/QR)** | Sistema de Gestão de Estoque        | Lê códigos para agilizar as movimentações de produtos.                        |
| **Sistema de Gestão de Estoque** | Serviço de Notificações             | Envia alertas automáticos sobre validade e estoque baixo.                     |
| **Sistema de Gestão de Estoque** | Provedor de Nuvem (DB/Storage)      | Persiste dados, armazena arquivos e realiza backups.                          |
| **Sistema de Gestão de Estoque** | Ferramentas Externas (Planilhas/BI) | Exporta relatórios (CSV, Excel, PDF) e importa planilhas para análises.       |


### 🧩 Diagrama de Contexto (PlantUML)

![c4 contexto](https://github.com/pauloh48/prti-projeto-design-software/blob/main/c4/c4_contexto.png)

```plantuml
@startuml
!includeurl [https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Context.puml](https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Context.puml)

' Layout e estilos básicos (opcional)
LAYOUT_LEFT_RIGHT()
SHOW_PERSON_OUTLINE()

' Pessoas
Person(comerciante, "Pequeno Comerciante", "Cadastra produtos, registra movimentações, consulta relatórios e recebe alertas.")
Person(operador, "Operador/Atendente", "Executa entradas/saídas e pode importar/exportar dados.")

' Sistema (caixa central)
System(sge, "Sistema de Gestão de Estoque", "Aplicação Web/Mobile com alertas (validade/estoque baixo), histórico e relatórios.")

' Sistemas/Serviços Externos
System_Ext(cloud, "Provedor de Nuvem (DB/Storage)", "Banco de dados, armazenamento de arquivos e backups.")
System_Ext(notify, "Serviço de Notificações", "E-mail / SMS / Push para alertas.")
System_Ext(sheets, "Ferramentas Externas (Planilhas/BI)", "CSV/Excel/PDF para importação/exportação e análises.")
System_Ext(scanner, "Leitor/Câmera (Código de Barras/QR)", "Dispositivo/feature usado para leitura rápida.")

' Relacionamentos (rotular com verbos claros)
Rel(comerciante, sge, "Cadastra produtos, consulta estoque/relatórios, configura níveis mínimos")
Rel(operador, sge, "Registra entradas/saídas; importa/exp. dados")
Rel(scanner, sge, "Lê códigos para agilizar movimentações")
Rel(sge, notify, "Envia alertas de validade e estoque baixo", "Assíncrono")
Rel(sge, cloud, "Persiste dados e realiza backups")
Rel(sge, sheets, "Exporta CSV/Excel/PDF; importa planilhas")

' (Opcional) Legenda
SHOW_LEGEND()
@enduml
```

### 🧩 Diagrama de Container (PlantUML)
<img width="1348" height="779" alt="diagram-export-04-12-2025-20_34_22" src="https://github.com/user-attachments/assets/2ceebffe-ce57-4366-bcd2-d303729e4264" />

```plantuml
@startuml
!includeurl https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Container.puml
LAYOUT_TOP_DOWN()
SHOW_PERSON_OUTLINE()

' ======================================================
' PERSONAS
' ======================================================
Person(comerciante, "Pequeno Comerciante", "Usa Web e Mobile para gerenciar estoque.")
Person(operador, "Operador/Atendente", "Registra entradas/saídas e gera relatórios.")

' ======================================================
' SISTEMA E CONTAINERS
' ======================================================
System_Boundary(sge, "SGE - Sistema de Gestão de Estoque") {

    Container(webapp, "Web App", "Angular / React",
        "Interface web para cadastro de produtos, movimentações, histórico e relatórios.")

    Container(mobile, "Mobile App", "Flutter / React Native",
        "App móvel para consulta rápida, alertas e leitura de código de barras.")

    Container(api, "API Backend", "Java • Spring Boot",
        "Regras de negócio: produtos, movimentações, alertas, relatórios, exportações.
         Expõe APIs REST e integra com auth, storage, banco e serviço de notificações.")

    Container(auth, "Auth Service", "Spring Security • JWT / OAuth2",
        "Autenticação e autorização. Emite e valida tokens JWT.")

    ContainerDb(db, "Database", "PostgreSQL",
        "Armazena produtos, usuários, alertas e movimentações.
         Dono: API Backend.")

    Container(storage, "File Storage", "S3 / Cloud Storage",
        "Armazena arquivos exportados (CSV, Excel, PDF) e backups.")
}

' ======================================================
' SISTEMAS EXTERNOS
' ======================================================
System_Ext(notify, "Serviço de Notificações", "E-mail / Push / SMS")
System_Ext(scanner, "Leitor de Código de Barras", "Camera/Device Scanner")

' ======================================================
' RELACIONAMENTOS
' ======================================================

' Usuários
Rel(comerciante, webapp, "Usa (HTTPS)")
Rel(operador, webapp, "Usa (HTTPS)")
Rel(comerciante, mobile, "Usa (HTTPS)")
Rel(operador, mobile, "Usa (HTTPS)")

' Apps → API
Rel(webapp, api, "CRUD, relatórios, alertas", "REST/JSON, HTTPS, síncrono + JWT")
Rel(mobile, api, "Movimentações, scanner, alertas", "REST/JSON, HTTPS, síncrono + JWT")

' Autenticação
Rel(webapp, auth, "Login e Refresh Token", "HTTPS, síncrono")
Rel(mobile, auth, "Login e Refresh Token", "HTTPS, síncrono")
Rel(api, auth, "Validação de token JWT", "Local decode / introspection")

' API Interno
Rel(api, db, "Queries / Updates", "JDBC / JPA, síncrono")
Rel(api, storage, "Upload/Download de arquivos", "HTTPS, assíncrono")
Rel(api, notify, "Envio de alertas", "Webhook/SMTP/Push, assíncrono")

' Scanner
Rel(scanner, mobile, "Lê código e envia ao app", "Local API / Hardware Access")

' ======================================================
' CENÁRIOS CRÍTICOS VISUAIS (ANOTAÇÕES)
' ======================================================

' --------- Cenário Feliz
AddNote(webapp, api, 
"CENÁRIO FELIZ\n\nCadastro de Movimentação:\n1. WebApp → API\n2. API → DB\n3. Resposta rápida (<3s).",
"yellow")

AddNote(api, db,
"CENÁRIO FELIZ\nPersistência OK\nRollback em caso de falha.",
"yellow")

' --------- Cenário de Pico
AddNote(api, notify,
"CENÁRIO DE PICO\nEnvio massivo de alertas.\nProcesso assíncrono para evitar travar o usuário.",
"orange")

' --------- Cenário de Falha
AddNote(api, db,
"CENÁRIO DE FALHA\nDB indisponível.\nAPI retorna 503 e aciona alertas internos.",
"red")

' ======================================================
' LEGENDA DE CENÁRIOS
' ======================================================
legend right
<b>Cenários Críticos</b>

<color:yellow>●</color> Cenário Feliz – Cadastro de movimentações  
<color:orange>●</color> Cenário de Pico – Envio massivo de alertas  
<color:red>●</color> Cenário de Falha – DB indisponível  
endlegend

SHOW_LEGEND()
@enduml
```

