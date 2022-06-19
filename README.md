# Desafio-bar-


Var

   sexo , F, M : caractere
   quantCerveja, quantRefrigerante, quantEspetinho, cerveja, refrigerante, espetinho, couvert, consumo, ingressoF, ingressoM, valorTotalM, valortotalF :real


Inicio

    escreva("Escreva qual o sexo (F/M):")
    leia (sexo)
    escreva("Escreva a Quantidade de cerveja ")
    leia(quantCerveja)
    escreva("Escreva a quantidade de refrigerante")
    leia(quantRefrigerante)
    escreva("Escreva a quantidade de espetinho ")
    leia(quantEspetinho)
    escreval()


    couvert <- 4.00
    cerveja <- 5.00
    refrigerante <- 3.00
    espetinho <- 7.00
    ingressoF <- 8.00
    ingressoM <- 10.00

    consumo <- (cerveja * quantCerveja) + (refrigerante * quantRefrigerante) + (espetinho * quantEspetinho)
    valorTotalM <- consumo + ingressoM
    valorTotalF <- consumo + couvert + ingressoF

    se(consumo > 30.0)e (sexo = "F") entao
    escreval("Relatório:")
    escreval()
    escreval("consumo = R$ " , consumo:4:2)
    escreval("Isento de couvert")
    escreval("Ingresso = R$ " , ingressoF:4:2)
    escreval("valor a pagar - R$ " , valorTotalF:4:2)
    senao
        se(consumo > 30.0)e (sexo = "M") entao
        escreval("Relatório:")
        escreval()
        escreval("consumo = R$ " , consumo:4:2)
        escreval("Isento de couvert")
        escreval("Ingresso = R$ " , ingressoM:4:2)
        escreval("valor a pagar - R$ " , valorTotalM:4:2)
        senao
            se(consumo < 30.0)e (sexo = "F") entao
            couvert <- 4.00
            escreval("Relatório:")
            escreval()
            escreval("consumo = R$ " , consumo:4:2)
            escreval("Ingresso = R$ " , ingressoF:4:2)
            escreval("Couvert = R$ " , couvert:4:2 )
            escreval("valor a pagar - R$ " , valorTotalF:4:2)
            senao
                se(consumo < 30.0)e (sexo = "M") entao
                couvert <- 4.00
                escreval("Relatório:")
                escreval()
                escreval("consumo = R$ " , consumo:4:2)
                escreval("Ingresso = R$ " , ingressoM:4:2)
                escreval("Couvert = R$ " , couvert:4:2 )
                escreval("valor a pagar - R$ " , valorTotalM:4:2)

                fimse
            fimse
        fimse
    fimse
