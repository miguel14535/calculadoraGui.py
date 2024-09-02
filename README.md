# Calculadora Gui.oo

![Calculadora](![Captura de tela 2024-09-02 195339](https://github.com/user-attachments/assets/a030ad06-297b-4989-9136-9e0befa00365)
) 

## Descrição

Este projeto é uma calculadora simples desenvolvida em Python utilizando a biblioteca Tkinter para a interface gráfica. A calculadora permite ao usuário realizar operações matemáticas básicas, como adição, subtração, multiplicação e divisão.

## Diagrama UML

![Diagrama UML](![Captura de tela 2024-09-02 200111](https://github.com/user-attachments/assets/9aa1a066-9adc-47b2-b7a1-0d505d727d71)
)
## Documentação das Classes e Métodos

### Classe `Display`

Esta classe herda de `tk.Entry` e é responsável pela área de exibição da calculadora.

**Construtor:**

python
def __init__(self, master):
    super().__init__(master, font=('Arial', 24), bd=10, relief='ridge', justify='right',
                     bg='#F5F5F5', fg='#333')
    self.grid(row=0, column=0, columnspan=4, padx=5, pady=5)
master: Instância do widget pai (a janela principal).

master: Instância do widget pai (a janela principal).
Propriedades:
font: Define o tipo e o tamanho da fonte.
bd: Define a espessura da borda.
relief: Define o estilo da borda.
justify: Alinha o texto à direita.
bg: Cor de fundo.
fg: Cor do texto.

Método update(text):

![Captura de tela 2024-09-02 200744](https://github.com/user-attachments/assets/697a395c-f0d5-40d7-add0-bf6e1c132d72)
Atualiza o texto exibido na área de entrada.

Classe CalculatorButton
Esta classe herda de tk.Button e representa cada botão da calculadora.

Construtor:

![Captura de tela 2024-09-02 201836](https://github.com/user-attachments/assets/ca82b804-0e90-4590-80ac-2114cbf766a7)

master: Instância do widget pai.
text: Texto exibido no botão.
command: Função a ser chamada quando o botão é clicado.
row e column: Posições na grade.

Métodos on_enter(e) e on_leave(e):

![Captura de tela 2024-09-02 201911](https://github.com/user-attachments/assets/96073940-71bf-4077-81d4-de25c62a16af)

Alteram a cor de fundo do botão ao passar e retirar o mouse.

Classe Calculator
Gerencia a lógica e a interface da calculadora.

Construtor:

![Captura de tela 2024-09-02 202146](https://github.com/user-attachments/assets/db669ee4-05c0-41b7-bff5-9ed583532056)

master: Instância da janela principal.
current_input: Armazena a expressão matemática atual.
last_result: Armazena o último resultado calculado.

Método create_widgets():

![Captura de tela 2024-09-02 202224](https://github.com/user-attachments/assets/c0cd2f26-8cae-474f-b0b1-d4f44bc07d55)

Cria e posiciona os botões da calculadora na janela.

Método button_click(value):

![Captura de tela 2024-09-02 202252](https://github.com/user-attachments/assets/d57a30d8-0d9a-4a70-9dc0-97a038c11bca)

Lida com os eventos de clique dos botões, atualiza a entrada e calcula o resultado.

##Descrição das Funcionalidades
Entrada de Números e Operações: O usuário pode inserir números e operadores matemáticos (adição, subtração, multiplicação, divisão) através dos botões.
Resultado da Operação: Ao clicar em =, a expressão matemática é avaliada e o resultado é exibido.
Limpeza: O botão C limpa a entrada e o display, permitindo que o usuário inicie uma nova operação.

## Roadmap de Execução
Inicialização: O aplicativo é iniciado com a criação da janela principal (root) e da instância de Calculator.
Tela Principal: O usuário interage com a tela principal para realizar cálculos.
Operações: Ao clicar nos botões, a expressão é atualizada e, ao clicar em =, o resultado é calculado e exibido.
Limpeza: Permite ao usuário limpar a entrada e o display com o botão C.

## Manual de Instalação e Uso
Dependências
tkinter: Para criar a interface gráfica do usuário.

## Instalação
Tkinter geralmente vem pré-instalado com o Python. Se necessário, você pode instalar Tkinter usando o gerenciador de pacotes apropriado para sua distribuição Python.

## Inicialização
Para iniciar o programa, execute o seguinte comando no terminal:

![Captura de tela 2024-09-02 202410](https://github.com/user-attachments/assets/cbd7e904-b3fa-4caf-b09d-0c2885ef7a7d)
