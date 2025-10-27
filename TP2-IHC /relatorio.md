# Relatório - TP2: IHC e Machine Learning

**Equipe:**
- 22552726 - Alyce Benevides Lima
- 22552010 - Jhonatan Gonzaga Galdino
- 22550449 - Oliviê Kalil de Menezes Miranda
- 22550444 - Rodrigo Torres Rodrigues
- 22552381 - Victor dos Santos Cardoso
#  Análise de Engajamento e Dificuldade de Alunos em Ambientes de Ensino a Distância (EAD)

##  1. Definição do Problema

###  Contexto  
O **Ensino a Distância (EAD)** consolidou-se como uma modalidade essencial na educação contemporânea, impulsionada pela transformação digital e pelo uso crescente de plataformas virtuais.  
Esses ambientes de aprendizagem geram, continuamente, uma grande quantidade de **dados de interação** — tempo em vídeos, número de acessos, progresso em módulos, entre outros.

Entretanto, a ausência de contato presencial cria uma lacuna importante: a dificuldade em **identificar quando um aluno está desmotivado ou com dificuldades**.  
Enquanto, em uma sala de aula tradicional, o professor pode perceber sinais visuais e comportamentais de desengajamento, no ambiente digital, esse aluno torna-se “invisível” até que seu desempenho caia ou ele abandone o curso.  

Essa invisibilidade contribui para **altas taxas de evasão**, tornando urgente o desenvolvimento de sistemas capazes de reconhecer padrões de interação que indiquem dificuldades de aprendizagem.

---

###  Motivação  
A motivação deste trabalho reside na necessidade de **converter dados operacionais em indicadores pedagógicos úteis**.  
O objetivo é criar um modelo capaz de **prever o status de engajamento do aluno**, permitindo **intervenções pedagógicas proativas** antes que o desempenho seja comprometido.  

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
SE (revisitas_painel_principal > 3)
E (progresso_no_modulo < 2)
E (desvio_sequencia > 2)
ENTÃO status_aluno = com_dificuldade


**Justificativa:**  
O aluno retorna frequentemente ao início do curso, não avança significativamente nos módulos e acessa conteúdos fora de sequência — um comportamento típico de desorganização e confusão cognitiva.  

---

### Regra 2 — `status_aluno = progredindo`  
Um aluno é classificado como **progredindo** quando apresenta **avanço consistente e comportamento focado**.

**Regra Lógica:**  
SE (progresso_no_modulo > 4)
E (tempo_medio_recurso > 30)
E (desvio_sequencia = 0)
ENTÃO status_aluno = progredindo


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
A análise de base "dataset_EAD_classificacao.arff" no Weka teve como objetivocompreender o comportamentoe e o desempenho de alunos em um ambiente de Ensino a Distância (EAD), os dados foram importados no módulo Explorer, onde foi poasível observar estatísticas básicas e histogramas dos atributos. Essa etapa permitiu identificar diferenças 
