# SkinCancerPrediction

## 1. Projeto

O projeto _SkinCancerPrediction_ consiste na criação de um algoritmo utilizando redes neurais para determinação do tipo de cancer de pele por meio de imagem.

## 2. Problemática

O câncer de pele é um tumor que atinge a pele e corresponde a cerca de 30% de todos os tumores malignos registrados no Brasil, ocupando o primeiro lugar de número e casos em relação aos demais cânceres. Sua causado principal é a exposição excessiva ao sol e ele pode ser classificado em duas categorias gerais: melanoma e não melanoma.

O melanoma representa somente 3% dos tumores malignos da pele, sendo este o tipo mais grave, devido à sua alta possibilidade de provocar metástase (disseminação do câncer para outros órgãos).

> Estimativa de novos casos de câncer de pele melanoma no Brasil: 6.260, sendo 2.920 homens e 3.340 mulheres (2018 - INCA).

> Número de mortes por câncer de pele melanoma no Brasil: 1.794, sendo 1.012 homens e 782 mulheres (2015 – SIM)

Já o câncer de pele não melanoma, mais comum no Brasil, apresenta uma alta chance de recuperação, desde que seja detectado e tratado precocemente.

> Estimativa de novos casos de câncer de pele não melanoma no Brasil: 165.580, sendo 85.170 homens e 80.140 mulheres (2018 - INCA).

> Número de mortes por câncer de pele não melanoma no Brasil: 1.958, sendo 1.137 homens e 821 mulheres (2015 – SIM).

Os principais sintomas do câncer de pele de acordo com o Ministério da Saúde são:
- Manchas pruriginosas (que coçam), descamativas ou que sangram.
- Sinais ou pintas que mudam de tamanho, forma ou cor.
- Feridas que não cicatrizam em 4 semanas.

Para identificar e classificar um câncer de pele, um dermatologista é requirido e por meio de exame clínico conhecido como "Dermatoscopia" que permite visualizar as diversas camadas da pele e possibilita o diagnóstico. Contudo o acesso a um dermatologista nem sempre é possível dependendo da região em que a pessoa reside por conta da falta de profissionais qualificados a disposição ou pelo sucateamento do sistema de saúde de alguns estados e municípios.

## 3. Proposta de solução

Com a intenção de auxiliar o diagnóstico precoce do câncer de pele e torna-lo mais acessível, o projeto SkinCancerPrediction tem como objetivo identificar a partir de uma imagem o tipo de tumor de pele mais provável. Os parâmetros que podem ser usados para diferenciar os tipos de tumor são:
- Assimetria;
- Bordas e contorno irregulares;
- Coloração;
- Diâmetro.

O modelo de solução desenvolvido neste projeto conta com uma rede neural capaz de realizar o aprendizado de máquina e reconhecimento de padrões para identificar e classificar uma imagem de lesão/tumor de pele baseado em 7 principais tipos, sendo dois deles tumores malignos:
- Melanoma: O tipo mais grave de câncer de pele. O melanoma ocorre quando as células produtoras dos pigmentos que dão cor à pele tornam-se cancerígenas.
-  Carcinoma basocelular: Tipo de câncer de pele que começa nas células basais.
As células basais produzem novas células da pele conforme as antigas morrem. Limitar a exposição ao sol pode ajudar a evitar que essas células se tornem cancerígenas.
Esse tipo de câncer geralmente aparece como um nódulo de cera branco ou uma mancha escamosa marrom em áreas expostas ao sol, como rosto e pescoço.

Dois tumores benignos:
- Nevo melanocítico: Distúrbio geralmente não cancerígeno das células da pele produtoras de pigmento, comumente chamado de marcas de nascença ou pintas.
- Verruga seborreica: Condição de pele benigna com aspecto de um nódulo maleável de cor castanha, preta ou marrom.
A ceratose seborreica é um dos tumores de pele benignos mais comuns em idosos. Embora existam casos de tumores individuais, a presença de vários tumores é mais comum.

E três tipos de lesões:
-  Ceratose actínica: Mancha escamosa áspera na pele causada por anos de exposição ao sol.
A ceratose actínica geralmente afeta idosos. Reduzir a exposição ao sol pode ajudar a diminuir o risco.
É mais comum no rosto, nos lábios, nas orelhas, no dorso das mãos, nos antebraços, no couro cabeludo e no pescoço. A pele escamosa e áspera aumenta lentamente e não costuma causar outros sinais ou sintomas. A lesão pode levar anos para se desenvolver e dificilmente gera um risco a saúde.
-  Lesões vasculares: As anomalias vasculares correspondem a um extenso espectro de alterações que se dividem em dois grupos principais: 1) tumores vasculares, que representam as lesões proliferativas e 2) malformações vasculares, originadas por ectasias nos vasos, sejam elas capilares, venosas ou linfáticas.
-  Dermatofibroma: lesões benignas típicas de extremidades, como braços, antebraços e pernas. Por terem coloração acastanhada, geralmente, são motivos de consulta, na qual os pacientes buscam saber se são pintas ou sinais.

## 4. Arquitetura de rede neural

Definimos a rede neural com duas camadas de convolução com ativação relu e duas camadas de MaxPooling, planificamos os dados e adicionamos uma camada Dense com ativação relu e outra camada Dense com ativação Sigmoid que será a saida da rede.

A escolha da saida em sigmoid se deve ao fato de sua saída ser sempre em porcentagem, variando de 0 a 1.

## 5. Como executar

### 1. clone o repositório na sua máquina:
```https://github.com/deeplearningunb/SkinCancerPrediction``` 

### 2. Ativar seu ambiente virtual:
```virtualenv {virtual_env_name}```

```source {virtual_env_name}/bin/activate```

### 3. Instalar os requerimentos do projeto
``` pip3 install -r requirements.txt```

A aplicação deverá estar pronta para ser inicializada.

## 4. Contribuintes

| Nome | Matrícula |
| ------ | ------ |
| Breno Beleza | 18/0098641 |
| Felipe Chermont | 16/0119570 |
| Guilherme Simões | 16/0123364 |
