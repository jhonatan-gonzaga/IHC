# Design Final

Nesta seção, apresentamos a evolução final da interface do Conecta Obra Itacoatiara, consolidando os fluxos de tarefas e wireframes desenvolvidos anteriormente em uma solução de alta fidelidade. O objetivo principal deste design é materializar uma plataforma que atue como um diretório digital eficiente para a construção civil, conectando clientes, profissionais e lojistas de forma ágil e segura.

# Telas para a Persona de Profissional

## telas de Oportunidades
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
  
