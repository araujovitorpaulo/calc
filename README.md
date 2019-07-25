# python_basics_calc
Calculadora com operações básicas.
Criada a partir da linguagem Python

    exit = False
    print("---------------------------------------------")
    lang = input("Select your language (en/pt): ")
    if lang == "en":
        print("Welcome to Paulo Vitor's Calculator v1.0")
        while exit == False:
            num1 = input("Type the first number: ")
            num1 = float(num1)
            op = input("What operator do you want do use (+, -, *, /, **): ")
            num2 = input("Type the second number: ")
            num2 = float(num2)

            available_ops = "+", "-", "*", "/", "**"

            if op == "+":
                result = num1 + num2
                result = int (result)
                print("The result is: ", result)

            elif op == "-":
                result = num1 - num2
                print("The result is: ", result)

            elif op == "*":
                result = num1 * num2
                print("The result is: ", result)

            elif op == "/":
                result = num1 / num2
                print("The result is: ", result)

            elif op == "**":
                result = num1 ** num2
                print("The result is: ", result)

            elif op != available_ops:
                print("Invalid operator")

            leave = input("Do you want to leave (y/n)?")
            if leave == "y" or "Y":
                exit = True
                print("Exiting now...")

    elif lang == "pt":
        print("Bem vindo à Calculadora do Paulo Vítor versão 1.0")
        while exit == False:
            num1 = input("Digite o primeiro número: ")
            num1 = float(num1)
            op = input("Qual operador você deseja usar? (+, -, *, /, **): ")
            num2 = input("Digite o segundo número: ")
            num2 = float(num2)

            available_ops = "+", "-", "*", "/", "**"

            if op == "+":
                result = num1 + num2
                print("O resultado é: ", result)

            elif op == "-":
                result = num1 - num2
                print("O resultado é: ", result)

            elif op == "*":
                result = num1 * num2
                print("O resultado é: ", result)

            elif op == "/":
                result = num1 / num2
                print("O resultado é: ", result)

            elif op == "**":
                result = num1 ** num2
                print("O resultado é: ", result)

            elif op != available_ops:
                print("Operador inválido")

            leave = input("Você deseja sair?(s/n)")
            if leave == "s" or "S":
                exit = True
                print("Saindo...")
