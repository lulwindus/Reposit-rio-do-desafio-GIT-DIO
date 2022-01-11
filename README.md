# Reposit-rio-do-desafio-GIT-DIO
O projeto é um radar para carros.
#Aplicador de multa
print(f"Olá eu sou o Multador, se passar na minha mira só chega a multa")
Kc= int(input(f"Qual velocidade o carro passou em km: "))
Kp= int(input(f"Qual velocidade máxima permitida em km: "))
#Constante das %
Kr= int(Kp*10/100)+Kp
Kt= int(Kp)-(Kp*20/100)
Kr1= int(Kp*15/100)+Kp
VI= int(50)
VII= int(100)
#se A velocidade do carro for maior que 110% da velocidade da via
if Kc<=Kr1 and Kc>=Kr:
    print(f"Vai tomar multa")
    print(f"Enviar o valor de: {VI:4.2f}R$ de multa para o infrator")
    V=input(f"o Cidadão reside em que cidade?: ")
    if str("sp") in V:
        print (f" Vai pagar só a multa, sem taxa adicional.")
        print (f"Volte sempre")
    if str("cubatao") in V:
        print (f"Devido a localização, se  adiciona 80 Reais")
        print(f"Valor a pagar: {80+VI:4.2f} R$")
        print (f"Volte sempre")
    elif str("outra") in V:
       print (f"Vai pagar 10 Reais  a mais de custo logistico")
       print (f"Vai pagar: {VII+10}")
       print (f"Volte sempre")
#se A velocidade do carro for maior que 115% da velocidade da via
if Kc>=Kr1:
    print(f"Tá rapido entao, né?")
    print(f"Envar o valor de: {VII:4.2f} R$ de multa para o infrator")
#Codificação da taxação Logística por Km
    V=input(f"o Cidadão reside em que cidade?: ")
    if str("sp") in V:
        print (f" Vai pagar só a multa, sem taxa adicional.")
    if str("cubatao") in V:
        print(f"Valor a pagar: {80+VII:4.2f} R$")
        print(80+VII)
    elif str("outra") in V:
       print (f"Vai pagar 10$ a mais de custo logistico")
       print (f"Volte sempre")
if Kc<Kt:
    print (f"Tá devagar demais rapa, paga ai uns 20 conto pra deixar de ser tartaruga")
    print (f"Pagar: 20 R$\n vai na paz")
#se a velocidade for menor
else:
    print (f"Cidadão tá de boa, deixa ir na paz")
   

