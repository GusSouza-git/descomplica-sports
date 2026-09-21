# Descomplica Sports

**Descomplica a sua partida.**

Projeto acadêmico da avaliação A3 da disciplina **Projeto e Engenharia de Software**, voltado ao planejamento de um aplicativo de agendamento e gerenciamento de quadras esportivas.

Este repositório reúne a documentação e acompanha a evolução do projeto. As funcionalidades descritas estão sendo especificadas e ainda não representam um aplicativo implementado.

## Documentação

| Documento | Finalidade | Arquivos |
| --- | --- | --- |
| Termo de Abertura | Apresenta o problema, os objetivos e a visão inicial do escopo. | [PDF](docs/termo-de-abertura.pdf) · [Word](docs/termo-de-abertura.docx) |
| Documento de Requisitos | Detalha as regras de negócio, os requisitos funcionais e não funcionais, as prioridades e os critérios de aceite. | [PDF](docs/documento-de-requisitos.pdf) |

O termo de abertura registra a proposta inicial. O documento de requisitos detalha as decisões atuais e os limites da primeira versão.

## Sobre o projeto

O Descomplica Sports propõe um aplicativo que conecta jogadores e proprietários de espaços esportivos, centralizando a busca por quadras, a consulta de horários e a realização de reservas.

## Problema

Os jogadores enfrentam dificuldades para localizar quadras, consultar disponibilidade, avaliar a estrutura dos espaços e confirmar suas reservas.

Os proprietários precisam divulgar seus estabelecimentos, organizar a agenda, evitar conflitos de horários e acompanhar os pagamentos.

## Objetivo

Facilitar a busca e a reserva de quadras esportivas, oferecendo aos jogadores uma experiência organizada e aos proprietários recursos para divulgar e administrar seus espaços.

## Público-alvo

- Pessoas que procuram quadras para praticar esportes.
- Proprietários de espaços esportivos.

## Funcionalidades especificadas

O resumo abaixo segue o documento de requisitos. As prioridades de cada função estão indicadas nos respectivos cartões.

### Conta e acesso

- Criação de contas de jogador e proprietário, com confirmação do e-mail.
- Entrada por e-mail e senha, saída da conta e recuperação de senha.
- Edição dos dados permitidos do perfil.
- Canal para solicitações sobre dados pessoais.

### Busca e reserva

- Busca de quadras por nome, cidade ou bairro, sem uso de GPS na primeira versão.
- Filtros por data, horário e esporte.
- Consulta de endereço, fotos, esportes, períodos disponíveis, preços, contato e avaliações disponíveis.
- Reserva temporária do horário por 10 minutos, com contador visível.
- Pagamento por Pix ou cartão de crédito.
- Consulta das próprias reservas e da situação dos pagamentos.
- Avaliação da quadra após a conclusão da reserva, como recurso de prioridade *could*.

### Gestão do proprietário

- Cadastro do espaço e das quadras, com períodos reserváveis e preços.
- Atualização das informações das quadras.
- Consulta da agenda e bloqueio ou liberação de períodos sem reservas ativas.
- Acompanhamento dos pagamentos, das devoluções previstas e do total recebido.

## Regras centrais da reserva

- O primeiro pedido aceito e registrado pelo sistema obtém a reserva temporária do período.
- O horário fica indisponível para outros jogadores durante os 10 minutos da reserva temporária.
- A aprovação do pagamento deve ser recebida antes da expiração para confirmar a reserva.
- Uma aprovação recebida no instante da expiração ou depois dele não confirma a reserva e gera uma solicitação de devolução integral.
- Uma reserva confirmada passa a concluída ao atingir o horário de término.

## Qualidade e operação

Os requisitos não funcionais tratam de desempenho, segurança, usabilidade, disponibilidade, compatibilidade com celulares Android e iOS, privacidade, auditoria, backup e recuperação, além de acessibilidade.

As metas numéricas registradas no documento são propostas de projeto a validar antes de uma implantação.

## Limites da primeira versão

O documento de requisitos mantém fora da primeira versão o bate-papo, o cancelamento e a remarcação pelo aplicativo, a formação de times e a confirmação de presença do grupo.

O termo de abertura também apresenta possíveis evoluções, como ranking, estatísticas dos jogadores, sistema de amigos e torneios.

### Pontos de alinhamento entre os documentos

Login com Google e Apple, favoritos, formas de pagamento salvas e preferências de notificações aparecem na visão inicial do termo de abertura, mas ainda não têm requisitos próprios na especificação atual. Esses itens precisam ter seu detalhamento e sua prioridade definidos nas próximas revisões.

## Próximas etapas

- Elaborar os diagramas UML com base nos requisitos.
- Detalhar as telas e os fluxos de navegação.
- Preparar a apresentação do projeto.
- Desenvolver, ao final do planejamento, um demonstrativo navegável com dados e pagamentos simulados.

O desenvolvimento em código não é uma exigência desta etapa acadêmica. O demonstrativo está planejado como apoio à apresentação.
