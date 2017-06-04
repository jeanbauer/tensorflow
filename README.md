# Tensorflow


## Instalando Tensorflow no Mac OS X com virtualenv

#### 1. Instale o Python (_Python 2.7.10 ou > 3_) e abra o terminal

#### 2. Instalaremos o pip (gerenciador de depêndencias do Python)

Digite `sudo easy_install pip` e depois enter

Digite `sudo pip install --upgrade virtualenv` e depois enter

#### 3. Criaremos um ambiente virtual para rodar o tensorflow

Digite `virtualenv --system-site-packages ~/tensorflow`

Ou seja, criamos o ambiente na pasta `tensorflow` que fica na root do sistema `~/`, para validar, vá até lá (`cd ~/`) e digite `ls`.

> Caso sua versão de Python seja 3, rode: `virtualenv --system-site-packages -p python3 ~/tensorflow`

#### 4. Vamos ativar o ambiente virtual que criamos
Digite `source ~/tensorflow/bin/activate`

Se apareceu um símbolo ` (tensorflow)$ ` no seu terminal, então tudo funcionou até agora.

Caso queira derrubar esse ambiente, basta digitar `deactivate 
` na sessão.

#### 5. Upgrade/Download do Tensorflow
Digite `pip install --upgrade tensorflow`

Pronto! Estamos prontos para testar.

## Testando o algoritmo

Com o terminal aberto, certfique-se de ter o tensorflow rodando:
Digite `source ~/tensorflow/bin/activate`

Depois, na raíz deste projeto, digite:

```
cd image/imagenet
python classify_image.py
```

O resultado deverá ser algo como: 

```
giant panda, panda, panda bear, coon bear, Ailuropoda melanoleuca (score = 0.89107)
indri, indris, Indri indri, Indri brevicaudatus (score = 0.00779)
lesser panda, red panda, panda, bear cat, cat bear, Ailurus fulgens (score = 0.00296)
custard apple (score = 0.00147)
earthstar (score = 0.00117)
```

Agora teste utilizando nosso arquivo de imagem:

`python classify_image.py --image_file rose1.jpg`

Resultando em:

```
bee (score = 0.13641)
hummingbird (score = 0.13188)
ant, emmet, pismire (score = 0.10686)
picket fence, paling (score = 0.08646)
hip, rose hip, rosehip (score = 0.05405)
```
