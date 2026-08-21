# Estudo de Iluminação — Galpão 3D

Este documento apresenta configurações de iluminação aplicadas a uma cena de galpão 3D. O objetivo é observar como o tipo, a posição, a cor, a intensidade, o alcance e as sombras das fontes de luz alteram a aparência do ambiente.

## Índice

- [Directional Light](#directional-light)
  - [Modo 1](#modo-1)
  - [Modo 2](#modo-2)
- [Point Light](#point-light)
  - [Configuração 1 — Azul](#configuração-1--azul)
  - [Configuração 2 — Vermelha](#configuração-2--vermelha)
- [Spot Light](#spot-light)
  - [Configuração 1 — Amarela](#configuração-1--amarela)
  - [Configuração 2 — Branca](#configuração-2--branca)
- [Conclusão](#conclusão)

---

## Directional Light

A `Directional Light` foi utilizada para simular a iluminação do Sol. Esse tipo de fonte emite luz em uma direção específica; portanto, sua rotação controla a direção em que a luz incide sobre a cena.

### Modo 1

Nesta primeira configuração, a luz teve intensidade `2` e temperatura de `5000 K`, produzindo uma iluminação branca e relativamente forte. Foram utilizadas sombras suaves (`Soft Shadows`), com intensidade de sombra `1`.

O resultado foi uma iluminação geral do ambiente, com áreas mais claras e sombras projetadas pelos objetos. Como a estrutura possui partes fechadas, algumas regiões internas permaneceram mais escuras, demonstrando a influência direta da direção da luz nas áreas iluminadas.

| Parâmetro | Valor |
| --- | --- |
| Tipo de luz | Directional Light |
| Intensidade | 2 |
| Temperatura | 5000 K |
| Sombras | Soft Shadows |
| Intensidade da sombra | 1 |

<img width="1361" height="821" alt="image" src="https://github.com/user-attachments/assets/47d3781e-417a-4ef8-8db1-ac9a3e8ab3bd" />

### Modo 2

Na segunda configuração, a intensidade foi aumentada de `2` para `4`, deixando a cena consideravelmente mais iluminada. A temperatura foi reduzida de `5000 K` para `3422 K`, resultando em uma luz mais quente, com aparência amarelada.

As sombras também foram alteradas de `Soft Shadows` para `Hard Shadows`, tornando-as mais marcadas e definidas. A rotação da luz foi modificada, mudando a direção em que a iluminação incide sobre o galpão. Como resultado, uma parte maior da estrutura ficou diretamente iluminada, enquanto outras regiões continuaram mais escuras.

| Parâmetro | Modo 1 | Modo 2 |
| --- | --- | --- |
| Intensidade | 2 | 4 |
| Temperatura | 5000 K | 3422 K |
| Sombras | Soft Shadows | Hard Shadows |
| Direção | Configuração inicial | Rotação alterada |

<img width="1364" height="824" alt="image" src="https://github.com/user-attachments/assets/fb3fac14-7dde-435e-80d5-d69a0bde23e1" />

---

## Point Light

A `Point Light` emite luz em todas as direções a partir de um único ponto. Ela é adequada para representar lâmpadas, focos de iluminação e outras fontes localizadas dentro do ambiente.

### Configuração 1 — Azul

Nesta configuração, a Point Light foi posicionada no lado direito da estrutura e configurada com a cor azul. A intensidade foi definida como `50` e o alcance como `10`.

O resultado é uma iluminação azul evidente no lado direito do galpão. As superfícies próximas à fonte recebem uma tonalidade azulada, enquanto as regiões mais distantes sofrem menos influência. Também é possível observar sombras nas partes da estrutura posicionadas entre a fonte de luz e outras superfícies, criando contraste entre áreas iluminadas e áreas escuras.

| Parâmetro | Valor |
| --- | --- |
| Tipo de luz | Point Light |
| Posição | Lado direito do galpão |
| Cor | Azul |
| Intensidade | 50 |
| Alcance | 10 |

<img width="1512" height="856" alt="image" src="https://github.com/user-attachments/assets/0fe42681-ba64-4e92-8750-6273f73ac827" />

### Configuração 2 — Vermelha

Nesta segunda configuração, a Point Light foi posicionada no lado esquerdo do galpão e configurada com a cor vermelha. A intensidade foi definida como `10`, enquanto o alcance permaneceu em `10`.

Em comparação com a configuração azul, a intensidade menor faz com que a luz vermelha fique mais concentrada e menos intensa sobre a estrutura. O lado esquerdo do galpão recebe uma tonalidade avermelhada, principalmente nas superfícies próximas à fonte, enquanto as regiões mais afastadas continuam recebendo pouca influência da luz.

A cor vermelha cria uma aparência mais quente e chamativa, em contraste com o aspecto frio produzido pela iluminação azul. As sombras permanecem presentes e mostram como os objetos bloqueiam parcialmente a passagem da luz.

| Parâmetro | Point Light azul | Point Light vermelha |
| --- | --- | --- |
| Posição | Lado direito | Lado esquerdo |
| Cor | Azul | Vermelha |
| Intensidade | 50 | 10 |
| Alcance | 10 | 10 |
| Aparência | Fria e intensa | Quente e mais concentrada |

<img width="1600" height="864" alt="image" src="https://github.com/user-attachments/assets/e246d69d-43f2-43e3-a257-b0d3d4548262" />

---

## Spot Light

A `Spot Light` concentra a iluminação em uma direção e área específicas, sendo útil para destacar pontos da cena, como uma parede ou um objeto.

### Configuração 1 — Amarela

Nesta configuração, a Spot Light foi direcionada para uma área específica da parede. A luz possui tonalidade amarelada, intensidade `80` e alcance `10`, criando um foco forte, quente e bastante destacado sobre a superfície iluminada. As sombras utilizadas são do tipo `Hard Shadows`.

| Parâmetro | Valor |
| --- | --- |
| Tipo de luz | Spot Light |
| Cor | Amarela |
| Intensidade | 80 |
| Alcance | 10 |
| Sombras | Hard Shadows |

<img width="1512" height="928" alt="image" src="https://github.com/user-attachments/assets/6bf012d2-48c2-451a-826f-c5cfdc428ca4" />

### Configuração 2 — Branca

Nesta configuração, foi utilizada uma Spot Light branca direcionada para uma área específica da parede. O foco de luz permanece facilmente identificável, preservando a principal característica desse tipo de iluminação: a concentração em um ponto determinado.

Em relação à configuração anterior com luz amarelada, a iluminação branca oferece um resultado mais neutro e natural. A ausência da tonalidade quente permite que as cores originais dos objetos sejam preservadas de forma mais próxima, enquanto a área iluminada mantém contraste com as regiões ao redor, que permanecem mais escuras.

| Aspecto | Spot Light amarela | Spot Light branca |
| --- | --- | --- |
| Cor percebida | Quente e chamativa | Neutra e natural |
| Efeito sobre os objetos | Altera as cores com tonalidade amarelada | Preserva melhor as cores originais |
| Foco de iluminação | Forte e destacado | Direcionado e contrastante |

> A captura da configuração amarela permite identificar intensidade `80`, alcance `10` e `Hard Shadows`. Os valores numéricos da Spot Light branca não foram informados.

<img width="1513" height="924" alt="image" src="https://github.com/user-attachments/assets/db07c471-862b-4a75-b390-ed9c39d6e583" />

---

## Conclusão

As configurações demonstram que a iluminação altera significativamente a aparência de um mesmo cenário. A `Directional Light` cria iluminação geral e permite controlar a direção, a temperatura e a definição das sombras. Já a `Point Light` produz iluminação localizada em todas as direções, com diferenças evidentes conforme a posição, a cor, a intensidade e o alcance. Por fim, a `Spot Light` concentra a luz em áreas específicas, permitindo destacar superfícies e criar diferentes atmosferas por meio da cor.

Ao ajustar esses parâmetros, é possível criar cenas com aparência fria ou quente, maior ou menor contraste, sombras mais suaves ou definidas e destaque para regiões específicas do ambiente.
