# 🧬 Tech Challenge 2 – FIAP  
## Otimização de Rede Neural com Algoritmo Genético (GA) – Dataset Iris  

Projeto individual da Fase 2 da pós-graduação em Inteligência Artificial para Devs – FIAP.  
Neste desafio, foi desenvolvido um modelo de **Algoritmo Genético** para otimizar a **arquitetura de uma rede neural** com o objetivo de classificar corretamente flores do **dataset Iris**.

---

## 📹 Demonstração do Projeto  
▶️ Assista ao vídeo explicativo no YouTube:  
[https://youtu.be/BEYjdcwEJm4](https://youtu.be/BEYjdcwEJm4)

---

## 📂 Acesse o Código no Google Colab  
🔗 [Notebook no Google Colab](https://colab.research.google.com/drive/1ANClljztX5Y45omNk98aQjzVdrvYqSvV)

---

## 📘 Sobre o Problema

O **dataset Iris** é um conjunto clássico de Machine Learning que contém 150 amostras de flores divididas em 3 espécies. Cada flor é representada por 4 atributos:
- Comprimento da sépala
- Largura da sépala
- Comprimento da pétala
- Largura da pétala

O objetivo é **classificar corretamente a espécie da flor** a partir desses atributos.

---

## 🤖 O que o GA Otimiza?

O Algoritmo Genético busca encontrar a melhor combinação de:
- 🔢 Número de neurônios na camada oculta 1
- 🔢 Número de neurônios na camada oculta 2
- ⚙️ Função de ativação da camada 1 (`0 = relu`, `1 = sigmoid`, `2 = tanh`)
- ⚙️ Função de ativação da camada 2

Cada indivíduo da população representa uma possível configuração da rede neural.

---

## ⚙️ Funcionamento do Algoritmo Genético

- `create_individual()`: cria um indivíduo com parâmetros aleatórios  
- `decode_individual()`: monta e treina uma rede neural com base nos genes  
- `fitness`: acurácia do modelo no conjunto de teste  
- `mutate()`: altera aleatoriamente um dos genes  
- `crossover()`: combina dois indivíduos para gerar filhos  

A população evolui por 10 gerações com base em seleção, cruzamento e mutação.

---

## 📈 Resultados

O algoritmo encontrou rapidamente uma solução ótima:
- **Geração 1**: Acurácia de 96,67%
- **Geração 2 em diante**: Acurácia de **100% mantida** até a Geração 10

### 📊 Gráfico da Evolução da Acurácia:
> O gráfico gerado no notebook mostra a evolução da acurácia do melhor indivíduo em cada geração. A melhoria é clara e a convergência ocorre rapidamente.

---

## ✅ Conclusão Crítica

O Algoritmo Genético se mostrou eficaz ao:
- Otimizar automaticamente a estrutura da rede neural
- Alcançar acurácia máxima com poucas gerações
- Demonstrar estabilidade da solução ao longo do tempo

**Limitações:** tempo de execução e variação aleatória nos resultados podem ocorrer.

---

## 👨‍💻 Autor

**Luís Felipe Alves Silva**  
RM: 363734  
Pós-graduação FIAP – IA para Devs
