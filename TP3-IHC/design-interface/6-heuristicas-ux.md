# heuristicas-ux

Nesta seção, detalhamos como o design da interface do Conecta Obra Itacoatiara incorpora as Heurísticas de Usabilidade de Jakob Nielsen para assegurar uma interação fluida, eficiente e livre de erros. Considerando o perfil dos nossos usuários (desde clientes em busca de serviços até profissionais da construção e lojistas) priorizamos decisões de design que reduzem a carga cognitiva e aumentam a segurança na navegação.

---

# Telas para a Persona de Profissional
## Telas de Oportunidades

<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/2cdb4bc1-075e-4851-a90d-83bc01cc0120" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/2dbd40b8-12e7-4367-84b7-cd6b78128d2c" />
</p>
</p>

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#1 Visibilidade do estado do sistema** | **Tela: Novos Pedidos** e **Meus Serviços** | O **badge numérico "2"** na aba superior informa claramente quantas pendências existem. Nos cards, as etiquetas coloridas (**Verde** para "Concluído", **Azul** para "Em Andamento") mostram o status exato do serviço sem a necessidade de abrir detalhes. |
| **#2 Correspondência entre o sistema e o mundo real** | **Tela: Meus Serviços** | O botão **"falar no WhatsApp"** utiliza o ícone e o nome oficial do aplicativo, conectando a interface à ferramenta de comunicação real que o profissional já utiliza no dia a dia. |
| **#3 Controle e liberdade do usuário** | **Tela: Novos Pedidos** | O sistema oferece um botão **"Recusar"** claro e acessível nos cards de pedido, permitindo que o profissional tenha controle total para declinar trabalhos que não deseja ou não pode realizar. |
| **#4 Consistência e Padrões** | **Todas as Telas de Pedidos** | Há um padrão visual rigoroso para botões: ações positivas/primárias ("Aceitar", "Salvar") são sempre **vermelhas e sólidas**. Ações negativas/secundárias ("Recusar", "Finalizar") são sempre **brancas com contorno**, facilitando a decisão rápida. |
| **#6 Reconhecimento em vez de memorização** | **Tela: Novos Pedidos** | O uso de ícones universais nos cards (📍 **Pin** para localização e 📅 **Calendário** para data) permite que o usuário identifique o tipo de informação visualmente, sem precisar ler rótulos de texto repetitivos como "Endereço:" ou "Data:". |

---

## Usabilidade, Comunicabilidade e Coerência Visual
- O design das telas prioriza a **usabilidade** através de uma arquitetura de informação clara, onde a separação entre "Oportunidades" (Novos Pedidos) e "Gestão" (Meus Serviços) evita erros operacionais. A navegação é facilitada por áreas de toque generosas nos botões ("Aceitar"/"Recusar"), essenciais para o público-alvo que pode estar em movimento ou utilizando equipamentos de proteção.

- A **comunicabilidade** é garantida pela hierarquia tipográfica: o título do serviço ("Pintura Residencial") em negrito captura a atenção imediata, enquanto os ícones de suporte (local e data) fornecem contexto secundário rápido. A coerência visual é mantida pelo uso consistente da paleta de cores da marca (tons de vermelho/terracota e branco) e pelo estilo uniforme dos componentes (cards com bordas arredondadas e sombras sutis) em todas as etapas do fluxo.

## Considerações de Acessibilidade
- Tamanho de Toque: Os botões de ação ("Aceitar", "Recusar", "Finalizar") ocupam quase toda a largura do card e possuem altura adequada (acima de 44px), facilitando a interação para usuários com dificuldades motoras finas ou dedos largos.
- Contraste: O texto branco sobre o botão vermelho sólido e o texto vermelho sobre o fundo branco (botões outlined) apresentam alto índice de contraste, garantindo legibilidade.
- Independência de Cor: Embora as cores Verde e Azul indiquem status, elas são acompanhadas por rótulos de texto explícitos ("Concluído", "Em Andamento"), garantindo que usuários daltônicos compreendam o estado do sistema.

## Evidências de Signos Metalinguísticos
- Ícones Funcionais:

  - O ícone do WhatsApp não é apenas decorativo, mas um signo metalinguístico que avisa ao usuário: "ao clicar aqui, você sairá deste aplicativo e abrirá um mensageiro externo".

  -  O Badge numérico (2) na aba superior é um signo universal de notificação, indicando "quantidade de itens pendentes de atenção".

---
  ## Telas de Meu Projetos 
<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/c0dc771c-8fdd-4093-a186-0a2d20f86329" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/673e4107-6531-4c62-ae32-04593f8dde0b" />
</p>
</p>
A tabela abaixo mapeia a aplicação das heurísticas fundamentais de usabilidade nas telas desenvolvidas.

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#1 Visibilidade do estado do sistema** | Abas de Pedidos e Cards de Serviço | O sistema utiliza **badges numéricos** (ex: "2") para alertar sobre novas oportunidades e **etiquetas coloridas** ("Concluído", "Em Andamento") para indicar o status do serviço em tempo real. |
| **#2 Correspondência entre o sistema e o mundo real** | Botões e Ícones | O botão **"falar no WhatsApp"** utiliza a terminologia e marca familiar ao usuário. A seleção de mídia usa uma metáfora clara de **Câmera** (foto instantânea) vs **Quadro** (galeria). |
| **#3 Controle e liberdade do usuário** | Navegação e Formulários | O usuário possui saídas claras: botão **"Recusar"** para declinar pedidos, botões de **"Editar/Excluir"** (ícones de lápis/lixeira) no portfólio e botão **"Cancelar"** em formulários. |
| **#4 Consistência e Padrões** | Botões de Ação (CTA) | Existe um padrão visual rigoroso: ações primárias ("Aceitar", "Adicionar") são botões sólidos na cor da marca (Vermelho/Terracota). Ações secundárias ("Recusar", "Cancelar") são botões de contorno (*outlined*). |
| **#6 Reconhecimento em vez de memorização** | Lista de Projetos e Pedidos | O uso de ícones universais (Pin de mapa, Calendário) elimina a necessidade de ler rótulos repetitivos. No portfólio, a foto da obra é o elemento principal de reconhecimento. |
| **#7 Flexibilidade e eficiência de uso** | Formulário de Projeto | O campo de descrição inclui um ícone de **microfone**, permitindo entrada de dados por voz (*Speech-to-Text*), agilizando o preenchimento para usuários em movimento. |


## Análise de UX/UI: Usabilidade, Comunicabilidade e Coerência

### Usabilidade e Comunicabilidade
A interface foi projetada para reduzir a carga cognitiva. Na tela de "Novos Pedidos", apenas as informações essenciais para a tomada de decisão (Título, Bairro e Data) são exibidas, evitando ruído visual. No cadastro de projetos, a hierarquia visual guia o usuário: o botão **"Tirar foto Agora"** é significativamente maior e mais colorido que as outras opções, comunicando a preferência do sistema pelo registro imediato e autêntico da obra.

### Coerência Visual
A identidade visual é mantida através da repetição consistente de componentes:
* **Cards:** Todos os itens de lista (pedidos ou projetos) utilizam o mesmo contêiner com bordas arredondadas e sombra sutil.
* **Cores:** A cor primária (Terracota #B84B55 aprox.) é usada exclusivamente para elementos interativos ativos e ícones de destaque.


##  Acessibilidade e Inclusão

O design considera as limitações contextuais e físicas do público-alvo:

* **Tamanho de Toque:** Botões críticos como "Aceitar", "Recusar" e "Tirar Foto" ocupam toda a largura do contêiner e possuem altura generosa (>48dp), facilitando o acionamento por usuários com dificuldades motoras ou dedos largos.
* **Entrada Multimodal:** A opção de **ditado por voz** no formulário de projetos remove a barreira da digitação para usuários com baixo letramento digital.
* **Independência de Cor:** Os status de serviço utilizam cores (Verde/Azul), mas são sempre acompanhados de rótulos de texto ("Concluído"/"Em Andamento"), garantindo que daltônicos compreendam a informação.
* **Seleção Simplificada:** O uso de *Chips* (botões de tag) para selecionar categorias ("Construção", "Elétrica") evita erros de ortografia e reduz o esforço motor de digitação.

##  Signos Metalinguísticos

Elementos visuais que reforçam a comunicação e fornecem feedback instantâneo:

* **Ícones Semânticos:**
    *  **Badge Numérico (2):** Signo universal de notificação/pendência.
    *  **Logo WhatsApp:** Significa "Comunicação externa" (saída do app).
    *  **Câmera:** Significa "Captura de imagem".
    *  **Lápis /  Lixeira:** Signos padrão para "Editar" e "Destruir" conteúdo.
* **Feedback de Navegação:** Na barra inferior (*Bottom Bar*), o ícone ativo (ex: Martelo ou Prancheta) torna-se preenchido e colorido, enquanto os inativos permanecem em linha cinza, indicando visualmente a localização do usuário na arquitetura do app.

---
## Tela de Perfil do Profissional

 <p align="center">
   <img width="413" height="1328" alt="image" src="https://github.com/user-attachments/assets/f5fa3599-929c-4170-8770-d7c4e0bb325f" />
</p>

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#3 Controle e liberdade do usuário** | Topo e Base da Tela | O usuário tem múltiplas rotas de saída: um botão "voltar" (seta), um botão "X" (fechar) no cabeçalho e um botão "Cancelar" na base, permitindo abandonar a tarefa sem erros. |
| **#4 Consistência e Padrões** | Botões de Ação | A hierarquia visual é clara: o botão "Adicionar" (ação final) segue o padrão da marca (fundo vermelho), enquanto "Cancelar" é apenas contornado. Os ícones de Câmera e Galeria seguem padrões universais de UI. |
| **#6 Reconhecimento em vez de memorização** | Botões de Categoria (Chips) | O uso de etiquetas selecionáveis ("Construção", "Elétrica", "Pintura") evita que o usuário precise lembrar ou digitar manualmente a categoria do serviço, reduzindo a carga cognitiva. |
| **#7 Flexibilidade e eficiência de uso** | Campo de Detalhes | A presença do ícone de microfone dentro do campo de texto oferece um atalho para entrada de voz (*Speech-to-Text*), permitindo descrições mais ricas com menos esforço físico. |
| **#8 Estética e design minimalista** | Layout Geral | O formulário é segmentado em blocos lógicos (Mídia > Dados Básicos > Categoria > Detalhes), com amplo espaçamento, evitando a sensação de "formulário burocrático". |

## Análise de UX/UI
Usabilidade e Hierarquia Visual
O design utiliza a Lei de Fitts ao maximizar a área de toque do botão "Tirar foto Agora". Ele é significativamente maior e mais colorido que o botão de "Galeria", guiando o usuário para a ação preferencial do sistema: documentar a obra em tempo real para garantir autenticidade.

## Comunicabilidade
A interface utiliza perguntas diretas e informais ("Toque no que você fez:", "Em qual Bairro?") em vez de rótulos técnicos ("Categoria", "Localização"), adequando a linguagem ao perfil do usuário e tornando a interação mais conversacional.

##  Acessibilidade
- Tamanho de Toque: O botão principal de câmera ocupa quase 25% da área útil da tela, facilitando o acionamento por usuários em movimento ou utilizando luvas de proteção.
- Entrada Multimodal: O suporte a ditado por voz (microfone) remove barreiras para usuários com dificuldades de letramento ou limitações motoras finas para digitação em teclados virtuais pequenos.

- Contraste: Os botões de ação principal (Vermelho com texto Branco) possuem alto contraste, garantindo legibilidade.

##  Signos Metalinguísticos
Elementos visuais que comunicam função sem depender de texto:

- Ícone de Câmera: Signo universal para "Captura de imagem imediata".

- Ícone de Quadro: Signo para "Arquivo de imagem / Galeria".

- Ícone de Microfone: Signo metalinguístico que instrui: "Você pode falar aqui em vez de digitar".

- Ícone X: Signo de cancelamento/fechamento de modal.

---
#  Telas para a Persona Lojista

## Tela do Perfil Loja

<p align="center">
   <img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/2d15e453-8439-465f-ab25-ece42befb61c" />
</p>

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#3 Controle e liberdade do usuário** | Botões de "Lixeira" e "Voltar"" | O sistema oferece saídas claras: o ícone de lixeira nos cartões permite a exclusão imediata de itens obsoletos, e a seta de "voltar" no topo garante a navegação reversa sem travar o usuário em fluxos de cadastro. |
| **#4 Consistência e Padrões** | Cards de Listagem | A estrutura visual dos cartões de "Produto" e "Promoção" é idêntica (Nome no topo, valores à esquerda, quantidade à direita), variando apenas o dado crítico (R$ vs %). Isso reduz a curva de aprendizado ao alternar entre abas. |
| **#6 Reconhecimento em vez de memorização** | Placeholders e Rótulos | Os campos de formulário possuem rótulos claros ("Preço", "Promoção") e placeholders ("R$ 0", "% 0", "Digite o nome") que exemplificam o formato esperado, eliminando a dúvida sobre como inserir os dados. |
| **#5 Prevenção de erros** | Botão "Salvar Alterações" | Na tela de edição de perfil, as mudanças não são aplicadas instantaneamente. O botão persistente no rodapé atua como uma barreira de confirmação, prevenindo que toques acidentais alterem dados críticos da loja. |
| **#8 Estética e design minimalista** | Formulários de Cadastro | A tela de "Adicionar" remove qualquer elemento desnecessário, focando apenas nos inputs essenciais. O uso de espaço em branco generoso entre os campos ("Nome", "Preço/Qtd", "Detalhes") evita a poluição visual. |

## Análise de UX/UI: Usabilidade, Comunicabilidade e Coerência
- O design do módulo lojista prioriza a usabilidade através da eficiência nas tarefas de manutenção (CRUD). A decisão de colocar os ícones de ação rápida (Edição/Lápis e Exclusão/Lixeira) diretamente no cabeçalho dos cartões, na tela de perfil, reduz o número de cliques necessários para gerenciar o inventário, dispensando menus de contexto ocultos que dificultariam a operação rápida.
- A comunicabilidade é reforçada pela clareza dos rótulos e distinção contextual. Ao separar "Catálogo" de "Promoções", a interface comunica que, embora sejam itens de estoque, possuem comportamentos de venda diferentes. O uso de prefixos como "R$" para produtos e "%" para promoções informa visualmente a natureza do valor numérico antes mesmo da leitura do rótulo.
- A coerência visual é mantida pelo reuso estrito de componentes. O botão de ação primária (Adicionar/Salvar) sempre utiliza a cor sólida da marca (vermelho/terracota) e ocupa a largura total na base da tela, criando um padrão mental de "finalização de tarefa" consistente em todo o aplicativo.
-A coerência visual é mantida pelo reuso estrito de componentes. O botão de ação primária (Adicionar/Salvar) sempre utiliza a cor sólida da marca (vermelho/terracota) e ocupa a largura total na base da tela, criando um padrão mental de "finalização de tarefa" consistente em todo o aplicativo.

## Acessibilidade
- Áreas de Toque: Os ícones de interação crítica na lista editável (Lápis e Lixeira) foram posicionados com espaçamento suficiente entre si e das bordas do cartão, visando acomodar o "dedo gordo" (fat finger) e prevenir toques acidentais, crucial para uso em dispositivos móveis em movimento.
- Contraste e Leitura: Os formulários utilizam bordas bem definidas e alto contraste entre o texto (preto/cinza escuro) e o fundo (branco/rosa claro), garantindo que os campos de entrada sejam facilmente identificáveis por usuários com baixa visão.
- Hierarquia de Foco: O título da tela ("Adicionar Produto", "Perfil Loja") é o elemento de maior peso visual, seguido pelos rótulos dos campos, orientando a ordem de leitura natural de cima para baixo.

## Metalinguísticos
- Ícones Universais:
  - O ícone de Lápis é um signo metalinguístico universal para "modificação de conteúdo existente".
  - O ícone de Lixeira comunica inequivocamente a ação destrutiva de "remoção permanente".
  - O ícone de Loja (fachada) e Relógio na edição de perfil agem como metáforas visuais que substituem a necessidade de ler os rótulos "Endereço" ou "Horário", acelerando o reconhecimento cognitivo.
- Cores Semânticas: O uso da cor vermelha nos botões principais não é apenas estética, mas um signo que indica "Ação Prioritária" ou "Conclusão". Já o contorno vermelho nos campos de input ativos (foco) indica ao usuário "você está editando este campo agora".

## Tela de Adicionar Produto e Adicionar Promção

<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/d983555a-0cb3-4beb-a81d-96a88a1e1278" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/e30f6e15-489b-4a68-8afa-4ba94e24fa7a" />
</p>
</p>

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#2 Correspondência com o mundo real** | Placeholders e Símbolos (R$ / %) | O sistema adota a linguagem nativa do varejo. Ao exibir "R$" para produtos e "%" para promoções como texto de exemplo, a interface conecta-se ao modelo mental do lojista: cadastro de estoque é valor monetário, oferta é valor percentual. |
| **#4 Consistência e Padrões** | Espelhamento de Layout | Os formulários são estruturalmente idênticos. A manutenção rígida da grade (Grid) — "Nome" no topo, variáveis numéricas no meio, "Detalhes" abaixo — garante previsibilidade. O usuário aprende o fluxo uma vez e o aplica em ambos os cenários com carga cognitiva mínima. |
| **#5 Prevenção de erros** | Restrição Visual de Campos | A separação explícita entre o campo de valor ("Preço" ou "Promoção") e o de "Quantidade", dispostos lado a lado, sugere visualmente a entrada de dados numéricos curtos, induzindo o usuário ao formato correto antes mesmo da digitação. |
| **#6 Reconhecimento em vez de memorização** | Rótulos (Labels) Estáticos | A interface mantém os rótulos ("Nome Produto", "Preço") visíveis acima dos campos o tempo todo, evitando o padrão de floating labels que somem ao digitar. Isso permite a revisão dos dados a qualquer momento sem esforço de memória. |
| **#8 Estética e design minimalista** | Área de Texto Limpa | O campo "Detalhes" é apresentado como uma área ampla e livre de ruídos visuais, focando inteiramente na redação das especificações técnicas do produto. |

## Análise de UX/UI: Usabilidade, Comunicabilidade e Coerência
- Usabilidade (Eficiência de Input): O layout aplica o princípio de agrupamento (Gestalt) na linha central. Ao posicionar as variáveis críticas ("Preço/Promoção" e "Quantidade") lado a lado, o design otimiza o espaço vertical, evitando a rolagem excessiva e mantendo o botão de ação "Adicionar" acessível na primeira dobra da tela (above the fold) na maioria dos dispositivos.
- Comunicabilidade (Contexto Semântico): A interface comunica a mudança de contexto de forma sutil, mas vital. Embora visualmente semelhantes, a troca do rótulo e do placeholder altera o significado do dado:
  - Tela Produto: Comunica "Definição de Valor" (R$).
  - Tela Promoção: Comunica "Estratégia de Desconto" (%). Essa distinção semântica previne que o lojista cadastre acidentalmente um desconto de "90" como se fosse um preço de "R$ 90".
- Coerência Visual: A identidade visual é preservada através do sistema de design: campos com bordas arredondadas e sombras suaves, tipografia consistente e o botão de ação primária em vermelho sólido, alinhado com o restante do aplicativo (Login, Perfil).

## Acessibilidade
- Lei de Fitts (Alvos de Toque): Os campos de input possuem altura generosa (padrão >48dp), facilitando a seleção precisa. O botão "Adicionar", ocupando largura isolada no rodapé, oferece um alvo de toque fácil e seguro, reduzindo erros motores.
- Contraste e Legibilidade: O texto de placeholder ("Digite o nome...", "R$ 0") utiliza um cinza que garante contraste suficiente para leitura, mas se diferencia claramente do texto preto de entrada final, indicando o estado de "campo vazio".
- Navegação Sequencial: A ordem lógica dos campos (Topo → Baixo, Esquerda → Direita) favorece a navegação por tecnologias assistivas (leitores de tela) e teclados, seguindo o fluxo natural de leitura.

## Metalinguísticos
- Simbologia Instrucional:
  - O símbolo "R$" funciona como um signo imperativo: "Insira moeda corrente".
  -O símbolo "%" funciona como um alerta matemático: "Insira uma fração de desconto".
- Cor Semântica de Ação: A cor do botão "Adicionar" (Vermelho/Terracota) carrega o significado de "Commit" (Gravação/Comprometimento). Ela sinaliza que aquela interação resultará em uma alteração permanente no banco de dados, distinguindo-se de ações de navegação neutras.
- Ícone de Cabeçalho: O ícone de "Caixa" (Product Box) ao lado do título reforça visualmente o contexto operacional da tela: gestão de estoque físico.

## Tela de Lista Catálogo e Lista Promoção

<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/6e7106c6-5f4e-4651-8f90-acf4601a70c7" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/160b727a-3fbb-4f31-b47d-35ea88fb3268" />
</p>
</p>

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#2 Correspondência com o mundo real** | Placeholders (R$ 0 / % 0) | O sistema fala a linguagem do lojista: ao exibir "R$" para produtos e "%" para promoções dentro do campo de input, a interface reforça o modelo mental de varejo, onde o cadastro padrão é monetário e a oferta é relativa (desconto percentual). |
| **#4 Consistência e Padrões** | Estrutura dos Formulários | Os dois formulários são espelhos um do outro. A manutenção da mesma grade (Grid) e posicionamento dos campos garante que o usuário não perca tempo reaprendendo a interface ao mudar de tarefa. |
| **#5 Prevenção de erros** | Restrições de Input (Implícito) | A separação visual clara entre "Preço" e "Quantidade" lado a lado, com placeholders numéricos ("0"), sugere ao usuário o tipo de teclado que deve ser aberto (numérico vs. alfanumérico), prevenindo a inserção de texto em campos de cálculo. |
| **#6 Reconhecimento em vez de memorização** | Labels (Rótulos) Externos | Os rótulos ("Nome Produto", "Detalhes") estão posicionados permanentemente fora dos campos de digitação. Isso garante que, mesmo após o usuário começar a digitar (e o placeholder sumir), ele ainda saiba a que se refere aquele campo, sem precisar apagar o texto para lembrar. |
| **#8 Estética e design minimalista** | Área de "Detalhes" | O campo de descrição é amplo e limpo, sem ícones desnecessários ou formatação complexa, focando totalmente no conteúdo textual que descreve o item. |

## Análise de UX/UI: Usabilidade, Comunicabilidade e Coerência
- Usabilidade (Eficiência de Preenchimento): O design adota o agrupamento lógico (Gestalt) na linha intermediária dos formulários. Ao colocar as variáveis numéricas curtas ("Preço/Promoção" e "Quantidade") lado a lado, o sistema otimiza o espaço vertical da tela e reduz a necessidade de rolagem (scroll), permitindo que o botão de ação "Adicionar" esteja visível sem esforço na maioria dos dispositivos.
- Comunicabilidade (Contexto da Ação): A distinção entre as telas é comunicada sutilmente, mas de forma eficaz, pela adaptação do primeiro campo numérico.
  - Em Produto, o campo comunica "Valor Monetário" (R$).
  - Em Promoção, o campo comunica "Fator de Desconto" (%). Isso assegura que o lojista entenda o impacto financeiro do dado que está inserindo (preço cheio vs. margem de desconto).
- Coerência Visual: A consistência é mantida pelo uso rigoroso do sistema de design: inputs com bordas arredondadas na cor da marca (quando ativos ou focados), tipografia padronizada e o botão primário "Adicionar" com a mesma cor sólida e dimensões encontradas no restante do aplicativo.

## Acessibilidade
- Lei de Fitts (Alvos de Toque): Os campos de entrada de texto possuem altura generosa (> 48dp), facilitando a seleção precisa com o dedo. O botão "Adicionar" é largo e isolado, tornando-se um alvo fácil de atingir, o que é crucial para usuários com coordenação motora reduzida.
- Contraste e Legibilidade: O texto de preenchimento ("Digite o nome...") utiliza um cinza claro que tem contraste suficiente para ser lido, mas é distinto o bastante do texto preto final, indicando seu estado provisório. As bordas dos inputs delimitam claramente a área interativa.
- Navegação por Teclado (Foco): A ordem linear dos campos (Cima para Baixo, Esquerda para Direita) favorece a navegação lógica para quem utiliza leitores de tela ou teclados externos, seguindo o fluxo natural de leitura ocidental.

## Metalinguísticos
- Símbolos de Unidade como Signos:
  - O símbolo "R$" (Real) não é apenas uma moeda, mas um signo que instrui o usuário: "Insira aqui o valor de venda".
  - O símbolo "%" (Porcentagem) atua como um alerta metalinguístico: "Cuidado, este valor será subtraído do preço original".
- Cores de Ação: O vermelho/terracota no botão "Adicionar" carrega o significado de "Commit" (Comprometimento). Ele sinaliza que aquela ação irá alterar o estado do banco de dados do sistema, diferenciando-se de botões de navegação neutros.
- Ícone do Cabeçalho: A caixa aberta (logo) ao lado do título atua como um identificador visual da seção "Logística/Estoque", reforçando o contexto operacional da tela.

## Tela de Edição

 <p align="center">
   <img width="413" height="1328" alt="image" src="https://github.com/user-attachments/assets/3d39aa92-b4a2-4676-b2e9-13621f6f3ea4" />
</p>

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#3 Controle e liberdade do usuário** | Ícones de Lixeira e Voltar | O sistema oferece "saídas de emergência" e reversibilidade. O ícone de lixeira permite a remoção de itens indesejados, enquanto o botão de voltar garante que o usuário possa desistir da edição sem aplicar mudanças indesejadas. |
| **#5 Prevenção de erros** | Botão "Salvar Alterações" | A interface adota um modelo de confirmação explícita. Ao invés de salvar cada caractere digitado em tempo real (o que poderia causar erros catastróficos em dados públicos), o sistema exige um clique final no botão "Salvar Alterações" para efetivar as mudanças no banco de dados. |
| **#6 Reconhecimento em vez de memorização** | Ícones de Edição (Lápis) | O uso repetitivo do ícone de lápis ao lado de cada campo editável (Nome, Horário, Telefone) elimina a necessidade de o usuário adivinhar o que pode ser alterado. A interface sinaliza visualmente: "onde há lápis, há edição". |
| **#7 Flexibilidade e eficiência de uso** | Ações Rápidas nos Cards | Para usuários experientes (lojistas), a interface oferece atalhos (aceleradores). Permitir a edição e exclusão direta no cartão do produto evita a necessidade de abrir a página de detalhes de cada item, agilizando a manutenção do estoque em massa. |
| **#8 Estética e design minimalista** | Agrupamento de Seções | A tela organiza densas informações administrativas em blocos claros ("Informações", "Catálogo", "Promoções"), utilizando espaços em branco para reduzir a carga visual e permitir que o gestor foque em um grupo de dados por vez. |

## Análise de UX/UI: Usabilidade, Comunicabilidade e Coerência
- Usabilidade (Eficiência Operacional): A tela foi desenhada para o fluxo de trabalho de Manutenção (CRUD). A decisão de expor as ações de "Editar" e "Excluir" diretamente na lista (no canto superior direito dos cards) reduz drasticamente o número de cliques (interaction cost) necessários para gerenciar um estoque grande, comparado a fluxos que exigem entrar em cada item individualmente.
- Comunicabilidade (Estado do Sistema): A interface comunica claramente que está em "Modo de Edição" através da mudança de affordance. Diferente da tela de visualização passiva, aqui todos os campos ganham ícones indicadores (lápis) e bordas de input, sinalizando interatividade.
- Coerência Visual: A consistência é mantida pelo sistema de ícones (Iconography System). O estilo de linha (outlined) na cor da marca é aplicado uniformemente tanto nos ícones institucionais (relógio, loja) quanto nos funcionais (lápis, lixeira), criando uma harmonia visual que guia o olhar.
  
## Acessibilidade
- Áreas de Toque (Touch Targets): Os ícones de ação nos cartões (Lápis e Lixeira) possuem um espaçamento horizontal crítico entre si. Isso é vital para evitar o "erro de toque vizinho", onde o usuário tenta editar mas acaba clicando em excluir.
- Feedback de Estado: O botão "Salvar Alterações" no rodapé possui alta proeminência (cor sólida e largura total). Para acessibilidade, ele serve como um ponto de ancoragem visual e de navegação por teclado, indicando o fim do formulário.
- Hierarquia de Leitura: O uso de títulos em negrito ("Informações da Loja", "Catálogo") permite que usuários de leitores de tela naveguem rapidamente entre as seções, pulando blocos de conteúdo que não desejam editar no momento.

## Metalinguísticos
- Metáforas Universais:
  - Lápis: Signo metalinguístico universal para "reescrever" ou "alterar conteúdo".
  - Lixeira: Signo icônico para "descarte" ou "destruição irreversível".
- Cores Funcionais: Enquanto a cor vermelha/terracota é a cor da marca (branding), nos ícones de "Lixeira" ela assume uma conotação de alerta (Warning), sugerindo cuidado na interação.
- Posicionamento Espacial: O posicionamento do botão "Salvar" flutuando ou fixo na base da tela cria uma metáfora de "rodapé de documento", indicando que aquela ação valida tudo o que está acima dela (herança de formulários de papel).

## Telas de Caixa de Mensagem e CHAT entre Logista e Clientes

<img width="233" height="521" alt="image" src="https://github.com/user-attachments/assets/b03c05d7-8715-4dd1-9149-55d128420b83" />
<img width="237" height="521" alt="image" src="https://github.com/user-attachments/assets/d101f585-0b34-468e-84ab-fc0069b5da3b" />

## Tela de Caixa de Mensagens — Avaliação por Heurísticas de Nielsen

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#1 Visibilidade do status do sistema** | Lista de Conversas | O badge numérico de mensagens não lidas informa imediatamente ao usuário que há novas interações pendentes, mantendo-o ciente do estado atual do sistema. |
| **#3 Controle e liberdade do usuário** | Cabeçalho | O botão de voltar (seta à esquerda) possibilita que o usuário abandone a tela a qualquer momento, sem consequências negativas ou perda de progresso. |
| **#4 Consistência e padrões** | Barra de Navegação Inferior | Os ícones e sua disposição seguem o mesmo padrão visual e funcional das demais telas do aplicativo, reduzindo a necessidade de reaprendizado. |
| **#6 Reconhecimento em vez de memorização** | Item de Conversa | O texto “Toque para conversar” explicita a ação possível, evitando que o usuário tenha de lembrar como iniciar uma conversa. |
| **#8 Estética e design minimalista** | Layout Geral | A tela apresenta apenas os elementos essenciais (conversa, avatar e navegação), eliminando ruídos visuais e facilitando a leitura e tomada de decisão. |

### Análise de UX/UI — Caixa de Mensagens

#### Usabilidade e Hierarquia Visual
A hierarquia é clara e direta: o nome do contato aparece em maior destaque, seguido pelo texto de apoio e pelo indicador de mensagens. Isso permite que o usuário identifique rapidamente onde deve interagir, sem esforço cognitivo adicional.

#### Comunicabilidade
A interface utiliza linguagem simples e orientada à ação (“Toque para conversar”), comunicando de forma explícita a possibilidade de interação e reduzindo ambiguidades quanto à função da tela.

#### Acessibilidade
- **Área de toque:** O item de conversa ocupa uma faixa horizontal ampla, facilitando o toque preciso.  
- **Contraste:** O uso de tons mais escuros para o nome e indicadores garante boa legibilidade sobre o fundo claro.

#### Signos Metalinguísticos
- **Avatar circular:** Signo universal de representação de usuário/pessoa.  
- **Badge numérico:** Signo visual imediato para “há algo novo aqui”.  
- **Ícone de chat na barra inferior:** Representação clara do contexto atual da navegação.

---

## Tela de Chat (Conversa Ativa) — Avaliação por Heurísticas de Nielsen

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#1 Visibilidade do status do sistema** | Cabeçalho e Identificação do Contato | O nome “Cliente” e o avatar no topo deixam claro com quem o usuário está conversando no momento. |
| **#2 Correspondência entre o sistema e o mundo real** | Estrutura da Conversa | A disposição vertical das mensagens segue o modelo mental comum de aplicativos de mensagens do cotidiano. |
| **#3 Controle e liberdade do usuário** | Botão de Voltar e Campo de Entrada | O usuário pode sair da conversa a qualquer momento e escolher entre digitar, usar voz ou não enviar a mensagem. |
| **#4 Consistência e padrões** | Campo de Mensagem e Ícones | Os elementos visuais seguem padrões amplamente reconhecidos em aplicativos de chat. |
| **#6 Reconhecimento em vez de memorização** | Placeholder do Input | O texto “Informar mensagem…” orienta claramente o usuário sobre o que deve ser feito. |
| **#8 Estética e design minimalista** | Tela como um todo | O uso de fundo neutro e poucos elementos visuais mantém o foco total na comunicação. |

### Análise de UX/UI — Chat

#### Usabilidade e Hierarquia Visual
A posição fixa do campo de entrada na base da tela respeita a ergonomia do uso móvel, reduzindo deslocamentos e priorizando interações rápidas.

#### Comunicabilidade
A interface comunica suas funções por meio de ícones e textos curtos, eliminando a necessidade de instruções adicionais.

#### Acessibilidade
- **Entrada multimodal:** Presença de microfone para ditado por voz, reduzindo barreiras de digitação.  
- **Elementos amplos:** Facilita o uso em telas pequenas ou em contextos de mobilidade.

#### Signos Metalinguísticos
- **Ícone de Microfone:** Indica entrada por voz.  
- **Ícone de Enviar:** Representa a ação de despachar a mensagem.  
- **Seta de Voltar:** Signo universal de retorno de navegação.
