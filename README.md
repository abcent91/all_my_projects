# all_my_projects
python_learning
def butterbrod (bread_loaves, butter_grams, chees_grams, sausage_grams):
    bread_loaves = int(input('Сколько батонов хлеба? '))
    while bread_loaves == 0:
        print('Без хлеба не будет бутербродов :-)')
        bread_loaves = int(input('Сколько батонов хлеба? '))

    butter_grams = int(input('Сколько грамм масла? '))
    while butter_grams == 0:
        print('Без масла не будет бутербродов :-)')
        butter_grams = int(input('Сколько грамм масла? '))

    chees_grams = int(input('Сколько грамм сыра? '))
    while chees_grams == 0:
        print('Без сыра не будет бутербродов :-)')
        chees_grams = int(input('Сколько грамм сыра? '))

    sausage_grams = int(input('Сколько грамм колбасы? '))
    while sausage_grams == 0:
        print('Без колбасы не будет бутербродов :-)')
        sausage_grams = int(input('Сколько грамм колбасы? '))

    bread = (bread_loaves * 15) // 2
    butter = butter_grams // 5
    chees = chees_grams // 10
    sausage = sausage_grams // 10
    amount = min(bread, butter, chees, sausage)
    return amount
print('Вы можете приготовить', butterbrod(0,0,0,0), 'бутербродов')
