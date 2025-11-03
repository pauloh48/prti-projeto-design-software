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
- [5. Business Model Canvas (BMC)](#-5-business-model-canvas-bmc)
- [6. Arquitetura — Modelo C4](#-6-arquitetura--modelo-c4)

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

## 💼 5. Business Model Canvas (BMC)

### 📊 Modelo de Negócio — Sistema de Gestão de Estoque

![BMC](https://github.com/pauloh48/prti-projeto-design-software/blob/main/bmc.png)

> 💡 **Resumo Estratégico:**  
> O sistema visa democratizar o acesso à automação de estoque, oferecendo um produto simples, econômico e escalável, com potencial de expansão via planos pagos e integrações empresariais.

---

## 🧭 6. Arquitetura — Modelo C4

### 🧩 Diagrama de Contexto (PlantUML)

![c4 contexto](https://github.com/pauloh48/prti-projeto-design-software/blob/main/c4/c4_contexto.png)

```plantuml
@startuml
!includeurl https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Context.puml

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

