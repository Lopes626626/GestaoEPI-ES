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

## 🧪 Ambiente de Teste e Execução
O protótipo funcional foi desenvolvido em Python e está pronto para ser testado.

**Instruções de Uso:**
1. Faça o download do arquivo `Codigo do EPI.ipynb` disponível na raiz deste repositório.
2. Acesse o [Google Colab](https://colab.research.google.com/drive/1ZpWurHFDaMXMgvSkqg68aY5wM8lilnEZ?usp=sharing) e faça o upload do arquivo.
3. O notebook já contém os dados mockados (funcionários e EPIs fictícios).
4. Clique no botão de "Play" (Executar célula) ao lado do bloco de código.
5. Interaja com o menu do sistema respondendo aos prompts de entrada diretamente no terminal inferior do Colab (ex: digite `1` para registrar uma entrega).
6. Caso queira ver o caminho de como fica o resultado do código Python, acesse [aqui](Codigo%20do%20EPI.ipynb)

## 📐 Modelagem UML

### 1. Diagrama de Classes
![Diagrama de Classes UML](docs/Modelagem%20UML.png)

**Descrição:** Representa a estrutura principal de dados e classes do VisioGuard. É composto por três entidades fundamentais: **Funcionario** (dados do colaborador), **EPI** (equipamentos e validade) e **RegistroUso** (a classe que cruza o colaborador com o equipamento utilizado no momento).

### 2. Diagrama de Sequência
![Diagrama de Sequência](docs/Diagrama%20de%20sequencia.png)

**Descrição:** O diagrama acima ilustra o fluxo principal de execução do nosso MVP. Ele demonstra a interação do gestor com o sistema em Python, desde a inicialização (onde alertas automáticos são exibidos) até o passo a passo de inserção de IDs para registrar e validar a entrega de um equipamento.

## 🎨 Protótipo e Identidade Visual (Figma)
Toda a concepção da marca (logo, paleta de cores, tipografia) e a construção inicial das interfaces do VisioGuard foram desenvolvidas no Figma.

🔗 **[Acessar a identidade visual do projeto no Figma](https://www.figma.com/design/gjzCn0fLXneK2Z6N2l9VFR/Checkpoint---ES?node-id=3-19&t=dA5vwTSKBbMjpM50-1)**

- **Nome:** VisioGuard
- **Cores:** 
  - Amarelo Segurança (`#FFCC00`)
  - Azul Marinho (`#003366`)
  - Cinza Claro (`#F4F4F9`)
- **Tipografia:** Pixelify Sans

## 💡 Ideia de Venda e Simulação (Pitch)
**O Diferencial:** O VisioGuard substitui planilhas confusas por um sistema inteligente e acessível. Nossa solução permite que o técnico de segurança saiba exatamente quem está com qual equipamento e quando ele vence, tudo de forma rápida e visual. *VisioGuard: proteção que você pode provar.*


## 📂 Estrutura de Pastas
```text
/
├── docs/
│   ├── Diagrama de sequencia.png
│   └── Modelagem UML.png
├── Codigo do EPI.ipynb
└── README.md
