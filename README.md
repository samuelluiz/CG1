- Introdução

Primeira atividade da disciplina 'Introdução a Computação Gráfica' ministrada na UFPB em 2019.
A atividade consiste na projeção de 1 ponto(pixel), 1 linha e 1 triângulo não preenchido, com o bônus de 1 triângulo preenchido.
Para tal foi utilizado o Glut/GLutfree setup disponível em: https://www.opengl.org/resources/libraries/glut/

- Ponto

Para mostrar o ponto na tela foi necessário criar uma função que recebe como parâmetros: a posição em x, em y e a cor do pixel. Utilizando a equação: Offset = x*4 + y*w*4 . Sendo W a largura da tela, pre-definida no arquivo que inicia a tela do OpenGl.

Arquivo exibindo o resultado: (ponto.JPG)

- Linha
A função para desenhar uma linha foi criada utilizando e chamando a função anterior para desenhar um ponto. Como parâmetros recebe a posição em (x,y) do ponto inicial e sua cor, assim como a posição em (x,y) do ponto final e respectivamente a sua cor. Trançando uma linha do ponto inicial até o ponto final misturando ambas as cores.

Código base para implementação:  http://electrofriends.com/source-codes/software-programs/c/graphics/c-program-to-for-midpoint-line-algorithm/
Arquivo exibindo o resultado: (linha.JPG)

- Triângulo


Código base para implementação: https://www.scratchapixel.com/lessons/3d-basic-rendering/rasterization-practical-implementation/rasterization-stage
Arquivo exibindo o resultado: (triângulo.JPG)

- Triângulo Preenchido



Código base para implementação: https://www.scratchapixel.com/lessons/3d-basic-rendering/rasterization-practical-implementation/rasterization-stage
Arquivo exibindo o resultado: (triângulopreenchido.JPG)
