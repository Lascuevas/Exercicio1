#CRUD - 1 TENTATIVA

import os
# IMPORTANDO A BIBLIOTECA OS

RH = []
# CRIANDO UMA LISTA COM O NOME DE RH

while True:
# CRIANDO UM LOOP INFINITO QUE SÓ PARA NO BREAK

    os.system('cls')
'''
A linha os.system('cls') é usada para limpar a tela do terminal ou console. 
Aqui está um detalhamento do que ela faz:

Importação do Módulo os: Antes de usar os.system, o módulo os deve ser importado
como você fez no início do seu código. Esse módulo fornece uma maneira de interagir 
com o sistema operacional.

Comando 'cls': No Windows, o comando cls é utilizado para limpar a tela do console. 
Quando você chama os.system('cls'), o Python executa esse comando no sistema operacional.

Limpeza da Tela: Essa linha é útil para que o usuário não fique confuso com as informações acumuladas na tela. 
Ao limpar a tela antes de exibir o menu novamente, você proporciona uma interface mais limpa e organizada.

'''

    menu=input('''Seja bem-vindo ao sistema de cadastro da nossa empresa! 
O que deseja fazer?:
               
    1 - INCLUIR
    2 - ALTERAR
    3 - EXCLUIR
    4 - RELATÓRIO GERAL
    5 - PESQUISAR POR NOME
    6 - SAIR
               
Digite a opção de sua escolha ==>  ''')

    if menu == '1':
        print('Por favor, entre com os dados a seguir... ')
        matricula = input('Digite sua matrícula: ')
        nome = input('Digite seu nome: ')
        salario = float(input('Digite o valor do seu salário; '))

        RH.append([matricula, nome, salario])
        # A FUNÇÃO append SERVE PARA ADICIONAR NOVOS ELEMENTOS A FUNÇÃO

        input('Inclusão concluida, por favor, pressione <Enter> para voltar ao menu! ')
    elif menu == '2':
        for i in RH:
            print('Numero da matrícula:', i[0], '- Nome:', i[1], '- Salário:', i[2])
        input('Pressionte <Enter> para finalizar!')
    elif menu == '3':
        input('Pressione <Enter> para finalizar!')
    
