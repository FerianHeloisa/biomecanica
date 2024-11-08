# Projeto de Reconstrução 3D da Trajetória de uma Bola

Este projeto realiza a reconstrução 3D da trajetória de uma bola chutada, utilizando vídeos capturados por duas câmeras. A partir dos vídeos fornecidos, são extraídas as coordenadas 2D da bola e dos pontos de calibração, que são usadas para calcular a trajetória em 3D via DLT (Transformação Linear Direta).

## Estrutura do Projeto

- **Vídeos**:
  - `c1.avi` e `c2.avi`: vídeos das câmeras 1 e 2 que mostram o movimento da bola.
  - `c1cal.avi` e `c2cal.avi`: vídeos de calibração para definir pontos de referência e permitir a reconstrução 3D.

- **Código Python (Google Colab)**: Script que executa a leitura dos vídeos, calibração, e reconstrução 3D da trajetória da bola.

## Funcionalidades

1. **Calibração**: Realiza a transformação das coordenadas 2D dos pontos de calibração nos vídeos para um sistema de coordenadas 3D usando DLT.
2. **Extração de Coordenadas 2D**: Processa os vídeos para identificar a posição da bola em cada quadro.
3. **Reconstrução da Trajetória 3D**: Utiliza as coordenadas 2D e a calibração para reconstruir a trajetória 3D da bola.
4. **Visualização e Análise**: Gera gráficos e salva resultados para análise da trajetória.

## Passo a Passo para Executar o Projeto

1. **Carregar o Script no Google Colab**:
   - Importe o código para um notebook no Google Colab.
   
2. **Importar Bibliotecas Necessárias**:
   - O script requer `numpy`, `pandas`, `opencv`, `matplotlib`, `scipy`, e `mpl_toolkits`. Execute `!pip install` para instalar pacotes que não estejam no ambiente do Colab.

3. **Carregar os Arquivos de Vídeo**:
   - Faça o upload dos arquivos `c1.avi`, `c2.avi`, `c1cal.avi` e `c2cal.avi` para o diretório de trabalho no Colab.

4. **Executar o Código**:
   - Siga as instruções no notebook para definir os parâmetros de calibração, realizar a extração de coordenadas 2D e reconstruir a trajetória 3D.

5. **Visualizar os Resultados**:
   - O script gera gráficos da trajetória reconstruída e exibe as velocidades calculadas.

6. **Salvar Resultados**:
   - Os resultados, incluindo os dados da trajetória e velocidades, podem ser exportados para análise adicional.

## Dependências

- **Python 3.x**
- **Bibliotecas**:
  - `numpy`
  - `pandas`
  - `opencv-python`
  - `matplotlib`
  - `scipy`
  - `mpl_toolkits`

## Créditos

Projeto realizado com base em referências de código fornecidas pelo professor e por colegas. Adaptado para execução no Google Colab.

---

