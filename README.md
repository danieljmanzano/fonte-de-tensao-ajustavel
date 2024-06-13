# Fonte de tensão ajustável
*trabalho da disciplina Eletronica para Computação - SSC0180*
# Tabela dos componentes

# Componentes
- **transformador**: tem o papel de diminuir a voltagem que o circuito recebe a partir da fonte corrente alternada (tomada). a partir da voltagem de 127V recebida, o transformador consegue diminuí=la para a faixa de tensão desejada (3V a 12V).
- **ponte de diodo**: uma junção de 4 diodos que têm a capacidade de transformar a tensão alternada (vinda da tomada) em contínua.
- **capacitor**: armazena carga no circuito nos ciclos da corrente alternada, liberando corrente quando a tensão da fonte é menor do que a tensão interna. ele descarrega sua carga armazenada quando há a inversão do ciclo no circuito. com base em cálculos de um ripple de 10%, chegamos próximos do valor comercial de 470uF de capacitância, usando um capacitor com esse valor no projeto.
- **diodo zener**: tem o intuito de regular a corrente máxima, sendo o usado especificamente de voltagem máxima de 13V. quando a ddp passa de 13V, ele mantém esse valor em seus terminais; quando a ddp chega menor do que 13V, ele não conduz e consequentemente não interfere no circuito.
- **potenciômetro**: é um resistor variável usado como controle da tensão resultante, que permite atingir as ddps de 3V a 12V no circuito.
- **transistor**: amplifica a corrente que recebe em sua base para um valor desejado, sendo o máximo de 100mA
- **resistores**: usados em mais de um momento no circuito, têm a função de limitar a corrente, garantindo certa "segurança" aos componentes. no circuito, usamos eles associados ao led, ao zener, ao potenciômetro e ao transistor.
- **led**: tem função de indicar o nível da corrente atingida na parte final do circuito, brilhando mais quando a voltagem e a corrente são maiores. de modo geral, não interfere nos valores obtidos no circuito, servindo unicamente como indicação da voltagem e corrente ajustáveis.

# Imagem do circuito no Falstad
![Captura de tela 2024-06-11 105750](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/e3c710aa-9977-4a19-93ae-4c3c98ba290d)
   link para o falstad: https://tinyurl.com/2cbdos5r

# PCB no Eagle
![Captura de tela 2024-06-12 210140](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/a610be01-ebc5-4f92-b6d7-2eceea460e35)

# Esquemático no Eagle
![Captura de tela 2024-06-12 204952](https://github.com/danieljmanzano/fonte-de-tensao-ajustavel/assets/162331747/86f89c07-bab1-40e5-bc8c-1dc4eaa14497)



