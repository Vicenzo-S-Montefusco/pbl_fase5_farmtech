# pbl_fase5_farmtech

# FarmTech Solutions – Análise Exploratória e Tendências de Safra

## Contexto
Este projeto faz parte da **Fase 5 do PBL FIAP**.  
O cenário envolve a **FarmTech Solutions**, que presta serviços de Inteligência Artificial para uma fazenda de médio porte (200 hectares).  
O objetivo é analisar os dados de clima e solo, explorar tendências de rendimento das culturas e identificar cenários discrepantes (outliers).

## Escopo do Projeto
- **Análise exploratória dos dados (EDA)**  
- **Identificação de tendências de rendimento via clusterização (KMeans + PCA)**  
- **Detecção de cenários discrepantes (outliers com DBSCAN e boxplots)**  
- **Documentação e vídeo explicativo dessa análise**
[adicionar suas partes]

*(Os modelos preditivos supervisionados fazem parte de outra etapa do grupo e não estão neste notebook.)*

## Dataset
Arquivo: `crop_yield.csv`  
Variáveis principais:
- Cultura  
- Precipitação (mm/dia)  
- Umidade específica a 2m (g/kg)  
- Umidade relativa a 2m (%)  
- Temperatura a 2m (ºC)  
- Rendimento (ton/ha)  

## Principais Etapas da Análise
1. **Exploração inicial** – estatísticas descritivas, distribuições e correlações.  
2. **Clusterização (KMeans + PCA)** – identificação de tendências de rendimento e agrupamentos distintos de culturas.  
3. **Detecção de outliers (DBSCAN + análises estatísticas)** – identificação de pontos discrepantes de produtividade.  
4. **Exportação de casos suspeitos** – arquivo adicional com registros extremos.  

## Estrutura do Repositório
- `vicenzo_montefusco_rm563810_pbl_fase4.ipynb` → Notebook completo com a análise.  
- `crop_yield.csv` → Base de dados fornecida.  
- `suspected_outliers_and_extremes.csv` → Registros suspeitos/exportados como potenciais **outliers**.  

### Sobre o arquivo de outliers
O arquivo `suspected_outliers_and_extremes.csv` contém as linhas do dataset que apresentaram **valores discrepantes** segundo:
- Análise estatística (boxplots, z-score)  
- Clusterização DBSCAN  

Esse material serve como **evidência** dos cenários incomuns de rendimento e pode apoiar decisões futuras da fazenda, como investigar condições climáticas anômalas ou problemas pontuais no solo.

## 🎥 Demonstração em Vídeo
➡ [Link para o vídeo no YouTube](COLOQUE_AQUI_SEU_LINK) *(modo não listado)*

## Conclusões
- Foram identificadas **tendências claras** nos rendimentos com base em clima e solo.  
- Clusters distintos de produtividade foram encontrados, revelando perfis diferentes de culturas.  
- Alguns **outliers** foram detectados, que podem indicar erros de coleta ou situações reais de stress agrícola.  
- Limitações: dataset relativamente pequeno, análise restrita a variáveis fornecidas.  
