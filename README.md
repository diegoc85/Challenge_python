# Challenge_python
 CHALLENGE (FIAP) 

Solução na linguagem Python do problema trazido pela TECH MAHINDRA da FÓRMULA E 

- GRUPO: 

    DIEGO CABRAL - RM: 557817

    ARNALDO FILHO - RM: 555780

    DÉBORA IVANOWSKI - RM:555694 

- DESCRIÇÃO DO PROBLEMA:
    A Fórmula E, por ser ainda uma categoria relativamente nova, não possui tanta popularidade nem reconhecimento global como outras categorias de corrida. Além disso, há pouca cobertura e divulgação dos eventos da categoria nos principais meios de comunicação. Embora a Fórmula E esteja fazendo progressos significativos e tenha um futuro promissor, ainda há um caminho longo a se percorrer para torná-la mais atrativa ao público e com maior prestígio dentro do automobilismo. Para isso, é necessário achar soluções que possam deixá-la mais interativa para seu espectador.

- SOLUÇÃO DO PROBLEMA:
    A solução visa, por meio da Visão Computacional (programa VISION FE), tornar a experiência do espectador que assiste à corrida presencialmente mais divertida e interativa. A ideia é criar uma conexão maior entre o espectador e a Fórmula E fornecendo informações relevantes que o ajudem a acompanhar e a se interar melhor daquilo que está acontecendo no circuito. Dessa forma, o usuário não se sentirá perdido ou alheio aos acontecimentos importantes como a troca de posições entre os carros. Esse código tem como objetivo simular o uso da Visão Computacional, por meio da câmera de um celular ou de um óculos de realidade aumentada, para rastrear e detectar os carros na pista. Assim, o espectador terá acesso a informações em tempo real, como a velocidade dos carros, volta mais rápida, a posição do piloto rastreado na corrida, além do seu nome e da sua respectiva equipe. 

    A Visão Computacional é um ramo da inteligência artifial que possibilita aos computadores a interpretarem e compreenderem o mundo visual da mesma forma que os humanos. Ela envolve a captura, o processamento e a análise de imagens e vídeos para extrair informações considerada significativas. Nesse caso em específico do código, há a captura de imagem por meio de um vídeo, mas também pode ser por uma imagem ou por uma câmera durante a corrida, por exemplo. Após a captura, a imagem é transformada em dados digitais que o computador poderá processar. Durante o processo, é extraído características como bordas, formas, cores, textura ou padrões encontrados na imagem. A partir dessas características, o sistema poderá realizar tarefas como:

    -> Reconhecimento de objetos: identificar e classificar objetos, como por exemplo, ('Essa imagem contém um carro de automobilismo')

    -> Detecção de padrões: encontrar padrões como letras e gestos 

    -> Análise de movimento: Em vídeos, poderá compreender o movimento dos objetos como os carros na Fórmula E. 

    São usadas também técnicas de aprendizado de máquina. Algoritmos de aprendizado profundo (redes neurais) são frequentemente utilizados para melhorar o reconhecimento de padrões e aumentar a precisão, sendo treinados com grandes volumes de dados visuais. Além de identificar o objeto, o algoritmo fornece a localização (normalmente por meio de caixas delimitadores ou bounding boxes) para mostrar onde o objeto está na imagem. No código é usado essas caixa delimitadores para mostrar onde os carros estão. 

    - Modelos que normalmente são usados para a detecção de objetos:

        - YOLO (You Only Look Once): é um modelo de detecção em tempo real que divide a imagem em uma grade e faz a predição simultânea de múltiplos objetos e suas posições.

       -  SSD (Single Shot Detector): Detecta objetos em uma única etapa, o que permite detecção em tempo real com boa precisão. Esse é o modulo que está sendo usado no código desenvolvido para reconhecer os carros do vídeo. 

        - R-CNN (Regions with Convolutional Neural Networks): Utiliza uma abordagem em duas etapas, primeiro identificando regiões de interesse e, em seguida, classificando o que está dentro dessas regiões.
    
    Primeiramente, o objeto é detectado no vídeo usando o modelo de detecção, que nesse caso é o OPEN CV, uma biblioteca de visão computacional de código aberto que permite aos desenvolvedores criar aplicações de visão artificial e inteligência artifical. Depois de detectado, o objeto é rastreado ao longo de vários quadros do vídeo. O rastreamento pode ser interrompido e uma nova detecção pode ser realizada caso o objeto saia da área de visão ou o sistema perca o objeto. À medida que o objeto se move, a posição é atualizada constantemente pelo rastreador, o que permite saber exatamente onde o objeto está em cada momento. 


     

- INSTRUÇÕES DE USO DO PROGRAMA:

    No código em Python, simulamos como será implementada a nossa solução usando a Visão Computacional. Para isso, foi utilizado um vídeo com carros se movimentando em uma rodovia onde o algoritmo é auxliado pela rede neural treinada (SSD), trabalhando de forma conjunta com a biblioteca OPEN CV reconhecendo detectando e fazendo o rastreio dos carros que aparecem no vídeo. Para essa demonstração, foi criado um sistema simples de cadastro (nome, e-mail e senha) e de login (e-mail e senha) para que o usuário possa acessar a área exclusiva do VISION FE. Sendo assim, não será possível acessar a solução sem fazer previamente um cadastro e logo após o login. No código, após o login efetuado com sucesso (só terá 3 tentativas), o usuário poderá escolher dentre as 5 opções que aparecerão no menu:

    1) Carregar o VISION FE, 
    2) Mostrar a velocidade atual do carro rastreado (é fornecida de forma aleatória, por meio da biblioteca random - de 0 320), 
    3) Posição atual do carro do piloto rastreado (obtida de forma aleatória pela biblioteca random - 1 a 22), 
    4) Nome do piloto e da sua respectiva equipe (obtida por meio de um arquivo CSV que foi transformado em um DataFrame utilizando a biblioteca pandas) ou 
    5) Sair do programa. 

    Como o código é apenas um protótipo para demonstrar o funcionamento do VISION FE, o usuário poderá escolher a opção que desejar para obter as informações geradas pelo VISION FE. No entanto, na prática, assim que o VISION FE for ativado, o espectador receberá todas essas informações mencionadas acima, em tempo real, de uma só vez na tela do seu dispositivo. Dessa forma, não será necessário escolher opções como no menu do código. 

    - Foi utilizado o Jupyter Notebook para a criação do código.
    - Caso as bibliotecas abaixo não estejam instaladas, será necessário instalar e depois importá-las. 
        -> Para instalar, usar o comando 'pip install'. Ex.: 'pip install cvzone
        -> Para importar, usar o comando 'import'. Ex.: 'import cvzone 
        Seguir esses comandos para todas as bibliotecas que não estiverm instaladas. 
    - Bibliotecas utilizadas no projeto:

        - pandas as pd ( oferece estruturas e operações para manipular tabelas numéricas e séries temporais.)
        - getpass (apresenta ao usuário um prompt solicitando a senha e não mostra os caracteres digitados na tela)
        - random (geração de números aleatórios)
        - cv2 (OPEN CV - biblioteca de Visão Computacional para reconhecimento de objetos)
        - numpy as np (realização de cálculos numéricos e matemáticos em larga escala, por meio da funcionalidade chamada vetorização)
        - cvzone (funciona como uma camada de abstração sobre as bibliotecas como OPEN CV, tornando mais acessíveis algumas tarefas mais comuns e complexas na área de visão computacional)

    No código, há uso de funções (def), função dentro de função, função chamando outra função, estruturas de repetição (for e while), estrutura condicional (if, else, elif), DataFrame (pilotos), listas com dicionários (usuários), uso de dicionários, o qual facilita a verificação dos dados de e-mail e senha cadastrados ao se fazer login. 
    Para executar esse código, é necessário clonar este repositório utilizando alguma IDE como VS CODE. Depois é só rodar o código e seguir as instruções do programa. 

    Nos arquivos do repositório também estão os relatórios gerados com as saídas da execução do código, bem como um diagrama em blocos do funcionamento do código.
    Também nos arquivos estão os dois arquivos (ssd_mobilenet_v3 e frozen_inference_graph) necessários para rodar o modelo neural. Esse modelo utilizado foi treinado na base de dados coco.names (lista com mais de 80 tipos de objetos que o modelo consegue identificar), que é um dos arquivos do projeto. 

    Caso ao executar o código apareça a mensagem de que o excesso de linhas no VS CODE foi extrapolado, será preciso configurar a quantidade de linhas na saída e aumentar esse número consideravelmente. Deve-se ir em configurações (CTRL + SHIFT + P) e digitar preferences: Open User Settings. Buscar pela opção Output: Text line limit, e escrever um valor, como por exemplo 1000 ou até mais, se for preciso. Pronto, o limite de linhas na saída do código foi alterado e você não deverá ter problemas na execução do código. 

    Divirta-se com o VISION FE e nao se esqueça de nos dar seu feedback! 




