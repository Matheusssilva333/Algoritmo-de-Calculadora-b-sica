
programa {


    funcao inicio() {
        real num1, num2, resultado
        cadeia operacao
        
        escreva("Digite o primeiro número: ")
        leia(num1)
        
        escreva("Digite o segundo número: ")
        leia(num2)
        
        escreva("Escolha a operação (soma | subtracao | multiplicacao | divisao): ")
        leia(operacao)
        
        escolha (operacao) {
            caso "soma":
                resultado = num1 + num2
                escreva("\nResultado da soma: ", resultado)
                pare
                
            caso "subtracao":
                resultado = num1 - num2
                escreva("\nResultado da subtração: ", resultado)
                pare
                
            caso "multiplicacao":
                resultado = num1 * num2
                escreva("\nResultado da multiplicação: ", resultado)
                pare
                
            caso "divisao":
                se (num2 != 0) {
                    resultado = num1 / num2
                    escreva("\nResultado da divisão: ", resultado)
                } senao {
                    escreva("\nErro: divisão por zero não permitida!")
                }
                pare
                
            caso-padrao:
                escreva("\nOperação inválida. Tente novamente!")
        }
    }
}
