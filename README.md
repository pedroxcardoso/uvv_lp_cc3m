# <img align="center" alt="Python" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg"> PSET-1 

> Aluno: Pedro Cardoso da Silva Neto      
> Turma: CC3M      
> Professor: Abrantes Araújo Silva Filho     
> Tema: MIT 6.009

# QUESTÕES

## Questão 01
> Se você passar essa imagem pelo filtro de inversão, qual seria o
> output esperado? Justifique sua resposta.


Resposta: <br>
O resultado será [226, 166, 119, 55], pois após passarem por esta função:
![image](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/d530cbe3-b3a9-421f-9e16-f6a23d3f2329) <br>
Cada um dos 4 números ira se subtrair de 255.

## Questão 02
> Faça a depuração e, quando terminar, seu código deve conseguir
> passar em todos os testes do grupo de teste TestInvertida 
> (incluindo especificamente o que você acabou de criar). 
> Execute seu filtro de inversão na imagem
> test_images/bluegill.png, salve o resultado como uma imagem PNG e
> salve a imagem em seu repositório GitHub.


Resposta: <br>
![image](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/c82418ee-dd6a-4e95-a707-7158fafc0adc) <br>
Resultado: <br>
![bluegill_invertida](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/aa2679bf-cb5c-4e8f-9217-45787b722f08)


## Questão 03
> Considere uma etapa de correlacionar uma imagem com o seguinte
> kernel:
>
> 0.00 -0.07 0.00 <br>
> -0.45 1.20 -0.25 <br>
> 0.00 -0.12 0.00 <br>
>
> Qual será o valor do pixel na imagem de saída no local indicado pelo destaque
> vermelho? Observe que neste ponto ainda não arredondamos ou recortamos o valor, informe exatamente como você calculou. Observação: demonstre passo a passo
> os cálculos realizados.

~~~
Resposta: O resultado será 32,76.
~~~
Ao multiplicarmos cada um dos "quadrados" por seus kernels, chegaremos no seguinte cálculo: <br>
(80 * 0) + (53 * - 0,07) + (99 * 0) + <br>
(129 * - 0,45) + (127 * 1,20) + (148 * -0,25) + <br>
(175 * 0) + (174 * - 0,12) + (193 * 0) <br>
= 32,76.

## Questão 04
> Quando você tiver implementado seu código, tente executá-lo em
> test_images/pigbird.png com o seguinte kernel 9 × 9:

Resposta: <br>
![image](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/19898256-68ad-4e08-a5a6-44408b65a0d6) <br>
Resultado: <br>
![pigbird2](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/98e8758a-e8f0-4699-bdff-b814fe6a70d2)


## Questão 05
> se quisermos usar uma versão desfocada B que foi feita com um
> kernel de desfoque de caixa de 3 × 3, que kernel k poderíamos usar para calcular
> toda a imagem nítida com uma única correlação? Justifique sua resposta mostrando
> os cálculos.

Resposta: <br>
![image](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/b29aac24-07b3-4921-adec-7fd5479d3a53)
Resultado: <br>
![python_focada](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/b98a8f84-4e95-4450-8b40-b62248b23d80)

## Questão 06
> Explique o que cada um dos kernels acima, por si só, está fazendo.
> Tente executar mostrar nos resultados dessas correlações intermediárias para ter
> uma noção do que está acontecendo aqui.

Resposta: <br>
Código: <br>
![image](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/dae8e651-8032-49aa-8f57-2c4e5ae474c0) <br>

Imagem Kx: <br>
![construct_Kx](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/16da8d87-6eae-4fff-bc27-360623073a42) <br>

Imagem Ky: <br>
![construct_Ky](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/8d255ded-1752-487b-ae40-efce6f2804a4) <br>

Imagem com ambos aplicados: <br>
![construct_Final](https://github.com/pedroxcardoso/uvv_lp_cc3m/assets/103221067/8f4d1d8c-b68a-4c0a-8f57-686286b18ceb) <br>


