- Introdução

Primeira atividade da disciplina 'Introdução a Computação Gráfica' ministrada na UFPB em 2019.
A atividade consiste na projeção de 1 ponto(pixel), 1 linha e 1 triângulo não preenchido, com o bônus de 1 triângulo preenchido.
Para tal foi utilizado o Glut/GLutfree setup disponível em: https://www.opengl.org/resources/libraries/glut/

- Ponto

![ponto](https://user-images.githubusercontent.com/30871470/61192895-20f4ed00-a68e-11e9-88b8-7398ade67530.JPG)

Para mostrar o ponto na tela foi necessário criar uma função que recebe como parâmetros: a posição em x, em y e a cor do pixel. Utilizando a equação: Offset = x*4 + y*w*4 . Sendo W a largura da tela, pre-definida no arquivo que inicia a tela do OpenGl.

Arquivo exibindo o resultado: (ponto.JPG)

- Linha

![linha](https://user-images.githubusercontent.com/30871470/61192920-336f2680-a68e-11e9-89db-0e21910ac264.JPG)

A função para desenhar uma linha foi criada utilizando e chamando a função anterior para desenhar um ponto. Como parâmetros recebe a posição em (x,y) do ponto inicial e sua cor, assim como a posição em (x,y) do ponto final e respectivamente a sua cor. Trançando uma linha do ponto inicial até o ponto final contando também com o algorítimo de mistura de ambas as cores dos polos.

Base para implementação:  http://electrofriends.com/source-codes/software-programs/c/graphics/c-program-to-for-midpoint-line-algorithm/

Arquivo exibindo o resultado: (linha.JPG)

- Triângulo

![triângulo](https://user-images.githubusercontent.com/30871470/61192933-408c1580-a68e-11e9-88f9-504c7b68a556.JPG)

Para exibir o triângulo foi necessário chamar a função de desenhar linha citada anteriormente, conectando os 3 pontos (x,y) passados nos parâmetros da função, colorindo as astes também com as 3 cores recebidas como parâmetro na função.

Base para implementação: https://www.scratchapixel.com/lessons/3d-basic-rendering/rasterization-practical-implementation/rasterization-stage

Arquivo exibindo o resultado: (triângulo.JPG)

- Triângulo Preenchido

![triângulopreenchido](https://user-images.githubusercontent.com/30871470/61192947-50a3f500-a68e-11e9-8cba-977f578b78a9.JPG)

Na mesma função citada anteriormente foi adicionado um boleano e uma 4ª cor, referentes ao preenchimento do triângulo e a cor do preenchimento, caso fosse verdadeiro o triângulo seria preenchido e caso falso, o triângulo permaneceria apenas com suas astes sem preenchimento.

Base para implementação: https://www.scratchapixel.com/lessons/3d-basic-rendering/rasterization-practical-implementation/rasterization-stage

Arquivo exibindo o resultado: (triângulopreenchido.JPG)
