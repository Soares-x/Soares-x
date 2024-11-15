
import random

def jogo_adivinhacao():
    print("Bem-vindo ao jogo de adivinhação!")
    print("Estou pensando em um número entre 1 e 100.")
    
    # Gera um número aleatório entre 1 e 100
    numero_secreto = random.randint(1, 100)
    tentativas = 0
    
    while True:
        try:
            # Solicita um palpite ao jogador
            palpite = int(input("Digite seu palpite: "))
            tentativas += 1

            if palpite < numero_secreto:
                print("Muito baixo! Tente novamente.")
            elif palpite > numero_secreto:
                print("Muito alto! Tente novamente.")
            else:
                print(f"Parabéns! Você adivinhou o número em {tentativas} tentativas.")
                break
        except ValueError:
            print("Por favor, insira um número válido.")

# Executa o jogo
jogo_adivinhacao()
<!---
Soares-x/Soares-x is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
