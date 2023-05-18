while True:
    # Solicita informações do usuário
    apolice = input("Digite o numero da apólice: ")
    cpf = input("Digite o seu CPF: ")
    alteracao = input("O veículo sofreu alguma alteração?Digite 's' para sim ou 'n' para não:")
    if alteracao.lower()== "n":
      print("Ok,")
    elif alteracao.lower()== "s":
     tipo_alteracao = input("Qual alteração foi feita? ")
     print("Entendi a alteração feita foi:",tipo_alteracao)
    else:
       print("Desculpe, não entendi a resposta. Por favor, responda com 's' ou 'n'.") 
    
    
    # Usuário escolhe o tamanha do veiculo
    modalidade = peso_veiculo
    peso_veiculo = float(input("Digite o peso do veículo: "))
    if peso_veiculo <= 2.5 :
        print("O guicho certo é a modalidade plataforma.")
    elif peso_veiculo <= 4.0 :
       print("O guincho certo é a modalidade guincho cegonha.")
    elif peso_veiculo <= 6.0 :
        print("O guincho certo é a modalidade guincho rotativo. ")
    elif peso_veiculo <= 8.0 :
        print("O guincho certo é a modalidade guincho prancha rebaixada.")



         # Exibe um resumo da operação realizada
    print(f"Operação realizada:\nApolice: {apolice}\nCPF: {cpf}\nModalidade de atendimento: {modalidade}")


    # Pergunta se o usuário deseja realizar uma nova operação ou encerrar o atendimento
    resposta = input("Deseja realizar uma nova operação? Digite 's' para sim ou 'n' para não: ")
    if resposta.lower() == 'n':
        break

print("Atendimento encerrado.")
