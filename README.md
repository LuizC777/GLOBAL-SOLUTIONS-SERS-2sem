# Projeto: Otimização Sustentável de Energias Renováveis com Análise e Automação Inteligente

## Integrantes
- Luiz Claro Lima Rm 563014  
- Gabriel Romão Soares Rm 563378  
- Leonardo Luster Gomes Rm 564448 

---

## Descrição Geral do Projeto
Este projeto tem como objetivo aplicar técnicas de análise de dados e modelagem inteligente para otimizar o uso de fontes de energia renovável.  
A proposta contribui para práticas sustentáveis aplicáveis ao contexto de trabalho, explorando automação, integração de dados climáticos e previsão de eficiência energética.  
A base de dados utilizada contém registros de diferentes fontes de energia renovável, acompanhados por variáveis climáticas como temperatura, velocidade do vento, radiação solar e precipitação.  

O trabalho é dividido em duas etapas principais:
1. **Análise de Dados:** exploração detalhada do conjunto de dados, identificação de padrões e fatores que afetam a eficiência energética.  
2. **Solução Sustentável:** aplicação de um modelo preditivo e de um sistema IoT simulado para otimização do uso e automação das fontes de energia.

---

## Instruções de Execução

### 1. Requisitos
Antes de executar o projeto, instale as seguintes bibliotecas Python:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
---
## 1. Análise de Dados

A análise de dados tem como objetivo compreender os fatores que influenciam a eficiência das fontes de energia renovável.  
Foram exploradas as principais variáveis do conjunto de dados e suas relações com a variável alvo **Efficiency_Ratio**, que representa a eficiência de geração.

### Estrutura dos Dados
A base inclui as seguintes colunas principais:
- **Temperature_C**: temperatura ambiente em graus Celsius.  
- **Wind_Speed_m_s**: velocidade média do vento em metros por segundo.  
- **Solar_Radiation_kWh_m2**: radiação solar diária em kWh/m².  
- **Rainfall_mm**: precipitação em milímetros.  
- **Energy_Source**: tipo de fonte renovável (solar, eólica, etc).  
- **Efficiency_Ratio**: percentual de eficiência da produção de energia.  

### Principais Etapas da Análise
1. **Inspeção e limpeza dos dados:** verificação de valores ausentes e estrutura das colunas.  
2. **Análise estatística descritiva:** cálculo de médias, desvios e faixas de variação.  
3. **Matriz de correlação:** identificação de relações entre variáveis climáticas e eficiência.  
4. **Visualizações individuais:**  
   - Gráfico de dispersão entre **temperatura** e **eficiência** mostrou tendência de queda de eficiência em temperaturas elevadas.  
   - **Velocidade do vento** apresentou correlação positiva com eficiência em turbinas eólicas.  
   - **Radiação solar** teve relação direta com eficiência em sistemas fotovoltaicos.  
   - **Chuva** indicou possível impacto negativo devido à obstrução e resfriamento dos equipamentos.

### Interpretação dos Resultados

A análise dos dados revelou que a eficiência das fontes de energia renovável é fortemente influenciada por condições climáticas específicas, destacando-se quatro fatores principais: temperatura, radiação solar, velocidade do vento e precipitação.

Os resultados indicaram que **temperaturas mais elevadas** tendem a reduzir a eficiência dos sistemas fotovoltaicos. Esse efeito ocorre devido ao superaquecimento dos painéis solares, que diminui sua capacidade de conversão de energia luminosa em elétrica. Já temperaturas amenas mantêm os painéis em uma faixa de desempenho mais estável.

A **radiação solar** mostrou-se o fator de maior impacto positivo na eficiência, o que confirma a dependência direta das tecnologias solares em relação à intensidade de luz incidente. Entretanto, níveis excessivos de radiação combinados com altas temperaturas podem gerar perdas por superaquecimento, reforçando a importância de mecanismos de resfriamento e monitoramento térmico.

No caso da **velocidade do vento**, observou-se uma correlação positiva com a eficiência das turbinas eólicas. Ventos constantes e de intensidade moderada promovem maior geração elétrica. Por outro lado, rajadas muito intensas podem causar sobrecarga mecânica e exigem o uso de sistemas de controle automático para limitar a rotação.

A **precipitação** apresentou relação negativa com a eficiência. Chuvas intensas reduzem a incidência solar, provocam umidade excessiva e podem interferir no desempenho de painéis e turbinas. Em contrapartida, chuvas leves ocasionais podem auxiliar na limpeza dos módulos solares, evitando acúmulo de poeira e melhorando o rendimento em períodos subsequentes.

De forma geral, os gráficos e correlações permitiram identificar padrões que indicam **quais condições ambientais favorecem ou comprometem o desempenho energético**. Essas informações fundamentam a construção de modelos preditivos e de sistemas automatizados capazes de ajustar a operação conforme o clima, maximizando o aproveitamento das fontes renováveis e minimizando perdas por ineficiência.

