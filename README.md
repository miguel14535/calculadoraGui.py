# Calculadora Tkinter

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

Propriedades:
font: Define o tipo e o tamanho da fonte.
bd: Define a espessura da borda.
relief: Define o estilo da borda.
justify: Alinha o texto à direita.
bg: Cor de fundo.
fg: Cor do texto.

Método update(text):

![Captura de tela 2024-09-02 200744](https://github.com/user-attachments/assets/01822960-17af-4ef0-81d8-60fecc2303d0)

