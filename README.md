# calculator

def calculator():


        print("простой калькулятор.")
        print("выберете операцию: +, -, *, /")
        operation = input("Введите операцию: ")
        if operation in ['+','-','*','/']:
            num1 = float(input("Введите первое число: "))
            num2 = float(input("Введите второе число: "))

            try:
                if operation == '+':
                    result = num1 + num2
                elif operation == '-':
                    result = num1 - num2
                elif operation == '*':
                    result = num1 * num2
                elif operation == '/':
                    result = num1 / num2


                return f"Результат: {result}"
            except Exception as e:
                print("Неверная операции", e)
            finally:
                print("Попробуйте что-то другое.")
while True:
    print(calculator())
