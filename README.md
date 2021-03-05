# CaptchaML

Esse programa foi criado com o intuido de decifrar 6 caracteres de um Captcha. Os 6 caracteres podem variar de 0 a 9 e todas as letras do alfabeto.
Através da cração de uma Inteligência Artificial e seu enriquecimento, utilizando Machine Learning, o foi possivel obter um acerto de cerca de 88% das letras.

Ferramentas utilizadas: Jupyter notebook (python), Anaconda Prompt, SKLearn, Numpy, Tensorflow.

Primeiro Passo: Download dos Captchas e estruturação dos arquivos de imagem.
  600 Captchas (Arquvos do tipo PNG) foram baixados e foi criado um programa em python que dividisse cada uma de suas 6 letras baseado em uma posição média que eles aparecem. O programa salva cada uma das letras em um repositório, e o próximo passo é renomear os arquvos conforme o exemplo ao lado.
  
![image](https://user-images.githubusercontent.com/55901438/110069193-1224e780-7d56-11eb-91b8-327c3ef3c006.png)

598 = número do arquivo captcha / F - letra da imagem, renomeada após o programa ter separado as letras. O programa separa as letras e gera o arquivo com o número do captcha, e à mão eu inseri a letra "f" após o "_". O mesmo se repete para os outros arquivos / letras.  

![image](https://user-images.githubusercontent.com/55901438/110070675-3df59c80-7d59-11eb-9bc4-30a3f0e08932.png)


