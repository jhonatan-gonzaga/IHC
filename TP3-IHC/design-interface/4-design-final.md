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

# Telas para a Persona de Lojista

## Tela do Perfil Loja

<p align="center">
   <img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/2d15e453-8439-465f-ab25-ece42befb61c" />
</p>

A tela de "Perfil Loja" atua como um painel de controle administrativo (dashboard) para o parceiro comercial, consolidando a edição de dados institucionais e o gerenciamento ativo de estoque e ofertas em uma interface centralizada.

1. Gestão Institucional: O topo da tela oferece acesso direto à manutenção da identidade da loja através do botão "Editar Perfil". Logo abaixo, os campos informativos (horário, segmento, localização e contato) servem como um resumo visual dos dados cadastrados, permitindo ao lojista conferir rapidamente as informações que estão visíveis para o cliente final.
2. Administração do Catálogo: A seção central facilita a expansão e o controle do mix de produtos. O botão de destaque "+ Adicionar Produto" agiliza a inserção de novos itens, enquanto a listagem em cartões (cards) apresenta o preço e a quantidade atual, permitindo o monitoramento do estoque disponível.
3. Controle de Promoções: A seção inferior é dedicada à estratégia de vendas, com um botão específico "+ Adicionar Promoção" para criar ofertas rapidamente. Os cartões diferenciam-se visualmente ao destacar o percentual de desconto (ex: "20% OFF") em vez do preço cheio, permitindo ao gestor administrar separadamente o inventário destinado a campanhas promocionais.

## Tela de Adicionar Produto e Adicionar Promção

<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/d983555a-0cb3-4beb-a81d-96a88a1e1278" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/e30f6e15-489b-4a68-8afa-4ba94e24fa7a" />
</p>
</p>

As interfaces de entrada de dados foram projetadas com um padrão de design unificado, garantindo que o lojista tenha uma experiência familiar tanto ao cadastrar um novo item quanto ao criar uma oferta relâmpago. A consistência visual reduz a carga cognitiva e agiliza a operação.

1. Padronização de Formulários: Ambas as telas priorizam a legibilidade com o campo "Nome Produto" em destaque no topo, seguido por uma grande área de texto para "Detalhes". Essa estrutura mantida assegura que o usuário não precise reaprender a interface ao alternar entre tarefas de estoque e marketing.

2. Adaptação Contextual de Campos: A diferenciação funcional ocorre na segunda linha de inputs. Enquanto a tela de Produto solicita o valor monetário absoluto ("Preço"), a tela de Promoção adapta-se para capturar a estratégia de desconto ("Promoção %"), mantendo o campo "Quantidade" inalterado para controle de estoque em ambos os cenários.

3. Foco na Ação: O layout limpo direciona o olhar para o botão de ação primária "Adicionar" (em vermelho). O posicionamento isolado na base da tela evita cliques acidentais e fornece um encerramento claro para o fluxo de cadastro.

## Tela de Lista Catálogo e Lista Promoção

<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/6e7106c6-5f4e-4651-8f90-acf4601a70c7" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/160b727a-3fbb-4f31-b47d-35ea88fb3268" />
</p>
</p>

As telas de listagem foram construídas sobre um sistema de cartões (cards) padronizado, permitindo que o lojista navegue por grandes volumes de itens (seja do catálogo regular ou de ofertas) com a mesma fluidez e carga cognitiva reduzida.

1. Arquitetura de Informação em Cards: A escolha por cartões individuais, delimitados por bordas sutis e espaçamento generoso, melhora a "escaneabilidade" da tela. Cada unidade de informação é isolada, evitando que os dados de um produto se confundam visualmente com o próximo, o que é essencial em listas longas de rolagem vertical.
2. Hierarquia de Dados: Em ambas as variações, o "Nome do Produto" recebe o peso visual primário no topo do cartão. Logo abaixo, a interface divide a atenção entre o atributo financeiro (esquerda) e logístico (direita - "Quantidade"), finalizando com metadados de descrição (ex: "Marca Leopoldo, 2025") no rodapé do cartão para contexto adicional.
3. Variação Funcional de Atributos: A distinção entre as telas ocorre no dado crítico de decisão:

- Catálogo Padrão: Exibe o campo "Preço" (R$), permitindo a conferência do valor de venda regular.
- Lista Promocional: Substitui o preço pelo campo "Desconto/Promoção" (%), destacando o impacto da oferta em vez do valor monetário final, facilitando a gestão da agressividade das campanhas de marketing.

## Tela de Edição

 <p align="center">
   <img width="413" height="1328" alt="image" src="https://github.com/user-attachments/assets/3d39aa92-b4a2-4676-b2e9-13621f6f3ea4" />
</p>

1. Ações Rápidas nos Cartões: A principal evolução de UX nesta tela é a introdução de ícones de ação no cabeçalho de cada cartão de produto.

- Ícone Lápis (Editar): Permite o ajuste imediato de preços, quantidades ou descrições, ideal para correções rápidas de inventário.
- Ícone Lixeira (Excluir): Oferece um caminho rápido para a descontinuação de produtos ou encerramento de ofertas, mantendo a lista sempre atualizada.
2. Consistência entre Seções: A funcionalidade de edição é aplicada simetricamente tanto na seção "Catálogo" quanto em "Promoções". Isso cria um modelo mental consistente para o usuário: independentemente de estar gerenciando um produto regular ou uma oferta sazonal, as ferramentas de controle (editar/excluir) estão posicionadas no mesmo local visual (canto superior direito do card).
3. Persistência Global: Diferente da visualização passiva, esta tela encerra-se com um botão de ação primária "Salvar Alterações" fixado no rodapé. Isso indica que as modificações (como alterações de telefone no topo ou exclusão de itens no meio) podem ser revisadas em lote antes da confirmação final, prevenindo erros operacionais acidentais.

## Tela da Caixa de Mensagem e CHAT entre Lojista e Clientes
<img width="233" height="521" alt="image" src="https://github.com/user-attachments/assets/19e8ba04-e6b9-404d-835f-dcd6a9759563" />
<img width="237" height="521" alt="image" src="https://github.com/user-attachments/assets/d101f585-0b34-468e-84ab-fc0069b5da3b" />

## Tela de Caixa de Mensagens

A tela de Caixa de Mensagens foi projetada para oferecer uma visão clara e imediata das conversas ativas, priorizando rapidez de acesso e simplicidade visual.

### 1. Estrutura e Navegação

Cabeçalho (Header): Localizado no topo, apresenta o título “Caixa de Mensagem” em destaque, acompanhado de um botão de retorno (seta à esquerda), garantindo orientação espacial ao usuário dentro do fluxo do aplicativo.
Lista de Conversas: O conteúdo principal é organizado em uma lista vertical limpa, com cada conversa representada por um item único. No estado atual, a conversa com “Cliente” aparece como elemento prioritário.
Barra de Navegação Inferior: Mantém consistência com o restante do aplicativo, apresentando os ícones de Chat, Caixa (ativo) e Loja, reforçando a hierarquia e continuidade da navegação global.

### 2. Design do Item de Conversa 

Avatar do Usuário: Um ícone circular com silhueta padrão identifica visualmente o interlocutor.
Nome e Ação: O nome “Cliente” aparece em tipografia de maior peso, acompanhado do texto auxiliar “Toque para conversar”, orientando claramente a ação esperada.
Indicador de Mensagens Não Lidas: Um badge numérico discreto sinaliza a existência de novas mensagens, chamando atenção sem gerar poluição visual.


### 3. Experiência do Usuário 

A tela funciona como um ponto de entrada direto para a comunicação, reduzindo fricção e permitindo que o profissional acesse rapidamente solicitações ou atualizações importantes.

## Tela de Chat (Conversa Ativa)

A tela de Chat individual foca na comunicação direta e contínua entre o profissional e o cliente, com ênfase na legibilidade e na facilidade de interação.

### 1. Estrutura Geral

Cabeçalho: Exibe o título “CHAT” de forma centralizada, com botão de retorno à esquerda, mantendo consistência com o padrão de navegação do aplicativo.
Identificação do Interlocutor: Logo abaixo do cabeçalho, o avatar e o nome “Cliente” reforçam visualmente com quem a conversa está sendo realizada, evitando ambiguidades.

### 2. Área de Conversação

Plano de Fundo Suave: O fundo em tom claro e neutro reduz distrações e favorece a leitura das mensagens.
Fluxo Vertical: As mensagens são organizadas em um fluxo vertical natural, preparado para crescimento conforme a conversa evolui.

### 3. Campo de Entrada e Ações

Input de Mensagem: Localizado na base da tela, com placeholder “Informar mensagem…”, claramente indicando o local de interação.
Ações Complementares: Ícone de microfone permite entrada por voz, enquanto o botão de envio destacado garante rapidez no envio da mensagem, favorecendo comunicações dinâmicas.


### 4. Usabilidade 

A disposição dos elementos prioriza o uso com uma mão, comum em dispositivos móveis, e assegura que a comunicação ocorra de maneira fluida, intuitiva e sem barreiras cognitivas.

---

# Telas para a Persona de Cliente

## Tela de Listagem de Lojas e Serviços 

<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/de945cba-c3bf-4028-8161-cf901e39cde1" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/771231f3-9990-44ff-8d4b-46a115e66827" />
</p>
</p>

## Aba "Abertas Agora"

Esta tela atua como a porta de entrada para o comércio local, funcionando como um catálogo centralizado de parceiros.

### 1. Diretório Geolocalizado:

No topo, a identificação do bairro ("Centro") assegura que o cliente está visualizando opções relevantes para a sua região, otimizando a logística de entrega.

### 2. Busca e Filtragem Imediata:

A barra de busca permite encontrar itens específicos rapidamente, enquanto o filtro "Abertas Agora" resolve uma necessidade crítica da obra: a urgência. O usuário consegue separar imediatamente quais fornecedores podem atender sua demanda naquele exato momento.

### 3. Cards de Decisão Rápida:

A listagem das lojas foi desenhada para fornecer todas as informações logísticas antes do clique. Cada card apresenta o nome do estabelecimento, a categoria (ex: Atacarejo, Loja de Bairro), a distância, o tempo estimado de entrega e a taxa. Isso permite que o cliente compare o custo-benefício entre diferentes fornecedores (como o "Lojão do João" versus o "Saldão do Ricardão") diretamente na listagem.

## Aba "Promoções"
Ao alternar para esta seção, a interface muda o foco do "fornecedor" para o "produto", facilitando a descoberta de oportunidades econômicas.

### 1. Visualização de Produtos:

O layout em grade destaca imagens de alta fidelidade dos materiais (cimento, ferramentas, tintas), permitindo que o usuário identifique visualmente o que precisa sem depender apenas de descrições textuais.

### 2. Destaque Econômico:

A função principal desta tela é a economia. A interface exalta os descontos através de etiquetas visuais e preços comparativos, incentivando a compra de insumos essenciais (como cimento e tinta) ou ferramentas de desejo (como a serra mármore).

### 3. Acesso Direto à Compra:

Diferente da tela anterior, que leva à loja, esta tela encurta o caminho para a aquisição do produto específico, agilizando o fluxo de compra para itens que estão em oferta relâmpago.
