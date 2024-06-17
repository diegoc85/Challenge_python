# Challenge_python
Solução do problema do Challenge, na linguagem Python.

- GRUPO: 
    Diego Cabral - RM: 557817
    Arnaldo Filho - RM: 
    Débora Ivanowski - RM: 

- DESCRIÇÃO DO PROBLEMA:
    A Fórmula E, por ser ainda uma categoria relativamente nova, não possui tanta popularidade nem reconhecimento global como outras categorias de corrida. Além disso, há pouca cobertura e divulgação dos eventos da categoria nos principais meios de comunicação. Embora a Fórmula E esteja fazendo progressos significativos e tenha um futuro promissor, ainda há um caminho longo a se percorrer para torná-la mais atrativa ao público e com maior prestígio dentro do automobilismo. Para isso, é necessário deixá-la mais interativa para aquele que acessa suas plataformas digitais.

- SOLUÇÃO DO PROBLEMA:
    A solução visa, por meio da criação de jogos interativos como quizzes, tornar a experiência do espectador que acessa o site ou app mais divertida e atrativa. A ideia é criar uma conexão maior entre o espectador e a Fórmula E oferecendo jogos informativos e que possibilitam, por exemplo, a personalização do som dos carros elétricos com motores à combustão. Esta, aliás, é uma das maiores reclamações daqueles que não gostam da Fórmula E, isto é, a ausência do ronco dos motores e também a falta de interatividade em suas plataformas. Atualmente não há uma solução desse tipo no site e aplicativo móvel.  
    Por meio de jogos interativos, será possível trazer mais dados e estatísticas relevantes da categoria como a velocidade atual do piloto, bem como a sua distância para o piloto a sua frente e sua posição atual. Essas informações não são exibidas aos espectadores que acessam o site e o aplicativo. Os jogos, além de divertirem, poderão exibir informações em tempo real da corrida para aqueles que jogam. 
    Os jogos ajudarão a quebrar os preconceitos que o grande público tem em relação à corrida elétrica, como a ausência de barulho. A ideia é utilizar o jogo como uma isca para que novos usuários possam se interessar pela Fórmula E. Poderá ser apresentado ao espectador outras formas de barulho e diferenciais que só existem nessa categoria. Um exemplo é o modo de ataque que é a possibilidade de ganhar potência extra durante um período ao passar por uma zona de ativação.  
    Esse jogo será oferecido dentro de uma área exclusiva do site e do aplicativo móvel, e será um benefício cobrado por meio de uma assinatura mensal. 

- INSTRUÇÕES DE USO DO PROGRAMA:
    No código em Python, simulamos como será implementado no site a nossa solução, que é a criação de um jogo estilo quiz, em que o usuário terá seus conhecimentos testados e também receberá informações relevantes sobre a Fórmula E. Além disso, terá acesso em tempo real de dados de telemetria dos carros como a velocidade atual de um determinado piloto, sua distância em relação ao piloto a sua frente e sua classificação atual na corrida. No jogo, será possível também personalizar o som dos motores dos carros elétricos com sons de motores à combustão de carros da Fórmula 1 e de outras categorias. Por enquanto, só será possível desligar e ligar o som dos carros, mas, posteriormente, será implementada as opções de sons de carros. Foi utilizado o Jupyter Notebook para a criação do código. 

    Primeiramente, ao executar o programa, será necessário fazer um prévio cadastro para acessar a área exclusiva do site, pois o jogo não será oferecido a todos. Após o cadastro, o assinante fará login com seu e-mail e senha cadastrados e, se os dados estiverem corretos, será liberado seu acesso à área exclusiva. Depois que entrar, será mostrado um menu com 4 opções: 1) Verificar a velocidade do piloto na lista exibida com os pilotos da atual temporada; 2) Ligar e desligar o som do carro; 3) Informar a posição e a distância do piloto na lista exibida, e 4) Sair do programa. Ao escolher uma das opções será exibida a informação de acordo com a opção desejada. A velocidade, a posição e a distância do piloto escolhido são números escolhidos de forma aleatória usando a biblioteca random. O menu aparecerá até o usuário digitar a opção 4 para sair do progrma, ou seja, o usuário poderá escolhes as opções quando vezes quiser. 

    No código, há uso de funções (def), estruturas de repetição (for e while), estrutura condicional (if, else, elif), além de listas (pilotos), e do uso de dicionários (usuarios), o qual facilita a verificação dos dados cadastros ao se fazer login. 




