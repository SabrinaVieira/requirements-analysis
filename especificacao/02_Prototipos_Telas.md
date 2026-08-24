## Documento: Protótipos de Ecrã (Wireframes Textuais) - Sistema Eventus
Abaixo estão as descrições de interface (de cima para baixo, da esquerda para a direita) para os três ecrãs principais do sistema.

## 1. Ecrã: Dashboard do Participante (Explorar Eventos)
**Objetivo:** Permitir ao participante ver todos os eventos num único local e acompanhar as suas inscrições ativas.

- **CABEÇALHO (Topo, a toda a largura):**

- [Esquerda] Logótipo "Eventus".
- [Direita] Ícone de Notificações (Sino) e Foto/Nome do Perfil do Utilizador com menu dropdown (Definições, Terminar Sessão).
- **MENU LATERAL (Esquerda, fixo):**

- [Link Ativo] Explorar Eventos
- [Link] As Minhas Inscrições
- [Link] Os Meus Certificados
- **ÁREA PRINCIPAL (Centro/Direita, área de conteúdo):**

- **Barra de Pesquisa e Filtros (Topo da área principal):**

- [Campo de Texto] "Pesquisar por nome do evento ou workshop..."
- [Filtros Dropdown] "Data", "Tipo (Gratuito / Pago)".
- **Secção: Destaques / Próximos Eventos:**

- [Grelha de Cartões (Cards)] Cada cartão representa um evento e contém:

- *Imagem/Cor de capa do evento.*
- *Título do Evento.*
- *Data e Horário.*
- *Etiqueta (Tag):* [Gratuito] ou [Pago].
- *[Botão Primário]* "Ver Detalhes".
- **Secção: As Minhas Inscrições Brevemente:**

- [Lista Rápida] Mostra 2 ou 3 eventos em que o utilizador já está inscrito com o estado (Ex: "Inscrição Confirmada" ou "Aguardando Pagamento").

### 2. Ecrã: Inscrição e Detalhes do Evento/Workshop
**Objetivo:** Apresentar a informação detalhada de um evento específico, tratar vagas/lista de espera e alertar sobre conflitos de horário.

- **CABEÇALHO (Topo):** Idêntico ao do Dashboard.
- **NAVEGAÇÃO SECUNDÁRIA:**

- [Link/Breadcrumb] "< Voltar para Explorar Eventos".
- **ÁREA PRINCIPAL (Esquerda - 70% do ecrã):**

- [Título Grande] Nome do Evento/Workshop.
- [Bloco de Informação] Data, Horário de Início/Fim e Local (ou link da transmissão).
- [Caixa de Texto] Descrição detalhada sobre o que será abordado, palestrantes envolvidos e cronograma.
- **PAINEL LATERAL DE AÇÃO (Direita - 30% do ecrã, fixo):**

- [Caixa de Resumo Financeiro] Preço do evento (ou indicação de "Gratuito").
- [Etiqueta de Vagas] Ex: "🟢 Vagas Disponíveis: 15" ou "🔴 Evento Esgotado".
- *[Alerta Condicional - Visível apenas se houver conflito]:* [Caixa Amarela de Aviso] "Atenção: Já está inscrito noutro workshop neste mesmo horário."
- **[Botão Principal de Ação - Condicional]:**

- *Cenário A (Com Vagas):* Botão Verde [Inscrever-me].
- *Cenário B (Sem Vagas):* Botão Laranja [Entrar na Lista de Espera].
- [Link pequeno abaixo do botão] "Ler política de cancelamento".

### 3. Ecrã: Painel do Palestrante (Consulta de Inscritos)
**Objetivo:** Permitir que o palestrante consulte quem está inscrito nas suas atividades respeitando regras de privacidade.

- **CABEÇALHO (Topo):**

- [Esquerda] Logótipo "Eventus" | [Etiqueta] "Portal do Palestrante".
- [Direita] Foto/Nome do Palestrante.
- **ÁREA PRINCIPAL (Centro, ocupando todo o ecrã):**

- [Título] "As Minhas Atividades".
- **Barra de Controlo (Topo da área principal):**

- [Filtro Dropdown] "Selecionar Workshop:" (Lista apenas as atividades vinculadas a este palestrante).
- [Caixa de Estatística 1] Total de Inscritos Confirmados (Ex: 45/50).
- [Caixa de Estatística 2] Pessoas na Lista de Espera (Ex: 12).
- **Tabela de Participantes (Centro):**

- *Cabeçalho da Tabela:* | Nome do Participante | Empresa/Organização | Estado da Inscrição |
- *Linhas da Tabela:* Dados dos participantes. (Nota de Privacidade: E-mail e telefone ocultados conforme regras LGPD).
- **Rodapé da Tabela (Direita):**

- *[Botão Secundário]* "Descarregar Lista (PDF)".
- *[Botão Secundário]* "Descarregar Lista (Excel)".