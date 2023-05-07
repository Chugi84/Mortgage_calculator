rate=20
region = input('Регион проживания:')
if region == 'Дальний Восток':
  rate -= 18
else:
  num_child = int(input('Количество детей:'))
  if num_child > 3:
    rate -= 1
  salary_project = input('Зарплатный проект:')
  if salary_project == 'Да':
    rate -= 0.5
  insurance = input('Оформление страхования:')
  if insurance == 'Да':
    rate -= 1.5
print(f'Ваша ставка: {rate} %')