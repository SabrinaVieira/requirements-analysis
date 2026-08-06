# Projeto Eventus - Especificação de Requisitos

## Ferramenta de GenAI Utilizada
Para a realização desta atividade, foi utilizada a ferramenta **Google Gemini** (acessada de forma direta e complementada por integrações de API mencionadas ao longo do processo).

## Como a IA apoiou as diferentes etapas da atividade
A Inteligência Artificial atuou como uma assistente de Engenharia de Requisitos prestando apoio nas seguintes etapas:
1. **Análise Inicial:** Processou o documento bruto de elicitação (entrevistas e observações) para extrair e classificar Requisitos Funcionais, Não Funcionais, Regras de Negócio e Pendências.
2. **Estratégia de Artefatos:** Apoiou a tomada de decisão sobre quais documentos seriam mais eficientes para o projeto, ponderando entre abordagens tradicionais e ágeis.
3. **Elaboração de Histórias de Usuário:** Ajudou a redigir as US e a embutir os requisitos e regras de negócio diretamente dentro dos critérios de aceitação, garantindo consolidação.
4. **Prototipação:** Estruturou descrições detalhadas (wireframes textuais) para orientar o desenho das telas principais do sistema.
5. **Rastreabilidade e Validação:** Criou a Matriz de Rastreabilidade, cruzando os pedidos originais da elicitação com os artefatos gerados, e forneceu prompts técnicos (código Mermaid) para geração de fluxogramas.

## Sugestões Aceitas
* A utilização de **Histórias de Usuário (User Stories)** como artefato principal para concentrar requisitos e regras de negócio.
* A criação de **Wireframes** para resolver a necessidade dos usuários de "visualizar os eventos em um único lugar" de forma clara e objetiva.
* A elaboração da **Matriz de Rastreabilidade** para comprovar que nenhuma solicitação dos stakeholders foi deixada de lado.
* O uso de fluxogramas de processos para detalhar as regras mais confusas (fila de espera e regras financeiras).

## Sugestões Descartadas ou Modificadas e Justificativas
* **Descartada:** A sugestão (proveniente da ferramenta paralela "Continue") de criar uma vasta gama de documentos separados (Documento de RF, Documento de RNF, Documento de Regras de Negócio, Diagrama ER, etc.).
  * *Justificativa:* Foi avaliado que essa abordagem geraria redundância, excesso de burocracia e sobrecarga no projeto. É muito mais eficiente consolidar as regras dentro dos Critérios de Aceitação das histórias.
* **Modificada:** A sugestão inicial de abandonar totalmente a criação de arquivos de texto em prol do uso de ferramentas de gestão ágil (como Jira/Trello).
  * *Justificativa:* Como o exercício exige a entrega de um repositório físico com a pasta `especificacao/`, a abordagem foi adaptada. Criamos arquivos consolidados (ex: `01_Historias_de_Usuario.md`) que simulam a dinâmica dos tickets ágeis dentro de documentos estáticos, respeitando os requisitos acadêmicos da entrega.

## Por que os artefatos escolhidos foram considerados os mais adequados para esse projeto
O Sistema de Gestão de Eventos possui múltiplos perfis de acesso (Participante, Organizador, Financeiro, Palestrante) com necessidades práticas e diretas.
* **Histórias de Usuário (com Critérios de Aceitação):** São ideais porque traduzem exatamente a "voz do usuário" capturada nas entrevistas ("Como participante, quero..."). Elas facilitam o entendimento tanto do cliente final quanto da equipe de desenvolvimento, amarrando as regras de negócio à funcionalidade prática.
* **Protótipos (Wireframes):** Atendem diretamente à preocupação do participante com a usabilidade e visualização. Um rascunho de tela resolve possíveis ambiguidades de layout muito mais rápido que um longo documento de texto.
* **Fluxos de Processo:** São fundamentais para elucidar a lógica sequencial do sistema em momentos críticos, como o disparo da fila de espera automática e a validação de pagamento.
* **Matriz de Rastreabilidade:** Demonstra profissionalismo e controle, permitindo identificar visualmente o que já está "Definido" e o que está "Pendente de Esclarecimento" (as pontas soltas da elicitação original).
