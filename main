import random

right = int(input('Введите правую границу: '))


def is_valid(num, r):
    return num.isdigit() and 1 <= int(num) <= r and int(num) == float(num)


n = random.randint(1, right)
count = 0
print('Добро пожаловать в числовую угадайку')
while True:
    dig = input(f'Введите целое число от 1 до {right}: ')
    if not is_valid(dig, right):
        print(f'А может быть все-таки введем целое число от 1 до {right}')
        continue
    dig = int(dig)
    if dig < n:
        print('Ваше число меньше загаданного, попробуйте еще разок')
        count += 1
        continue
    elif dig > n:
        count += 1
        print('Ваше число больше загаданного, попробуйте еще разок')
        continue
    else:
        count += 1
        print('Спасибо, что играли в числовую угадайку. Еще увидимся...', f'Количество попыток: {count}')
    if input('Хотите сыграть еще раз? y or n ') == 'y':
        n = random.randint(1, right)
        right = int(input('Введите правую границу: '))
        count = 0
        continue
    else:
        break
