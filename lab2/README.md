LAB
Хід роботи
За допомогою пакетного менеджера PIP інсталював pipenv та створив ізольоване середовище для Python.
pip install pipenv
pipenv --python 3.7  
pipenv shell
Встановив бібліотеки requests та ntplib у своєму середовищі.
pipenv install requests
pipenv install ntplib
Переконався що програма працює правильно.
python app.py
Результат:

========================================
Результат без параметрів: 
No URL passed to function
========================================
Результат з правильною URL: 
Time is:  10:27:23 PM
Date is:  11-10-2020
Встановив бібліотеку pytest та запустив тести, всі тести виконались успішно:
pipenv install pytest
pytest tests/tests.py
Дописав у програмі функцію, що перевіряє час доби на AM/PM та відповідно друкувати "Доброго дня/ночі". Також написав тест який перевіряє правильність роботи функції.
Перенаправив результат виконання функції та тестів у файл results.txt:
pipenv run pytest tests/tests.py >> results.txt
pipenv run python app.py append >> results.txt
Закомітив до репозиторію Makefile
Створив Makefile
Заповнив мейкфайл
Запустив мейкфайл
make