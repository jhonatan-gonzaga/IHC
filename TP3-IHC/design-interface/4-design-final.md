# Design Final

Nesta seção, apresentamos a evolução final da interface do Conecta Obra Itacoatiara, consolidando os fluxos de tarefas e wireframes desenvolvidos anteriormente em uma solução de alta fidelidade. O objetivo principal deste design é materializar uma plataforma que atue como um diretório digital eficiente para a construção civil, conectando clientes, profissionais e lojistas de forma ágil e segura.

# Telas para a Persona de Profissional

## Telas de Oportunidades

<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/2cdb4bc1-075e-4851-a90d-83bc01cc0120" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/2dbd40b8-12e7-4367-84b7-cd6b78128d2c" />
</p>
</p>

**1. Estrutura Global e Navegação**
- Cabeçalho (Header): A área superior é fixa e limpa, contendo um botão de navegação "voltar" (seta à esquerda), o logotipo da marca centralizado para reforço de identidade e a foto de perfil do usuário à direita, criando um ponto de ancoragem visual familiar.
- Barra de Navegação Inferior (Bottom Bar): A navegação principal do aplicativo é feita por uma barra inferior fixa com três ícones claros: "Oportunidades" (ícone de martelo, indicando a tela ativa em vermelho), "Meus Projetos" (ícone de prancheta) e "configuração" (ícone de engrenagem).
- Navegação em Abas (Tabs): Logo abaixo do cabeçalho, o fluxo de trabalho é dividido em duas abas principais: "Novos Pedidos" e "Meus Serviços". A aba ativa é sublinhada em vermelho, e a aba de pedidos possui um badge numérico (elipse vermelha com o número "2") para alertar sobre novas solicitações pendentes.

**2. Design dos Cards (Cartões de Informação)**
   
O conteúdo é organizado em Cards brancos com bordas arredondadas e um contorno sutil em vermelho/rosa, destacando-se sobre o fundo claro da aplicação. A hierarquia da informação dentro do card é:

- Título: O tipo de serviço (ex: "Pintura Residencial") aparece em negrito e tamanho maior no topo esquerdo.
- Metadados: Informações de contexto são apresentadas com ícones vermelhos lineares (outlined) seguidos de texto cinza: um ícone de "Pin" para localização (ex: Centro) e um ícone de "Calendário" para a data (ex: 04 de dez.).
- Descrição: Um breve descritivo do serviço aparece logo abaixo (ex: "Pintura completa de casa de 3 quartos").

**3. Interatividade e Estados**

O design adapta os elementos interativos conforme o contexto da aba:
- Tela "Novos Pedidos": Foca na tomada de decisão rápida. Apresenta dois botões grandes lado a lado: "Aceitar" (preenchimento sólido vermelho, indicando ação primária) e "Recursar" (fundo branco com borda vermelha, indicando ação secundária).
- Tela "Meus Serviços": Foca no gerenciamento.
  - dentificação de Status: Utiliza Tags (etiquetas) coloridas no canto superior direito do card: Verde para "Concluído" e Azul marinho para "Em Andamento".
  - Ações de Execução: Para serviços em andamento, os botões mudam para "falar no WhatsApp" (com ícone social integrado) e "Finalizar".
---

  ## Telas de Meu Projetos 
<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/c0dc771c-8fdd-4093-a186-0a2d20f86329" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/673e4107-6531-4c62-ae32-04593f8dde0b" />
</p>
</p>


O fluxo de gestão de portfólio foi desenhado para ser visualmente rico e exigir o mínimo de esforço de digitação.

1. Lista de Projetos: A tela principal ("Meus Projetos") destaca um botão de ação primária (+ Adicionar Novo Projeto) no topo, garantindo alta visibilidade. A lista de trabalhos realizados é apresentada em cards horizontais que priorizam a foto da obra, seguidos pelo título e local, permitindo rápida identificação visual.

2. Cadastro de Novo Projeto: A tela de inclusão substitui formulários longos por interações táteis. O destaque principal é a área de mídia: um botão massivo para "Tirar foto Agora" ocupa o terço superior da tela, incentivando o registro imediato da obra. A seleção de categorias é feita através de chips (botões de tag) e o campo de descrição inclui um recurso de entrada de voz (microfone) para facilitar o preenchimento.

   ---
## Tela de Perfil do Profissional
 <p align="center">
   <img width="413" height="1328" alt="image" src="https://github.com/user-attachments/assets/f5fa3599-929c-4170-8770-d7c4e0bb325f" />
</p>
A tela de edição de perfil consolida a gestão de identidade e reputação em uma única interface vertical e rolável (scrollable).

1. Gestão de Imagem e Reputação: O topo apresenta a foto de perfil em destaque com um botão de edição direta. Logo abaixo, um cartão de destaque exibe a nota média (4.0) e as estrelas de avaliação, seguido por uma lista horizontal (carousel) de "Avaliações Recentes", permitindo que o profissional leia e responda ao feedback de clientes sem sair da tela de edição.
2. Formulário de Dados Profissionais: A edição de informações utiliza componentes visuais interativos para agilizar o preenchimento. A seleção de "Especialidades" (ex: Pedreiro, Pintor) e "Disponibilidade" (dias da semana) é feita através de botões de alternância (toggle chips e botões circulares), onde o usuário apenas toca para ativar ou desativar, eliminando a necessidade de listas suspensas complexas ou digitação.
3. Definição de Valor e Horário: Campos numéricos simples definem o intervalo de horário de trabalho ("Das" / "Até") e o "Valor da Diária", finalizando com um botão de ação persistente "Salvar Perfil" na base da tela.

## Tela da Caixa de Mensagem
<img width="234" height="519" alt="image" src="https://github.com/user-attachments/assets/ecadb73c-3c33-4505-aca0-7a9d34513567" />
<img width="237" height="521" alt="image" src="https://github.com/user-attachments/assets/d101f585-0b34-468e-84ab-fc0069b5da3b" />


