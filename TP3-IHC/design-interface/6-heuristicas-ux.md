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

| Heurística de Nielsen                             | Localização na Interface           | Justificativa do Uso                                                                                                                                                                                                                                                           |
| ------------------------------------------------- | ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| #1 Visibilidade do estado do sistema              | Abas Superiores e Cards de Serviço | O sistema informa proativamente sobre novas demandas através do badge numérico "2" na aba "Novos Pedidos". Nos cards, o uso de etiquetas coloridas ("Concluído" em verde, "Em Andamento" em azul) comunica o status atual do trabalho sem necessidade de clique.               |
| #2 Correspondência entre o sistema e o mundo real | Botões e Ícones de Navegação       | O botão "falar no WhatsApp" utiliza o nome e a logomarca do aplicativo real que o profissional usa para comunicação diária. O ícone de Martelo na barra inferior conecta-se metaforicamente ao conceito de "trabalho/obra" no mundo físico.                                    |
| #3 Controle e liberdade do usuário                | Botões de Decisão e Navegação      | O botão "Recusar" (contorno vermelho) oferece uma saída clara para o profissional que não pode aceitar um serviço, dando-lhe controle sobre sua agenda. O botão "voltar" no topo permite retornar à navegação anterior a qualquer momento.                                     |
| #4 Consistência e Padrões                         | Botões de Ação (Cards)             | Há uma consistência visual rigorosa: ações primárias/positivas ("Aceitar", "falar no WhatsApp") são sempre botões sólidos na cor da marca. Ações secundárias/negativas ("Recusar", "Finalizar") são sempre botões de contorno (outlined), mantendo o padrão mental do usuário. |
| #6 Reconhecimento em vez de memorização           | Metadados do Card                  | O uso de ícones universais (Pin para localização, Calendário para data) permite que o usuário reconheça o tipo de dado visualmente, reduzindo a carga cognitiva de ler rótulos repetitivos como "Local:" ou "Data:".                                                           |
| #8 Estética e design minimalista                  | Layout Geral                       | A interface exibe apenas o essencial para a tomada de decisão (Título, Local, Data), com amplo uso de espaço em branco e agrupamento lógico em cards, evitando ruído visual que distraia o profissional.                                                                       |

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

