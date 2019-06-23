### 1. Problema a ser resolvido
Classificação de gênero musical: 
1. Utilizando Dados extraídos dos espectogramas das musicas
2. Utilizando as próprias imagens dos espectogramas


### 2. Dataset
#### GTZAN dataset

10 Gêneros Musicais
1. Blues
2. Classical
3. Country
4. Disco
5. Hiphop
6. Jazz
7. Metal
8. Pop
9. Reggae
10. Rock


Cada gênero contém 100 musicas. Total dataset: 1000 musicas. (1.2 GB)
Para cada música foi criado uma imagem do espectograma equivalente da musica. (276.6MB)
Para a extração de dados do espectograma foram selecionados as principais                                 features de extração da biblioteca Librosa, que são:

1. Mel-frequency cepstral coefficients (20 coeficientes):
Representação de um conjunto dos espectros de potência de cada faixa de um som
2. Spectral Centroid:
Medida de processamento digital de sinais para caracterizar um espectro. Indica onde está localizado o "centro de massa" do espectro. 
3. Zero Crossing Rate:
Taxa de mudanças de sinal ao longo de um sinal, ou seja, a taxa na qual o sinal muda de positivo para zero para negativo ou de negativo a zero a positivo.
4. Chroma Frequencies:
Medida que abstrai os sinais detectados e os aproximam das classes de notas harmônicas
5. Spectral Roll-off:
Medida que utiliza uma função da frequência logarítmica com as unidades representadas como decibéis ao longo das faixas.


### 3. Trabalhos com o mesmo dataset e mesmo pré processamento
1. https://medium.com/@navdeepsingh_2336/identifying-the-genre-of-a-song-with-neural-networks-851db89c42f0 52,5% acurácia RN 25 features
2. https://gist.github.com/parulnith/7f8c174e6ac099e86f0495d3d9a4c01e 63% acurácia RN 25 features

### 4. Trabalhos com mesmo dataset e preprocessamento mais detalhado
1. https://github.com/Hguimaraes/gtzan.keras 86.4% CNN com 74 features
2. https://github.com/jsalbert/Music-Genre-Classification-with-Deep-Learning CNN + transfer learning + RNN  
