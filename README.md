# Mensuração em Artes-terapia: Evidências Psicométricas e Validação _In Silico_

Este repositório contém os dados, códigos e modelos referentes à adaptação transcultural e validação psicométrica da escala **SERATS (Self-Expression and Emotion Regulation in Art Therapy Scale)** utilizando métodos de **Psicometria Generativa** e Inteligência Artificial.

## 📂 Estrutura do Repositório

O projeto está organizado para garantir a total reprodutibilidade dos achados:

### 1. Dados e Relatórios de Validade (`.xlsx`, `.csv`)
*   **`SERATS.csv` / `SERATS.xlsx`**: Banco de dados empírico utilizado nas análises.
*   **`Relatorio_BackTranslation_Arteterapia0906.xlsx`**: Log detalhado de todo o processo de tradução e retrotradução realizado pelos agentes de IA.
*   **`CVC_Final_Arteterapia0906.xlsx`**: Planilha com o cálculo do Coeficiente de Validade de Conteúdo (CVC) gerado pelo comitê de juízes virtuais.

### 2. Modelos e Inteligência Artificial (`.rds`, `.ipynb`)
*   **`mod_mestre_cohere_en.rds`**: O "Modelo Especialista" treinado via Elastic Net. Este modelo é o coração da validação *in silico*, capaz de prever correlações humanas a partir de interações vetoriais de *embeddings*. 
*   **`BackTranslationLLM_SERATS.ipynb`**: Notebook (Google Colab) contendo a arquitetura agêntica utilizada para a tradução e auditoria do instrumento.

### 3. Scripts de Análise e Resultados (`.Rmd`, `.html`, `.png`)
*   **`Analises.Rmd`**: Código-fonte em R contendo todas as etapas estatísticas (CFA, Análise de Redes, DFI e NCT).
*   **`Analises.html`**: Relatório gerado (Knit) que permite visualizar todas as saídas estatísticas e gráficos sem a necessidade de rodar o código.
*   **`Comparacao_Redes_SERATS_Alta.png`**: Visualização de alta resolução da equivalência topológica entre as redes em Inglês e Português.
*   **`Figura_Comparacao_Redes_BW.png`**: Versão em tons de cinza preparada para publicação impressa.

## 🛠️ Como Utilizar

1. **Reprodutibilidade:** Para replicar as análises estatísticas, utilize o arquivo `Analises.Rmd` no RStudio. Certifique-se de ter o arquivo `mod_mestre_cohere_en.rds` na mesma pasta para o carregamento do modelo sintético.
2. **IA Agêntica:** O arquivo `.ipynb` pode ser carregado diretamente no Google Colab para testes com novos itens ou outros instrumentos.


## Como citar


Pedrosa, F. (2026). *Mensuração em Artes-terapia: Evidências Psicométricas e Validação In Silico*. GitHub Repository. https://github.com/FredPedrosa/SERATS/

## Autor

*   **Frederico Pedrosa**
*   fredericopedrosa@ufmg.br

## 📜 Licença

Este projeto está licenciado sob a **Licença MIT** - veja o arquivo [LICENSE](LICENSE) para detalhes. Esta é uma licença permissiva que permite o uso, cópia e modificação para fins acadêmicos e profissionais, desde que mantidos os créditos originais.

---
**Contato:** Para dúvidas sobre a metodologia de Psicometria Generativa ou o protocolo *in silico*, sinta-se à vontade para abrir uma *Issue* ou entrar em contato.
