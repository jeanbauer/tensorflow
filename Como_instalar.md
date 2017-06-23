# Tensorflow


## Instalando Tensorflow no Mac OS X com virtualenv

#### 1. Instale o Python (_Python 2.7.10 ou > 3_) e abra o terminal
> Não testamos com Python v3.

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
