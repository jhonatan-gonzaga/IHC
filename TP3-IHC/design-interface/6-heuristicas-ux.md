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

| Heurística de Nielsen                   | Localização na Interface    | Justificativa do Uso                                                                                                                                                                                            |
| --------------------------------------- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| #3 Controle e liberdade do usuário      | Topo e Base da Tela         | O usuário tem múltiplas rotas de saída: um botão "voltar" (seta), um botão "X" (fechar) no cabeçalho e um botão "Cancelar" na base, permitindo abandonar a tarefa sem erros.                                    |
| #4 Consistência e Padrões               | Botões de Ação              | A hierarquia visual é clara: o botão "Adicionar" (ação final) segue o padrão da marca (fundo vermelho), enquanto "Cancelar" é apenas contornado. Os ícones de Câmera e Galeria seguem padrões universais de UI. |
| #6 Reconhecimento em vez de memorização | Botões de Categoria (Chips) | O uso de etiquetas selecionáveis ("Construção", "Elétrica", "Pintura") evita que o usuário precise lembrar ou digitar manualmente a categoria do serviço, reduzindo a carga cognitiva.                          |
| #7 Flexibilidade e eficiência de uso    | Campo de Detalhes           | A presença do ícone de microfone dentro do campo de texto oferece um atalho para entrada de voz (Speech-to-Text), permitindo descrições mais ricas com menos esforço físico.                                    |
| #8 Estética e design minimalista        | Layout Geral                | O formulário é segmentado em blocos lógicos (Mídia > Dados Básicos > Categoria > Detalhes), com amplo espaçamento, evitando a sensação de "formulário burocrático".                                             |

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
| **1. Visibilidade do Status do Sistema** | Botões de seleção em **"Especialidades"** e **"Disponibilidade"** (Dias da semana). | O uso de cores distintas (fundo preenchido em vermelho para "selecionado" e fundo branco para "não selecionado") informa visualmente ao usuário, em tempo real, quais opções estão ativas. |
| **2. Compatibilidade entre o Sistema e o Mundo Real** | Ícones de **Câmera** (na foto), **Estrelas** (avaliação) e **R$** (valor). | A interface utiliza metáforas visuais familiares ao cotidiano do usuário (câmera para tirar foto, estrelas para qualidade) e linguagem natural nas profissões ("Pedreiro", "Pintor"), facilitando o entendimento. |
| **3. Controle e Liberdade do Usuário** | Ícone de **Seta para a esquerda** (canto superior esquerdo). | Oferece uma "saída de emergência" clara, permitindo que o usuário cancele a ação de edição e retorne à tela anterior sem frustração. |
| **4. Consistência e Padrões** | Ícone de **Engrenagem** e posicionamento do **Botão Salvar**. | O ícone de engrenagem é um padrão universal para "Configurações", e o botão de ação principal ("salvar Perfil") está posicionado ao final do formulário, conforme a convenção da maioria dos aplicativos móveis. |
| **6. Reconhecimento em vez de Memorização** | Lista de tags em **"Especialidades"**. | Ao invés de o usuário ter que digitar (lembrar) o nome da profissão, o sistema oferece opções visíveis para seleção, reduzindo a carga cognitiva e o esforço de digitação. |
| **7. Flexibilidade e Eficiência de Uso** | Carrossel de **"Avaliações Recentes"**. | Permite que o usuário navegue rapidamente pelos feedbacks deslizando para o lado, vendo as informações mais relevantes sem precisar abrir uma nova tela imediatamente. |
| **8. Estética e Design Minimalista** | Layout geral da tela. | A interface mantém o foco no essencial (edição de dados), com bom uso de espaço em branco e hierarquia visual clara, sem poluição visual ou informações irrelevantes para a tarefa de editar o perfil. |

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

# Tela do Lojista

## Tela o Perfil da Loja

<p align="center">
   <img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/2d15e453-8439-465f-ab25-ece42befb61c" />
</p>

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#1 Visibilidade do status do sistema** |Painel Geral | A tela oferece um resumo imediato da "saúde" da loja: dados de contato visíveis, prévia do estoque e promoções ativas. O usuário não precisa adivinhar o que está online; a interface mostra explicitamente o que o cliente final vê. |
| **#4 Consistência e Padrões** | Botões e Cards | Segue o padrão estabelecido no restante do app: botões de ação primária em vermelho/terracota ("+ Adicionar", "Editar Perfil") e cartões brancos com sombra suave para agrupar conteúdo. A barra de navegação inferior mantém a consistência de navegação global. |
| **#7 Flexibilidade e eficiência de uso** | Botões "Lista +" | Para usuários frequentes (lojistas), o sistema oferece atalhos de navegação. Ao invés de forçar o usuário a rolar infinitamente por todos os produtos nesta tela principal, o botão "Lista +" atua como um acelerador para ver o inventário completo apenas quando necessário. |
| **#8 Estética e design minimalista** | Segmentação por Blocos | A interface combate a sobrecarga de informação dividindo o conteúdo em três blocos lógicos e isolados visualmente: "Informações", "Catálogo" e "Promoções". Isso permite que o cérebro processe uma categoria de dados por vez.|
| **#2 Correspondência com o mundo real** | Ícones de Contato | O uso de metáforas visuais (Relógio para horário, Telefone para contato, Pin para endereço) mapeia objetos do mundo real para dados digitais, permitindo leitura rápida sem a necessidade de rótulos de texto explicativos ("Endereço:", "Telefone:"). |

## Usabilidade, Comunicabilidade e Coerência Visual
- Usabilidade (Arquitetura de Informação): A tela funciona como um Hub de Navegação. A hierarquia visual prioriza a "Identidade" (topo), seguida pelo "Core Business" (Catálogo) e "Estratégia de Venda" (Promoções). O botão "Editar Perfil" é destacado no topo, garantindo que a manutenção da conta seja uma ação de primeiro nível, fácil de encontrar.

- Comunicabilidade (Síntese): A interface utiliza o princípio da Divulgação Progressiva (Progressive Disclosure). Ao mostrar apenas os primeiros itens de cada lista (Produto A, Produto B) e oferecer um botão "Lista +", o sistema comunica que "há mais conteúdo aqui", mantendo a tela inicial limpa e carregando rápido, sem sobrecarregar o usuário com dados excessivos de imediato.

- Coerência Visual: A paleta de cores (fundo rosa claro, cartões brancos, elementos vermelhos) cria uma atmosfera de marca forte. A repetição do estilo dos botões "+ Adicionar Produto" e "+ Adicionar Promoção" cria uma simetria visual que torna a interface previsível e agradável.

## Considerações de Acessibilidade
- Agrupamento Semântico: Para leitores de tela, a estrutura de cabeçalhos (H1, H2) está clara ("Informações da Loja", "Catálogo", "Promoções"). Isso permite que usuários com deficiência visual saltem diretamente para a seção de interesse sem ouvir todo o conteúdo anterior.

- Identificação de Ícones: É crucial que os ícones do bloco "Informações" (Relógio, Pin, Telefone) possuam etiquetas aria-label ou descrições alternativas no código, pois não há texto visível dizendo "Telefone" ao lado do número, confiando puramente na interpretação visual do ícone.

- Contraste: O texto cinza escuro/preto sobre fundo branco nos cartões oferece excelente legibilidade. Os botões de ação (vermelhos) com texto branco passam nos testes de contraste WCAG AA, garantindo leitura sob diversas condições de iluminação.

## Evidências de Signos Metalinguísticos
- O ícone de Lápis no botão "Editar Perfil" é um signo universal de modificação.

- O ícone de Carrinho de Compras na aba inferior ("Loja") indica o contexto atual do usuário (Visão do Lojista).

- O ícone de Caixa Registradora na aba inferior ("Caixa") sugere o local onde as transações financeiras ocorrem.

## Tela Adicionar Produto e Promoção

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
| **#5 Prevenção de erros** | Restrição Visual de Campos +" | A separação explícita entre o campo de valor ("Preço" ou "Promoção") e o de "Quantidade", dispostos lado a lado, sugere visualmente a entrada de dados numéricos curtos, induzindo o usuário ao formato correto antes mesmo da digitação. |
| **#6 Reconhecimento em vez de memorização** | Rótulos (Labels) Estáticos | A interface mantém os rótulos ("Nome Produto", "Preço") visíveis acima dos campos o tempo todo, evitando o padrão de floating labels que somem ao digitar. Isso permite a revisão dos dados a qualquer momento sem esforço de memória.|
| **#8 Estética e design minimalista** | Área de Texto Limpa | O campo "Detalhes" é apresentado como uma área ampla e livre de ruídos visuais, focando inteiramente na redação das especificações técnicas do produto. |

## Usabilidade, Comunicabilidade e Coerência Visual
- Usabilidade (Eficiência de Input): O layout aplica o princípio de agrupamento (Gestalt) na linha central. Ao posicionar as variáveis críticas ("Preço/Promoção" e "Quantidade") lado a lado, o design otimiza o espaço vertical, evitando a rolagem excessiva e mantendo o botão de ação "Adicionar" acessível na primeira dobra da tela (above the fold) na maioria dos dispositivos.

- Comunicabilidade (Contexto Semântico): A interface comunica a mudança de contexto de forma sutil, mas vital. Embora visualmente semelhantes, a troca do rótulo e do placeholder altera o significado do dado:

    - Tela Produto: Comunica "Definição de Valor" (R$).

    - Tela Promoção: Comunica "Estratégia de Desconto" (%). Essa distinção semântica previne que o lojista cadastre acidentalmente um desconto de "90" como se fosse um preço de "R$ 90".

- Coerência Visual: A identidade visual é preservada através do sistema de design: campos com bordas arredondadas e sombras suaves, tipografia consistente e o botão de ação primária em vermelho sólido, alinhado com o restante do aplicativo (Login, Perfil).

## Considerações de Acessibilidade
- Lei de Fitts (Alvos de Toque): Os campos de input possuem altura generosa (padrão >48dp), facilitando a seleção precisa. O botão "Adicionar", ocupando largura isolada no rodapé, oferece um alvo de toque fácil e seguro, reduzindo erros motores.

- Contraste e Legibilidade: O texto de placeholder ("Digite o nome...", "R$ 0") utiliza um cinza que garante contraste suficiente para leitura, mas se diferencia claramente do texto preto de entrada final, indicando o estado de "campo vazio".

- Navegação Sequencial: A ordem lógica dos campos (Topo → Baixo, Esquerda → Direita) favorece a navegação por tecnologias assistivas (leitores de tela) e teclados, seguindo o fluxo natural de leitura.

##  Evidências de Signos Metalinguísticos
- Simbologia Instrucional:

    - O símbolo "R$" funciona como um signo imperativo: "Insira moeda corrente".

    - O símbolo "%" funciona como um alerta matemático: "Insira uma fração de desconto".

- Cor Semântica de Ação: A cor do botão "Adicionar" (Vermelho/Terracota) carrega o significado de "Commit" (Gravação/Comprometimento). Ela sinaliza que aquela interação resultará em uma alteração permanente no banco de dados, distinguindo-se de ações de navegação neutras.

- Ícone de Cabeçalho: O ícone de "Caixa" (Product Box) ao lado do título reforça visualmente o contexto operacional da tela: gestão de estoque físico.

## Tela Lista Catálago e Lista Promoção

<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/6e7106c6-5f4e-4651-8f90-acf4601a70c7" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/160b727a-3fbb-4f31-b47d-35ea88fb3268" />
</p>
</p>

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| **#1 Visibilidade do status do sistema** | Listagem Completa | A tela fornece feedback imediato sobre a extensão do inventário. Ao expandir a visão (ação oriunda do botão "Lista +"), o sistema confirma que todos os itens cadastrados estão carregados e visíveis, eliminando a incerteza de "onde estão meus outros produtos?". |
| **#4 Consistência e Padrões** | Design dos Cartões (Cards) | O layout visual dos itens (Nome > Preço > Quantidade) mantém-se idêntico ao apresentado no Dashboard e na Edição. Essa consistência reduz a carga cognitiva, pois o usuário não precisa aprender uma nova forma de ler o produto só porque mudou de tela. |
| **#6 Reconhecimento em vez de memorização** | Dados Expostos | Todas as variáveis críticas (Preço, Qtd, Descrição, Ano) estão visíveis no primeiro nível. O usuário não precisa clicar no item para lembrar "qual era a descrição deste produto?", facilitando a conferência rápida. |
| **#8 Estética e design minimalista** | Ritmo Vertical | A repetição consistente dos blocos de cartões, com espaçamento uniforme, cria um ritmo visual agradável que facilita o "escaneamento" (skimming) da lista com os olhos, sem ruídos visuais ou botões flutuantes que distraiam a leitura.|

## Usabilidade, Comunicabilidade e Coerência Visual
- Usabilidade (Leiturabilidade e Escaneabilidade): O objetivo principal desta tela é o consumo de informação. O design favorece a leitura vertical rápida através de uma hierarquia tipográfica clara: o "Nome do Produto" possui o maior peso visual, servindo como âncora para o olhar. O alinhamento dos dados secundários (Preço à esquerda, Quantidade à direita) cria colunas visuais imaginárias que permitem ao lojista comparar valores rapidamente ao rolar a tela.

- Comunicabilidade (Contexto de Leitura): A ausência de ícones de edição (lápis/lixeira) nesta visualização específica comunica um estado de "Modo de Leitura" (Read-Only). Isso transmite segurança ao usuário para navegar e rolar a lista livremente sem o medo de arrastar ou apagar algo acidentalmente (diferente da tela de Edição).

- Coerência Visual: A interface mantém a integridade do Design System. O uso do cabeçalho com o ícone da loja e o título "Lista" reforça o local onde o usuário está na arquitetura do app. A borda vermelha e o fundo branco dos cartões destacam o conteúdo sobre o fundo rosa claro da página.

## Considerações de Acessibilidade
- Ordem de Leitura Linear: A estrutura de lista é ideal para tecnologias assistivas. Leitores de tela (Screen Readers) podem percorrer os itens sequencialmente (Item 1 > Detalhes > Item 2 > Detalhes) sem interrupções de navegação complexas.

- Densidade de Informação: O espaçamento interno (padding) dentro dos cartões evita que o texto fique aglomerado, o que beneficia usuários com dificuldades de leitura ou dislexia, permitindo que cada bloco de informação seja processado individualmente.

- Contraste Tipográfico: A diferenciação entre o rótulo (cinza/preto claro) e o dado (Preço/Quantidade em negrito) ajuda usuários com baixa visão a distinguirem rapidamente o que é título e o que é valor.

## Evidências de Signos Metalinguísticos
- Ausência de Signos de Ação: A falta deliberada de botões de ação (como "Adicionar" ou "Editar") dentro dos cards funciona como um signo negativo, indicando: "Esta é uma área de visualização, não de interação".

- Seta de Retorno: O ícone de seta circulada no canto superior esquerdo é um signo universal de navegação que significa "Voltar ao nível superior" (o Dashboard), permitindo a saída segura da lista.

- Ícone de Lista/Loja: O ícone no cabeçalho (fachada da loja) atua como um marcador de contexto, reafirmando que a lista visualizada pertence ao inventário do próprio estabelecimento.



# Telas de Caixa de Mensagem e CHAT entre Logista e Clientes

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


# Telas do Cliente

##   Tela Inicial do cliente


 <p align="center">
   <img width="413" height="1328" alt="image" src="https://github.com/user-attachments/assets/641471ca-0ed7-4ab4-abc9-133cfab8abfc" />
</p>

É uma tela simples. Temos o menu superior, que é igual ao mesmo menu da tela 3, porém, não temos o menu inferior.

O usuário precisa escolher entre duas opções: Loja de materiais ou profissionais

Dependendo de qual o usuário escolher, será levado a uma tela com todas as funcionalidade que o cliente pode fazer com as personas do mesmo nome. Ou seja, se escolher lojas de materiais, será levado a tela 2, na qual poderá comprar coisas das lojas, bem como buscar por mais lojas, ver promoções, etc.

### Heurísticas da Tela inicial do cliente

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| Controle e liberdade do usuário<br><br>Consistência e padrões | Menu superior -> voltar | O usuário pode voltar rapidamente caso tenha se confundido e não seja do tipo "cliente", como indicado pela seta com o texto "voltar" |
| Visibilidade e status do sistema                              | Menu inferior           | É mostrado onde o usuário está ao colocar o ícone e o texto da sua localização em vermelho                                            |
| Design estático e minimalista                                 | Tela inteira            | Há poucos elementos, já que é uma tela "intermediária"                                                                                |
| Compatibilidade entre o sistema e o mundo real                | Opções disponíveis      | É falado a linguagem do usuário ao colocar uma imagem que remete ao texto, e ao que aquela opção se refere.                           |

### Signos da Tela inicial do cliente
- **Estáticos**
  - A **logo do aplicativo** é um signo estático.
  - O texto **"Selecione uma opção:"** é um símbolo estático.

- **Dinâmicos**
  - O **botão de voltar** no menu superior.
  - O **botão de perfil** no menu superior.
  - As duas opções


## Tela da listagem de Lojas e Serviços


<p float="left">
<p align="center">
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/680258a1-4ab5-4e0d-a474-0e93226a7da3" />
<img width="412" height="917" alt="image" src="https://github.com/user-attachments/assets/dab3db71-cb34-464a-8557-8702ba07770b" />
</p>
</p>

É a tela principal de navegação para o cliente encontrar fornecedores. Temos o menu superior com a localização e botão de voltar, uma barra de busca e filtros de estado ("Abertas Agora" vs "Promoções").
Abaixo, uma lista vertical de "Cards" representando as lojas disponíveis. Cada card contém informações resumidas cruciais para a decisão rápida (nome, categoria, distância, tempo e taxa). O menu inferior persiste para navegação global.

A tela "Seção de promoções" é acessada ao alternar o filtro superior para "Promoções". O layout muda de lista de lojas para uma grade (grid) ou lista de produtos específicos em oferta.
O foco visual é inteiramente na vantagem econômica. As informações de loja ficam em segundo plano ou implícitas, priorizando a imagem do produto, o preço antigo (riscado) e o preço novo com destaque, além de etiquetas de desconto.

### Heurísticas da tela de listagem de Lojas e Serviços - Abertas Agora

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| Visibilidade e status do sistema | Menu inferior e Filtros | É mostrado onde o usuário está ao colocar o ícone "Início" em vermelho. O filtro "Abertas Agora" está preenchido, indicando o que está sendo exibido. |
| Correspondência entre o sistema e o mundo real | Linguagem e Ícones | Uso de termos coloquiais ("Lojão", "Comprinhas") e ícones universais (Carrinho, Lupa) que traduzem ações digitais para conceitos físicos conhecidos. |
| Reconhecimento em vez de memorização | Cards das Lojas | O usuário vê todas as informações de decisão (taxa, tempo, distância) no card, sem precisar clicar e voltar (memorizar) para comparar lojas. |
| Consistência e padrões | Layout da tela | Segue o padrão mental de apps de delivery (Busca no topo, lista vertical, navegação no rodapé), reduzindo a curva de aprendizado. |
| Controle e liberdade do usuário | Botão Voltar | O usuário pode retornar ao menu anterior caso tenha entrado na seção de lojas por engano, indicado pela seta no canto superior esquerdo. |

### Signos da tela de listagem de Lojas e Serviços - Abertas Agora
- **Estáticos**
  - A **logo do aplicativo** no topo é um signo estático.
  - O texto da **localização ("Centro")** atua como rótulo fixo de estado atual.

- **Dinâmicos**
  - Os **botões de filtro** ("Abertas Agora", "Promoções").
  - Os **cards das lojas** (elementos clicáveis que levam ao detalhe).
  - A **barra de busca**.
  - Os **ícones do menu inferior**.

- **Metalinguísticos**
  - O texto dentro da barra de busca (**"Buscar Loja**


### Heurísticas da tela de listagem de Lojas e Serviços - Seção de promoções

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| Visibilidade e status do sistema | Filtro Superior "Promoções" | O botão "Promoções" agora aparece preenchido (sólido) e "Abertas Agora" vazado, dando feedback visual imediato da mudança de modo de visualização. |
| Correspondência entre o sistema e o mundo real | Preços "De/Por" e Tags | Uso da metáfora de varejo físico: preço antigo riscado e etiquetas vermelhas de porcentagem, símbolos universais de liquidação. |
| Reconhecimento em vez de memorização | Fotos dos Produtos | Imagens fiéis das embalagens (ex: saco de cimento Votoran) permitem que o profissional identifique o material visualmente sem ler o nome técnico. |
| Estética e design minimalista | Hierarquia Tipográfica | Redução de ruído visual. O destaque máximo é o preço novo (negrito, grande), facilitando o escaneamento rápido das ofertas. |
| Prevenção de erros | Imagens de Alta Fidelidade | Ao mostrar a foto real do produto (ex: Makita), evita-se que o usuário compre o modelo errado por confusão apenas com o nome do item. |

### Signos da tela de listagem de Lojas e Serviços - Seção de promoções

- **Estáticos**
  - Os nomes dos produtos (ex: **"Cimento 50 KG"**) funcionam como rótulos identificadores.
  - A **estrutura do card** (bordas e fundo).

- **Dinâmicos**
  - O botão de filtro **"Promoções"** (estado ativo).
  - Os **cards de produtos** (clicáveis para compra).
  - O botão **"Adicionar"** (implícito ou ao clicar no card).

- **Metalinguísticos**
  - O **traço sobre o preço antigo** (~R$ 50,00~) explicando que aquele valor não é mais válido.
  - A **etiqueta vermel**


## Tela inicial da opção "Profissionais"


 <p align="center">
   <img width="413" height="1328" alt="image" src="https://github.com/user-attachments/assets/9d58f953-71f4-40ce-a813-ed32181fcafb" />
</p>


Menu superior<br>
Temos quatro coisas no menu superior: a localização do cliente, a logo do aplicativo, o perfil, e voltar. O ícone de perfil manda o usuário a configurações da sua conta. A localização redireciona o usuário para trocar a sua localização. O botão de voltar retorna o usuário para escolher o tipo da usa conta.

Menu inferior<br>
Todas as opções disponíveis no menu inferior dessa tela está conforme o molic. Temos a tela inicial, que o usuário cliente sempre irá começar quando escolher a opção de profissionais. Também temos a opção de busca, uma tela (não feita) para buscar diversos tipos de profissionais, podendo ou não utilizar filtros. Finalmente, temos a opção de anunciar para colocar um anúncio para profissionais, com o intuito de achar alguém qualificado para aquele trabalho.

Campo de busca<br>
Na aba inicial, temos o campo de busca, onde o usuário pode buscar rapidamente o tipo de profissional que deseja contratar. É redirecionado automaticamente para a aba e tela "busca".

Categorias<br>
Na parte de categorias, temos várias categorias de profissionais, onde, ao usuário cliente clicar, será redirecionado para a tela (não feita) de "busca", com uma pesquisa utilizando o filtro da categoria que o usuário clicou. É possível "scrollar" verticalmente essa parte.

Profissionais em destaque<br>
A parte de profissionais em destaque coloca diversos tipos de profissionais que pagaram para serem anunciados para mais clientes, tanto na aba de busca como inicial, conforme o modelo de monetização do aplicativo.
Assim, é mostrado a foto de perfil dos profissionais, suas profissões logo abaixo, bem como o preço de uma diária (preço de um dia inteiro) e a avaliação, representada por estrelas. É possível "scrollar" essa parte.

### Heurísticas da tela inicial da opção "Profissionais"

| Heurística de Nielsen | Localização na Interface | Justificativa do Uso |
| :--- | :--- | :--- |
| Visibilidade e status do sistema                                          | Menu inferior                          | É mostrado onde o usuário está ao colocar o ícone e o texto em vermelho                                                                                                                                                                 |
| Visibilidade e status do sistema<br><br>Flexibilidade e eficiência de uso | Menu superior -> Localização       | O usuário pode ver a localização em que o sistema acha que ele está, mostrando o feedback o sistema. Para usuários mais experientes, é possível clicar na sua localização atual para mudar.                                             |
| Controle e liberdade do usuário<br><br>Consistência e padrões             | Menu superior -> voltar                | O usuário pode voltar rapidamente, como indicado pela seta com o texto "voltar"                                                                                                                                                         |
| Design estético e minimalista                                             | Tela inteira                           | No total, temos apenas três informações na tela, além do inferior e superior: Barra de busca, categorias, e profissionais em destaque.                                                                                                  |
| Compatibilidade com o sistema e o mundo real                              | Profissionais em destaque -> avaliação | Ao utilizar um sistema de estrelas, o usuário consegue rapidamente entender que significam algo bom ou ruim, dependendo de quantas estrelas estão preenchidas.                                                                          |
| Prevenção de erros<br><br>Flexibilidade e eficiência de uso               | Campo de busca                         | Há um texto bem como um ícone explicando ao usuário para que aquele campo serve, assim, prevenindo erros. O campo de busca está disponível para usuários que querem pesquisar logo quando entram no aplicativo, gerando uma eficiencia. |
| Flexibilidade e eficiência de uso                                         | Categorias -> ícones                   | O usuário pode escolher logo uma categoria de profissional para pesquisar, sem ter que primeiro ir na tela de busca e colocar o filtro da categoria desejada, assim, é um atalho.      


### Signos da tela inicial da opção "Profissionais"

- **Estáticos**
  - Os textos **Categorias** e **Profissionais em destaque** são signos estáticos.
  - A **logo do aplicativo** é um signo estático.

- **Dinâmicos**
  - O **botão de voltar** no menu superior.
  - O **botão de perfil** no menu superior.
  - Os **ícones** na parte de categorias.
  - Os **profissionais** na seção *Profissionais em destaque*.
  - Todos os **ícones e textos** no menu inferior.

- **Metalinguísticos**
  - O **campo de busca**, ao explicar para que serve.
  - O **botão e o texto de voltar**.


