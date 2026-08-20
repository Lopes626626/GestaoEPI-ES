# VisioGuard 🛡️
**Sistema Inteligente de Gestão de EPIs Industriais**

Projeto desenvolvido para o Checkpoint de Engenharia de Software - FIAP.

## 👥 Equipe
- Rafael Lopes Bestilleiro Benedetti - RM: 554781
- Breno Ferreira e Silva - RM: 555503
- Pedro Gonçalves - RM: 557936

## 📖 Descrição do Problema e Público-Alvo
**Problema:** A falta de controle rigoroso sobre o uso e a validade de Equipamentos de Proteção Individual (EPIs) gera riscos de acidentes e passivos trabalhistas para indústrias. Sistemas atuais dependem de checagens manuais e planilhas desatualizadas.

**Público-alvo:** Técnicos de segurança do trabalho, gestores operacionais e auditores em plantas industriais e linhas de produção.

## ⚙️ Requisitos Funcionais (RF)
- **RF01:** O sistema deve permitir o cadastro, leitura, atualização e exclusão (CRUD) de dados de funcionários e EPIs.
- **RF02:** O sistema deve vincular a entrega de um EPI a um funcionário específico com data e hora.
- **RF03:** O sistema deve gerar alertas quando a validade de um EPI estiver próxima do vencimento.
- **RF04:** O sistema deve gerar relatórios básicos de conformidade de uso por setor.

## 🛠️ Requisitos Não Funcionais (RNF)
- **RNF01:** O desenvolvimento da lógica e manipulação de dados será feito em **Python** utilizando o **Google Colab**.
- **RNF02:** A interface visual inicial será prototipada no **Figma**.
- **RNF03:** O armazenamento temporário de dados no Colab será feito utilizando estruturas de dados do Python (como Dicionários, Listas ou DataFrames do Pandas) ou arquivos CSV.
- **RNF04:** A organização das tarefas e sprints será feita no **Trello**.
- **RNF05:** O versionamento de código e documentação será mantido no **GitHub**.

## 📦 Escopo do Projeto (Primeira Versão)
**O que ENTRA:**
- Lógica de controle de EPIs desenvolvida e documentada no Google Colab.
- Protótipo navegável no Figma contendo o dashboard de gestão.
- Documentação UML (Diagrama de Classes).
- Repositório no GitHub organizado.

**O que FICA DE FORA:**
- Integração de hardware físico.
- Sistemas de banco de dados relacionais complexos em nuvem.

## 📐 Modelagem UML

![Diagrama de Classes UML](docs/Modelagem%20UML.png)

**Descrição da Modelagem:**
O diagrama acima representa a estrutura principal de dados e classes do VisioGuard, refletindo a lógica que será implementada no Python (Google Colab). Ele é composto por três entidades fundamentais:

*   **Funcionario:** Representa o colaborador da indústria, contendo suas informações de identificação (ID, nome, matrícula e setor) e os métodos básicos de cadastro e atualização.
*   **EPI:** Armazena os dados dos equipamentos de proteção, com foco especial na `data_validade` e no `status` (ex: disponível, em uso, descartado), além do método para checar se o equipamento ainda é seguro para uso.
*   **RegistroUso:** É a classe que conecta as duas pontas. Ela registra o momento exato (`data_verificacao`) em que um funcionário (`funcionario_id`) recebe e utiliza um equipamento (`epi_id`). Também armazena se o uso está dentro das regras (`conformidade`) e o impacto daquele registro na segurança geral.

## 🎨 Identidade Visual e Marca
- **Nome:** VisioGuard
- **Cores:** 
  - Amarelo Segurança (`#FFCC00`)
  - Azul Marinho (`#003366`)
  - Cinza Claro (`#F4F4F9`)
- **Tipografia:** Inter ou Roboto

## 💡 Ideia de Venda (Pitch)
**O Diferencial:** O VisioGuard substitui planilhas confusas por um sistema inteligente e acessível. Nossa solução permite que o técnico de segurança saiba exatamente quem está com qual equipamento e quando ele vence, tudo de forma rápida e visual. *VisioGuard: proteção que você pode provar.*

## 📂 Estrutura de Pastas Inicial
```text
/
├── docs/                  
├── src/            
└── README.md
