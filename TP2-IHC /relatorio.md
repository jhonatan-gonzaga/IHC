k# Relatório - TP2: IHC e Machine Learning

**Equipe:**
- 22552726 - Alyce Benevides Lima
- 22552010 - Jhonatan Gonzaga Galdino
- 22550449 - Oliviê Kalil de Menezes Miranda
- 22550444 - Rodrigo Torres Rodrigues
- 22552381 - Victor dos Santos Cardoso
#  Classificação Supervisionada do Engajamento e Dificuldade de Alunos como Indicadores de UX em Sistemas EAD

##  1. Definição do Problema

###  Contexto  
O **Ensino a Distância (EAD)** consolidou-se como uma modalidade essencial na educação contemporânea, impulsionada pela transformação digital e pelo uso crescente de plataformas virtuais.  
Esses ambientes de aprendizagem geram, continuamente, uma grande quantidade de **dados de interação** — tempo em vídeos, número de acessos, progresso em módulos, entre outros.

Entretanto, a ausência de contato presencial cria uma lacuna importante: a dificuldade em **identificar quando um aluno está desmotivado ou com dificuldades**.  
Enquanto, em uma sala de aula tradicional, o professor pode perceber sinais visuais e comportamentais de desengajamento, no ambiente digital, esse aluno torna-se “invisível” até que seu desempenho caia ou ele abandone o curso.  

Essa invisibilidade contribui para **altas taxas de evasão**, tornando urgente o desenvolvimento de sistemas capazes de reconhecer padrões de interação que indiquem dificuldades de aprendizagem.

---

###  Motivação  
A motivação deste trabalho reside na necessidade de converter dados operacionais em indicadores pedagógicos úteis.
<br>
O objetivo é aplicar algoritmos de aprendizado de máquina, utilizando a ferramenta Weka, para treinar um modelo capaz de prever o status de engajamento do aluno, permitindo intervenções pedagógicas proativas antes que o desempenho seja comprometido. 

Com isso, pretende-se:

-  **Identificar riscos em tempo real:** reconhecer sinais precoces de desorientação ou desmotivação.  
-  **Permitir intervenções personalizadas:** alertar tutores para contatar o aluno de forma direcionada.  
-  **Reduzir a evasão:** agir preventivamente, mantendo o aluno engajado no processo de aprendizagem.  
-  **Melhorar a experiência educacional:** promover um ambiente mais empático e adaptativo.  

---

### Atributos Preditores  

| **Atributo** | **Tipo** | **Descrição** |
|---------------|-----------|---------------|
| `paginas_visitadas` | Numérico | Total de telas ou recursos acessados na sessão. |
| `revisitas_painel_principal` | Numérico | Quantidade de retornos à página inicial do curso. |
| `tempo_medio_recurso` | Numérico | Tempo médio (em segundos) gasto em cada recurso educacional. |
| `uso_busca` | Numérico | Número de vezes que o aluno utilizou a busca interna da plataforma. |
| `progresso_no_modulo` | Numérico | Grau de avanço na sequência de aulas (ex: Aula 1 → Aula 3 = progresso 3). |
| `desvio_sequencia` | Numérico | Número de vezes que o aluno acessou uma aula fora da ordem recomendada. |

---

### Classe-Alvo  

- **Nome:** `status_aluno`  
- **Tipo:** Binária  
- **Valores possíveis:**  
  - `com_dificuldade`  
  - `progredindo`  
- **Objetivo:**  
  Prever se o aluno está enfrentando **dificuldades de navegação/aprendizagem** ou **progredindo adequadamente** ao longo do curso.  

---

## 2. Regras de Geração da Classe-Alvo  

A classe-alvo foi definida com base em regras lógicas que traduzem padrões comportamentais observados em plataformas EAD.  

### Regra 1 — `status_aluno = com_dificuldade`  
Um aluno é classificado como **com dificuldade** quando demonstra **desorientação e falta de progresso**.

**Regra Lógica:**  
SE<br>
&nbsp;&nbsp;&nbsp;&nbsp;(revisitas_painel_principal > 3)E<br>
&nbsp;&nbsp;&nbsp;&nbsp;(progresso_no_modulo < 2) E<br>
&nbsp;&nbsp;&nbsp;&nbsp;(desvio_sequencia > 2)<br>
ENTÃO<br>
&nbsp;&nbsp;&nbsp;&nbsp;status_aluno = com_dificuldade


**Justificativa:**  
O aluno retorna frequentemente ao início do curso, não avança significativamente nos módulos e acessa conteúdos fora de sequência — um comportamento típico de desorganização e confusão cognitiva.  

---

### Regra 2 — `status_aluno = progredindo`  
Um aluno é classificado como **progredindo** quando apresenta **avanço consistente e comportamento focado**.

**Regra Lógica:**  
SE <br>
&nbsp;&nbsp;&nbsp;&nbsp;(progresso_no_modulo > 4) E <br>
&nbsp;&nbsp;&nbsp;&nbsp;(tempo_medio_recurso > 30) E <br>
&nbsp;&nbsp;&nbsp;&nbsp;(desvio_sequencia = 0) <br>
ENTÃO <br>
&nbsp;&nbsp;&nbsp;&nbsp;status_aluno = progredindo


**Justificativa:**  
Esse aluno demonstra evolução contínua no curso, dedica tempo adequado ao estudo e segue a trilha pedagógica proposta, indicando engajamento e autodisciplina.  

---

## 3. Descrição da Base de Dados Sintética  

A base de dados foi gerada como artefato da **Etapa 2** do projeto, utilizando um modelo de linguagem para simular registros de comportamento estudantil.  

| **Item** | **Descrição** |
|-----------|----------------|
| **Ferramenta Utilizada** | ChatGPT |
| **Formato do Arquivo** | `.arff` — compatível com o software **Weka** |
| **Número de Instâncias** | 200 registros (mínimo exigido) |
| **Número de Atributos** | 6 preditores + 1 classe-alvo (total: 7) |
| **Link para a Base** | [dataset.arff](base_sintetica.arff) |
---
### 3.1 Validação e Verificação  
Após a criação, o arquivo `dataset.csv` foi testado no ambiente **Google Colab**, utilizando o notebook disponível no link abaixo:  
🔗 [Verificação das Regras do Dataset](https://colab.research.google.com/drive/1Hs3Fev6L1sotBWnzCtZ_zhay3UvUWXMM?usp=sharing)  
<img width="779" height="338" alt="image (1)" src="https://github.com/user-attachments/assets/1611751c-fc85-42d3-8992-450ea092fae0" />
<br>
O código realizou uma verificação automática das instâncias, assegurando que todos os registros estavam rotulados corretamente conforme as regras definidas. 

### 3.2 Distribuição das Classes  

A distribuição das classes confirma o **balanceamento** entre as categorias:  

| Classe          | Quantidade |
|-----------------|-------------|
| com_dificuldade | 100         |
| progredindo     | 100         |
| **Total**       | **200**     |

## 4. Descrição dos Experimentos no Weka
A análise de base "dataset_EAD_classificacao.arff" no Weka teve como objetivocompreender o comportamentoe e o desempenho de alunos em um ambiente de Ensino a Distância (EAD), os dados foram importados no módulo Explorer, onde foi poasível observar estatísticas básicas e histogramas dos atributos. Essa etapa permitiu identificar diferenças iniciais entre alunos “progredindo” e “com dificuldade”, especialmente nos atributos ligados ao engajamento, como número de páginas visitadas, tempo médio nos recursos e revisitas ao painel principal.

Em seguida, na aba Visualize, foi gerada a matriz de dispersão, que mostrou graficamente as relações entre as variáveis. Observou-se que maior interação com os recursos e uso da busca estavam relacionados ao progresso, enquanto revisitas excessivas e desvio da sequência de estudo estavam associados às dificuldades. Essa análise visual evidenciou dois perfis distintos de alunos: os mais organizados e engajados, e os que apresentavam comportamentos desordenados e menor dedicação.

## 4.1 Exploração dos Dados
Na aba “Visualize” do WEKA, foi possível observar de forma clara as relações entre os principais atributos do conjunto de dados e a classe-alvo status_aluno, que diferencia alunos progredindo (vermelho) e com_dificuldade (azul). Os gráficos de dispersão revelam padrões bem definidos de comportamento, indicando correlações entre engajamento nas atividades e desempenho no curso.
-> IMAGEM DA ABA "VISUALIZE" "PANORAMA"

Na relação entre revisitas_painel_principal e uso_busca, nota-se que os alunos com_dificuldade tendem a revisitar mais vezes o painel e fazer pouco uso da busca. Já os alunos progredindo se concentram em níveis mais altos de uso da busca e revisitas menos frequentes, o que pode indicar uma navegação mais direcionada e eficiente.
-> IMAGEM DA RELAÇAO "revisitas_painel_principal e uso_busca,"

O gráfico entre tempo_medio_recurso e progresso_no_modulo evidencia uma forte correlação positiva: quanto maior o tempo médio dedicado aos recursos, maior o progresso. Os alunos progredindo se concentram nas faixas mais altas desses atributos, enquanto os com_dificuldade aparecem agrupados nas menores médias. Esse padrão reforça a ideia de que o engajamento e o tempo de estudo influenciam diretamente o desempenho.
-> IMAGEM DA RELAÇÃO "tempo_medio_recurso e progresso_no_modulo"

Na comparação de uso_busca com desvio_sequencia, percebe-se que alunos com_dificuldade apresentam maiores desvios da sequência esperada de estudo e menor uso da busca, sugerindo falta de foco ou navegação desordenada. Em contrapartida, os progredindo mostram comportamento mais estruturado, com baixo desvio e maior utilização da ferramenta de busca.
-> IMAGEM DA RELAÇÃO "uso_busca com desvio_sequencia"

Por fim, a matriz de dispersão da aba “Visualize” apresenta de forma geral dois agrupamentos bem distintos de acordo com a classe. As variáveis tempo_medio_recurso, uso_busca e progresso_no_modulo estão fortemente associadas a bons resultados, enquanto revisitas_painel_principal e desvio_sequencia aparecem mais ligados aos alunos com dificuldades. Esses padrões visuais revelam uma separação nítida entre os perfis comportamentais, indicando que o desempenho pode ser previsto a partir das interações registradas na plataforma.

## 4.2 Metodologia de Classificação
Utilizamos o Software WEKA para dividir os dados. (O WEKA (Waikato Environment for Knowledge Analysis) é um software de código aberto usado para mineração de dados e aprendizado de máquina. Ele oferece uma interface gráfica simples e ferramentas para pré-processamento, classificação, regressão, agrupamento, visualização e seleção de atributos. Desenvolvido na Universidade de Waikato, o WEKA é amplamente utilizado em pesquisas e ensino por permitir a aplicação prática de algoritmos de IA sem necessidade de programação complexa).
### Abordagem de Avaliação:
O datasete exigia o uso do Hold-out (66% para treino e 34% para teste), utilizei os seguintes passos: 
1. Carregar o conjunto de dados no painel "Preprocess".
2. Ir até a aba "Classify".
3. Em "Teste options", selecionar "Porcentage split".
4. Definir o valor 66% (WEKA usurá 66% para treino e 34% para teste).
5. Escolher algoritmo desejado em "Classifier" e clicar em "Start".

### Algoritmos Utilizados: 
- **J48 (Arvore de Decisão)**
- **IBk (k-NN)**
- **Naive Bayes**
- **ZeroR (baseline)**
- **OneR (baseline)**

---

## 5. Resultados

### 5.1. Tabela Comparativa de Acurácia

A tabela a seguir apresenta o percentual de acertos (acurácia) de cada um dos 5 algoritmos na base de teste.

| Algoritmo | Acurácia |
| :--- | :--- |
| J48 | 100% |
| IBk | 100% |
| Naive Bayes | 100% |
| OneR | 100% |
| ZeroR | 50% |

---

### 5.2. Matrizes de Confusão

Abaixo estão as matrizes de confusão para os algoritmos principais (J48, IBk, Naive Bayes). Para esta análise, a classe "com_dificuldade" foi definida como a classe Positiva.

**J48**

<img width="232" height="106" alt="image" src="https://github.com/user-attachments/assets/1ba8c8e7-6022-4055-841b-b29cf5479307" />

* **Verdadeiros Positivos (VP):** 38
* **Falsos Positivos (FP):** 0
* **Verdadeiros Negativos (VN):** 30
* **Falsos Negativos (FN):** 0
* **Comentário:** O modelo J48 acertou todas as 38 instâncias da classe "com_dificuldade" e todas as 30 instâncias da classe "progredindo". O modelo não confundiu nenhuma instância.

**IBk**

<img width="232" height="106" alt="image" src="https://github.com/user-attachments/assets/fcd83e05-fd17-41b7-8533-2467f14315a2" />

* **Verdadeiros Positivos (VP):** 100
* **Falsos Positivos (FP):** 0
* **Verdadeiros Negativos (VN):** 100
* **Falsos Negativos (FN):** 0
* **Comentário:** O modelo IBk acertou todas as 100 instâncias da classe positiva (Verdadeiros Positivos) e todas as 100 instâncias da classe negativa (Verdadeiros Negativos), não cometendo nenhum erro de classificação.

**Naive Bayes**

<img width="233" height="107" alt="image" src="https://github.com/user-attachments/assets/93086a85-a7b4-44bd-82e7-ade5f750a15d" />

* **Verdadeiros Positivos (VP):** 38
* **Falsos Positivos (FP):** 0
* **Verdadeiros Negativos (VN):** 30
* **Falsos Negativos (FN):** 0
* **Comentário:** O modelo Naive Bayes acertou todas as 38 instâncias da classe "com_dificuldade" e todas as 30 instâncias da classe "progredindo". O modelo não confundiu nenhuma instância.

### 5.3. Árvore de Decisão (J48)

<img width="901" height="347" alt="image" src="https://github.com/user-attachments/assets/52c6d7f2-4884-4598-8e23-56e032de483c" />

---

# 6. Análise Crítica dos Resultados

Como podemos ver na tabela presente na seção 5.1, todos os algoritmos, com a exceção do ZeroR apresentaram acurácias perfeitas, tendo 100% de acertos nas suas previsões para a parte da base de dados destinada para sua previsão. Podemos perceber que o ZeroR apresentou 50% de acerto pois metade da base de dados tem como classificação "Progredindo" (100 instâncias) e a outra metade é classificada como "Com dificuldade" (novamente, 100 instâncias). Ou seja, ele apenas pegou a classe alvo com maior quantidade de instâncias, que neste caso pode ser as duas, e presumiu que todas seriam daquela classe alvo.

O OneR também teve 100% de acurácia, assim como todos os algoritmos que não eram baseline. Como o OneR pega apenas o atributo mais discriminatório, podemos concluir que há pelo menos um atributo que discrimina perfeitamente as duas classificações.
