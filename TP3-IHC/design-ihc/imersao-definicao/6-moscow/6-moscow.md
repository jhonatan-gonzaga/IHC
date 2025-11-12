<div align="center">
  
  # MoSCoW
  
  &nbsp;
</div>

![MoSCoW](https://github.com/user-attachments/assets/d3e987e0-4e08-4975-91e7-d40201c7b8d0)


# Priorização de Requisitos (MoSCoW) Detalhada para o Projeto

A Matriz MoSCoW é utilizada para classificar e priorizar os requisitos levantados nas Jornadas do Usuário (Profissional, Cliente, Lojista e Suporte), definindo o escopo do produto (MVP - Mínimo Produto Viável).

## Must have (Obrigatórios) - DEVE TER

Estes são os requisitos **imprescindíveis** e não negociáveis. Sem eles, o produto não pode ser lançado, pois falha em cumprir seu propósito principal (conectar, gerenciar o ciclo de serviço e ranquear).

| Requisito | Explicação e Função |
| :--- | :--- |
| **Recurso Text-to-Speech (TTS) para leitura de textos críticos** | **Acessibilidade e Usabilidade:** É o recurso base que permite ao usuário com baixa literacia digital ouvir textos longos, instruções e dados sensíveis (códigos, termos) para minimizar erros e frustração. |
| **Cadastro/Login Simples com Código de Verificação** | **Segurança e Acesso:** Garante a autenticação segura do usuário (Profissional, Cliente, Lojista), sendo a porta de entrada para todas as funcionalidades. |
| **Criação e Edição de Perfil Profissional** | **Prontidão:** Permite ao profissional se qualificar e se apresentar, sendo um pré-requisito para receber ofertas. |
| **Cadastro de Loja e Perfil (Lojista)** | **Presença:** Permite ao lojista inserir informações básicas da loja para aparecer na busca de materiais. |
| **Opção de Anunciar Serviço OU Buscar Profissionais** | **Flexibilidade:** É a funcionalidade central que oferece ao Cliente a escolha entre criar uma demanda ou ir diretamente ao perfil de um profissional. |
| **Anunciar Serviço (Formulário Simples + Anexar Foto)** | **Gatilho de Demanda:** Permite ao Cliente criar um anúncio de serviço de forma ágil, com detalhes visuais do problema. |
| **Busca e Lista Filtrada de Profissionais** | **Localização:** Permite ao Cliente encontrar rapidamente profissionais por tipo de serviço e localização (ex.: "Pintores em Itacoatiara"). |
| **Visualização de Perfil Completo (Portfólio, Avaliações, Preço Médio)** | **Confiança:** Fornece os dados essenciais para o Cliente tomar a decisão de contratação, minimizando a incerteza. |
| **Sistema de Notificação de Ofertas/Candidatos/Suporte** | **Interação:** Alerta os usuários sobre eventos críticos (nova oferta, nova candidatura, novo pedido de suporte) para iniciar o ciclo de ação. |
| **Botão "Aceitar Oferta" (Candidatura)** | **Ação do Profissional:** Permite que o profissional manifeste interesse no serviço anunciado pelo Cliente. |
| **Botão "Contratar" (Decisão do Cliente)** | **Transição de Status:** É o ponto decisivo do Cliente que move o serviço para a fase de negociação (**Andamento**). |
| **Controle de Status do Serviço (Análise, Andamento, Concluído)** | **Gestão de Fluxo:** Essencial para que o sistema saiba em qual fase o serviço se encontra e quais ações estão liberadas. |
| **Liberação condicional do botão "WhatsApp/Ligar" (Apenas Cliente)** | **Segurança e Controle:** Permite que **apenas o Cliente** inicie o contato offline após a contratação, mantendo o controle da plataforma. |
| **Botão "Acordo Fechado! Iniciar Serviço" e Confirmação de Início** | **Validação:** Formaliza o acordo negociado offline e confirma o início da prestação do serviço no App. |
| **Botão "Serviço Finalizado"** | **Encerramento:** Necessário para dar o serviço como concluído e desencadear a próxima fase crítica (Avaliação). |
| **Tela de Avaliação 5 Estrelas Simples** | **Feedback:** Componente crucial para a coleta de dados de confiança. |
| **Lógica de Ranqueamento (melhorar ranking)** | **Objetivo de Negócio:** Algoritmo que utiliza as avaliações e portfólio para priorizar profissionais, combatendo a inconstância no trabalho. |
| **Chat/Comunicação Interna (Apenas Suporte)** | **Atendimento:** Canal primário para o profissional de suporte se comunicar com o cliente que precisa de ajuda. |
| **Funcionalidade de Registro de Suporte (log/ficha)** | **Controle Gerencial:** Permite registrar os atendimentos realizados, fundamental para medir a qualidade e o tempo de resposta do suporte. |
| **Interface de Cadastro e Atualização de Produtos (Lojista)** | **Catálogo:** Permite ao lojista manter seu estoque e preços visíveis e atualizados na seção "Onde Comprar". |
| **Funcionalidade para Divulgar Promoções/Destaques** | **Marketing:** Permite que o lojista promova ofertas para atrair Clientes e Profissionais. |
| **Integração de Comunicação (WhatsApp/Mensagens, Lojista)** | **Vendas:** Permite ao Cliente contatar o Lojista para cotação e compra de materiais (offline). |
| **Seção de Acompanhamento de Vendas/Histórico de Pedidos (Lojista)** | **Gestão:** Permite ao lojista visualizar o desempenho e o histórico de pedidos/consultas recebidas pelo App. |

## Should have (Importantes) - DEVERIA TER

Estes são recursos **importantes**, mas não essenciais. Sua ausência degrada a experiência ou a eficiência, mas o produto principal ainda é utilizável.

| Requisito | Explicação e Função |
| :--- | :--- |
| **Liberação condicional do Contato (WhatsApp/Ligar) APENAS para o Cliente** | **Controle:** Garante que o Cliente inicie a conversa após a contratação, um requisito crucial para a gestão da plataforma. |
| **Visualização de Perfis/Candidatos pelo Cliente** | **Usabilidade:** Oferece ao Cliente uma lista clara e organizada de todos os profissionais interessados no seu anúncio. |
| **Agendamento da tela de Avaliação (na próxima abertura do App)** | **UX (Experiência do Usuário):** Prática que aumenta a chance de coleta de feedback, lembrando o Cliente em um momento oportuno. |
| **Funcionalidade de Seleção/Redirecionamento do Canal de Comunicação (Suporte)** | **Flexibilidade:** Permite que o suporte mude do chat interno para um canal preferido pelo usuário (ex.: WhatsApp), aumentando a satisfação. |
| **Campos de Registro de Métricas (Tempo, Nível de Satisfação) na Ficha de Suporte** | **Gestão de Qualidade:** Adiciona campos específicos na ficha de suporte para que a empresa possa analisar a performance do atendimento. |
| **Sistema de Ranqueamento de Produtos/Promoções** | **Destaque:** Permite que o lojista promova itens mais relevantes ou em oferta de forma estratégica para os usuários. |
| **Notificações de Novas Mensagens/Consultas (Lojista/Suporte)** | **Agilidade:** Alerta o lojista ou suporte sobre novas interações, sendo vital para o tempo de resposta. |
| **Interface de Visualização de Feedbacks/Avaliações (Lojista)** | **Melhoria Contínua:** Permite que o lojista veja as notas e comentários dos clientes para ajustar seus serviços ou ofertas. |

##  Could have (Desejáveis) - PODERIA TER

Estes são recursos **não essenciais** que funcionam como diferenciais na experiência do usuário e só devem ser implementados se houver tempo e recursos.

| Requisito | Explicação e Função |
| :--- | :--- |
| **Funcionalidade de tirar fotos para o Portfólio ou galeria** | **Valor Agregado:** Facilita a criação de conteúdo visual pelo profissional, enriquecendo o perfil. |
| **Exibição do Portfólio do profissional (para o Cliente)** | **Detalhe:** Apresenta as imagens do portfólio de forma atrativa na visualização do perfil. |
| **Guia "Onde Comprar em Itacoatiara"** | **Conveniência:** Resolve um problema secundário do Cliente (encontrar materiais) com alto valor agregado. |
| **Integração com WhatsApp (para iniciar conversa diretamente)** | **Atalho de UX:** Simplifica o processo de transição do App para o WhatsApp, facilitando a vida do usuário. |
| **Opção de Chamada de Áudio (via App, suporte)** | **Qualidade de Suporte:** Oferece um canal de comunicação mais rico para resolver problemas complexos. |

##  Won't have (Fora do Escopo Atual) - NÃO TERÁ – POR ENQUANTO

Estes são requisitos que **não serão desenvolvidos** nesta versão, pois estão fora do escopo ou não geram valor imediato. Serão descartados ou adiados.

| Requisito | Explicação e Motivo |
| :--- | :--- |
| **Pagamento dentro do App** | **Motivo:** O projeto prevê que o pagamento seja realizado **offline** (Pix ou em dinheiro), fora da plataforma. |
| **Chat interno (dentro do App) para negociação** | **Motivo:** A negociação é direcionada e controlada via **WhatsApp/Ligar**, tornando o chat interno redundante para este fim. |
| **Base de Conhecimento/FAQ no App** | **Motivo:** Módulo de suporte mais avançado, não essencial para a função de atendimento básico. |
| **Sistema de Transferência de Atendimento (para outro Suporte)** | **Motivo:** Funcionalidade de gestão de suporte complexa, adiada para futuras versões. |
| **Módulo de Entrega/Logística** | **Motivo:** O escopo do lojista foca em divulgação e cotação, não na entrega física dos produtos. |
| **Processamento de Pagamento (Gateway)** | **Motivo:** Diretamente ligado ao "Pagamento dentro do App," o que está fora do escopo atual. |
