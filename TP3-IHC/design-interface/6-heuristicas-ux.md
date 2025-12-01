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

# Telas de Caixa de Mensagem e CHAT entre Logista e Clientes

<img width="234" height="519" alt="image" src="https://github.com/user-attachments/assets/ecadb73c-3c33-4505-aca0-7a9d34513567" />
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
