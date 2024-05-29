# Exercício Esquadro 2 (Lógica de Programação)

Na primeira aula vimos como desenhar linhas para, por exemplo, criar um esquadro. Entendemos que é preciso chamar a função beginPath e definir cada ponto do triângulo. Isso dá bastante trabalho e para quem não conhece tão bem a API até pode ser complicado!

Repare que é muito mais fácil criar um retângulo, basta chamar fillRect. Que tal criar uma função desenhaTriangulo que recebe as coordenadas dos 3 pontos? Seria muito mais fácil, não?

Aliás, podemos ir além, pois um esquadro é mais simples ainda! Para deixar mais claro, vamos analisar a imagem abaixo:

![image](https://github.com/paulateshima/exercicio.esquadro2/assets/170154538/84a3a204-0d4f-4f98-a9b5-f3cd9d7378a6)

Nesse tipo de triângulo, basta saber os pontos A e C para descobrir o B! Repare que o X do A também é o X do B, e o Y do C também é o Y do B. Ficou confuso? Veja essa outra imagem:

![image](https://github.com/paulateshima/exercicio.esquadro2/assets/170154538/c7aa06b2-a463-4487-96d5-98d4413ec568)

Sabendo disso, podemos criar uma função mais simples ainda, que recebe as coordenadas do ponto A e C (além da cor) para desenhar um esquadro!

A função desenhaEsquadro com os parâmetros fica similar a essa:

```
function desenhaEsquadro(xa, ya, xc, yc, cor) {
    //a implementacao fica com você :)
}
```

Agora é com você! Faça melhorias no código abaixo e crie a função desenhaEsquadro completa. Não esqueça que a cor do esquadro deve ser preta.

```
<canvas width="600" height="400"></canvas>

<script>

    var tela = document.querySelector('canvas');
    var pincel = tela.getContext('2d');

    pincel.fillStyle="black";
    pincel.beginPath();
    pincel.moveTo(50, 50);
    pincel.lineTo(50, 400);
    pincel.lineTo(400, 400);
    pincel.fill();

    pincel.fillStyle="white";
    pincel.beginPath();
    pincel.moveTo(100, 175);
    pincel.lineTo(100, 350);
    pincel.lineTo(275, 350);
    pincel.fill();

</script>
```

O código completo é?
