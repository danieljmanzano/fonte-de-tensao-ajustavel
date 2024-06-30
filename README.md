# Fonte de tensão ajustável

*trabalho da disciplina Eletronica para Computação - SSC0180*

# Sobre o projeto
Nesse trabalho, tivemos a tarefa de criar uma fonte que, recebendo tensão de uma tomada com corrente alternada, tenha capacidade de ajustar a ddp para uma faixa de 3V a 12V e tornar a corrente contínua, que possa atingir o valor de 100mA. Assim, usamos simuladores como o Falstad e o Eagle para elaborar a ideia e, posteriormente, construímos a fonte, cujos detalhes podem ser vistos no decorrer dessa página.

# Tabela dos componentes
| componente | quantidade | custo unitário |
| :----: | :----: | :----: |
|diodo zener|1|R$0,50|
|capacitor 470uF|1|R$4,40|
|diodo|4|R$0,20|
|potenciometro|1|R$7,00|
|resistor 100 (5W)|1|R$1,90|
|resistor 2k2|1|R$0,07|
|resistor 3k|1|R$0,07|
|resistor 5k|1|R$0,07|
|transistor|1|R$0,80|
|protoboard|1|R$21,70|
| | **`TOTAL:`** | **`R$37,31`** |

# Sobre os componentes
- **transformador**: tem o papel de diminuir a voltagem que o circuito recebe da fonte corrente alternada (tomada). a partir da voltagem de 127V recebida, o transformador consegue diminuí-la para a faixa de tensão desejada (3V a 12V).
- **ponte de diodo**: também chamada de ponte retificadora, é uma junção de 4 diodos que têm a capacidade de transformar a tensão alternada (vinda da tomada) em contínua, ou seja, tem capacidade de a "retificar".
- **capacitor**: armazena carga no circuito nos ciclos da corrente alternada, liberando corrente quando a tensão da fonte é menor do que a tensão interna. ele descarrega sua carga armazenada quando há a inversão do ciclo no circuito. com base em cálculos de um ripple de 10%, chegamos próximos do valor comercial de 470uF de capacitância, usando um capacitor com esse valor no projeto.
- **diodo zener**: tem o intuito de regular a corrente máxima, sendo o usado especificamente de voltagem máxima de 13V. quando a ddp passa de 13V, ele mantém o valor máximo de 13 em seus terminais; quando a ddp chega menor do que 13V, ele não conduz e consequentemente não interfere no circuito.
- **potenciômetro**: é um resistor variável usado como controle da tensão resultante, que permite atingir as ddps de 3V a 12V no circuito.
- **transistor**: amplifica a corrente que recebe em sua base para um valor desejado, sendo o máximo de 100mA.
- **resistores**: usados em mais de um momento no circuito, têm a função de limitar a corrente, garantindo certa "segurança" aos componentes. no circuito, usamos eles associados ao led, ao zener, ao potenciômetro e ao transistor, com resistências variadas de 100, 120, 2.2k e 3k de ohms.
- **led**: tem função de indicar o nível da corrente atingida na parte final do circuito, brilhando mais quando a voltagem e a corrente são maiores. de modo geral, não interfere nos valores obtidos no circuito, servindo unicamente como indicação da voltagem e corrente ajustáveis.

# Imagem do circuito no Falstad
![Captura de tela 2024-06-11 105750](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/e3c710aa-9977-4a19-93ae-4c3c98ba290d)
   - link para o falstad: https://tinyurl.com/2cbdos5r
   - *observação sobre o projeto final: apesar de no falstad e no eagle o resistor abaixo do potenciômetro possuir 5k ohms (que, em teoria, seria o melhor valor para "acertar" o restante do ciruito), o valor final escolhido foi de 3k para garantir que atingiríamos a voltagem esperada e criar uma certa margem de erro, uma vez que as plataformas não foram completamente condizentes com a realidade.*

# PCB no Eagle
![Captura de tela 2024-06-12 210140](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/a610be01-ebc5-4f92-b6d7-2eceea460e35)

# Esquemático no Eagle
![Captura de tela 2024-06-12 204952](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/86f89c07-bab1-40e5-bc8c-1dc4eaa14497)

# Vídeo do funcionamento e fotos da fonte
- Vídeo explicando o funcionamento da fonte: https://youtu.be/jX9TOlvzc-o

https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/7742d7ce-853e-4775-993b-c37a913293de

![fotoprotoboard](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/9b20688d-45e9-45c6-a025-179d9b8a1738)
![Imagem do WhatsApp de 2024-06-27 à(s) 20 25 01_90fc1dde](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/ab38b9e3-b5f2-4b77-a094-3af1bb4c167e)
![Imagem do WhatsApp de 2024-06-27 à(s) 20 25 00_5c0ad89b](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/931ddbbe-1e25-41eb-b518-417e3e881047)

# Contas para valores de certos componentes

![Calculo do capacitor](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/blob/main/Screenshot_20240629_023409_Samsung%20Notes.jpg)
![Calculo do resistor logo a cima do diodo zener](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/blob/main/Screenshot_20240629_020520_Samsung%20Notes.jpg)
![Calculo do resistor a cima do transistor](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/blob/main/Screenshot_20240629_020854_Samsung%20Notes.jpg)






# Integrantes
- Daniel Jorge Manzano - 154468661
- Matheus Muzza Pires Ferreira - 15479468
- Rodrigo Silva de Almeida - 15645380
- Vinicius Morotti - 15491876

