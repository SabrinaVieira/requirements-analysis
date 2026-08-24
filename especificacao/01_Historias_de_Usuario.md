## Documento: Histórias de Usuário - Sistema Eventus
### US01 - Cancelamento de Inscrição
Ator: Participante
História: Como participante, quero poder cancelar minha inscrição no sistema de forma autônoma, para que eu não precise entrar em contato com a organização.
Critérios de Aceitação:

O sistema deve verificar se o evento específico permite cancelamento (Regra de Negócio). Se não permitir, o botão de cancelar deve ficar inativo e exibir uma mensagem explicativa.

O sistema deve processar o cancelamento imediatamente após a confirmação do usuário.

O sistema deve liberar a vaga automaticamente para a lista de espera (se houver) assim que o cancelamento for concluído.

[Pendente de Definição] O sistema deve validar o prazo limite para cancelamento (ex: até 48h antes do evento).

### US02 - Gestão da Fila de Espera
Ator: Sistema / Organizador
História: Como organizador, quero que o sistema gerencie uma lista de espera automaticamente, para não perder interessados quando um evento lotar.
Critérios de Aceitação:

Assim que o número de inscritos atingir a capacidade máxima definida para o evento, o botão "Inscrever-se" deve mudar para "Entrar na Lista de Espera".

O sistema deve registrar a ordem cronológica exata de entrada na lista de espera.

Se um participante cancelar a inscrição (US01), o sistema deve notificar o primeiro da lista de espera automaticamente para assumir a vaga.

### US03 - Liberação de Inscrição Paga
Ator: Equipe Financeira
História: Como membro da equipe financeira, quero visualizar e confirmar o recebimento de pagamentos, para que o sistema libere a inscrição definitiva do participante.
Critérios de Aceitação:

Para eventos pagos, o status inicial da inscrição do participante deve ser "Aguardando Pagamento".

A equipe financeira deve ter uma tela com a listagem de inscrições pendentes para dar a "Baixa/Confirmação".

Assim que o pagamento for confirmado, o sistema deve mudar o status do participante para "Inscrição Confirmada" e disparar o envio do comprovante.

### US04 - Visualização de Eventos
Ator: Participante
História: Como participante, quero visualizar todos os eventos e workshops disponíveis num único local para que eu possa consultar as opções e escolher facilmente em quais me inscrever.
Critérios de Aceitação:

O sistema deve exibir uma listagem (ou calendário) de todos os eventos ativos organizados pela Eventus.

Cada item da lista deve mostrar informações básicas: título, data, horário, e indicar claramente se é um evento "Gratuito" ou "Pago" (Regra de Negócio).

O sistema deve permitir que o participante acesse esta visualização de forma centralizada a partir do seu painel principal (dashboard).

### US05 - Inscrição e Verificação de Conflito de Horários
Ator: Participante
História: Como participante, quero inscrever-me em múltiplos workshops que acontecem no mesmo dia para que eu possa aproveitar o evento ao máximo, sem que haja conflito entre as minhas atividades.
Critérios de Aceitação:

O sistema deve permitir a seleção e inscrição em mais de um workshop no mesmo dia.

[Regra de Negócio] O sistema deve validar os horários das atividades. Se o participante tentar inscrever-se num workshop cujo horário coincida com o de outra inscrição já realizada, o sistema deve bloquear a ação e apresentar um alerta de conflito de horários.

Imediatamente após a inscrição ser efetivada (ou o pagamento ser confirmado, no caso de eventos pagos), o sistema deve enviar um comprovante ao participante.

[Pendente de Definição] É necessário definir se a vaga é subtraída do total no momento em que o usuário inicia o pagamento ou apenas após a confirmação financeira.

### US06 - Emissão de Certificados
Ator: Participante
História: Como participante, quero conseguir emitir o meu certificado de participação diretamente no sistema após o evento, para que eu possa comprovar a minha presença sem depender da organização.
Critérios de Aceitação:

O sistema deve gerar um certificado digital num formato padronizado e descarregável (como PDF).

A opção de emissão de certificado só deve ficar visível ou ativa para o participante após a data e hora de encerramento do evento.

[Pendente de Definição] O sistema deve verificar a condição para emissão: validar se a liberação será automática após o evento ou se exigirá uma confirmação prévia de presença por parte da organização.

### US07 - Consulta da Lista de Inscritos pelo Palestrante
Ator: Palestrante
História: Como palestrante, quero consultar a lista e a programação com os participantes inscritos nas minhas atividades, para que eu possa conhecer o meu público e preparar-me adequadamente.
Critérios de Aceitação:

O sistema deve permitir que o palestrante visualize apenas a lista de inscritos das atividades às quais ele está formalmente associado.

A lista de participantes deve refletir a quantidade de inscritos em tempo real, atualizando conforme novas inscrições ou cancelamentos ocorram.

[Pendente de Definição] Por questões de privacidade (LGPD), o sistema deverá exibir apenas as informações autorizadas do participante (ex: nome e empresa), necessitando definição de quais dados ficarão visíveis.