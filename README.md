# CaptchaML

Esse conjunto de ferramentas foi criado com o objetivo de decifrar 6 caracteres de um Captcha. Os 6 caracteres podem variar de 0 a 9 e todas as letras do alfabeto.
Através da cração de uma Inteligência Artificial e seu enriquecimento, utilizando Machine Learning, o foi possivel obter um acerto de cerca de 88% das letras.

Ferramentas utilizadas: Jupyter notebook (python), Anaconda Prompt, SKLearn, Numpy, Tensorflow.

#  Primeiro Passo: Download dos Captchas e estruturação dos arquivos de imagem
600 Captchas (Arquvos do tipo PNG) foram baixados e foi criado um programa em python que divide cada um de seus 6 caracteres baseado em uma posição média que eles aparecem. O    programa salva cada uma das letras em um repositório, e o próximo passo é renomear os arquvos conforme o exemplo ao lado.
  
![image](https://user-images.githubusercontent.com/55901438/110069193-1224e780-7d56-11eb-91b8-327c3ef3c006.png)

598 = número do arquivo captcha / F - letra da imagem, renomeada após o programa ter separado as letras. O programa separa as letras e gera o arquivo com o número do captcha, e à mão eu inseri a letra "f" após o "_". O mesmo se repete para os outros arquivos / letras.  

![image](https://user-images.githubusercontent.com/55901438/110070675-3df59c80-7d59-11eb-9bc4-30a3f0e08932.png)


#  Segundo Passo: Separação das letras
Um outro programa em python identifica o caractere inserido no final de cada arquvo do repositório do primeiro passo e as copia para uma nova pasta identificada com o caractere.
  
![image](https://user-images.githubusercontent.com/55901438/110072869-3506ca00-7d5d-11eb-97ac-dea98412ec71.png)

#  Terceiro Passo: Treinar o modelo
Através de Machine Learning, utilizando a bibloteca sklearn, é treinado um modelo de classificação para previsão das letras contidas em cada uma das 6 posições do captcha. Os dados usados para o treinamento são os repositórios de cada caractere, especificados no segundo passo.

![image](https://user-images.githubusercontent.com/55901438/110074551-2a99ff80-7d60-11eb-987c-3cd75576f749.png)

# Quinto Passo: Identificação das letras
Com o modelo (arquvo .hdf5) treinado, um novo programa separa os 6 caracteres por posição, assim como o primeiro passo, e passa por cada um desses caracteres tentando identifica-los e classifica-los. O caractere identificado é printado no canto inferior esquerdo de cada divisão. O resultado da prevsão também é printado no prompt, conforme imagens abaixo.

![image](https://user-images.githubusercontent.com/55901438/110194349-e1f14d80-7e16-11eb-807f-733d89d81c50.png)

![image](https://user-images.githubusercontent.com/55901438/110194526-62b04980-7e17-11eb-9dff-3069386be2dc.png)
