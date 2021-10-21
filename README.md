# nosql2h2021-accidents-mapping
## Сценарий использования - «Получение информации о конкретной модели»:

Действующее лицо: Пользователь 

Основной сценарий: 

1. Пользователь заходит на главную страницу. *Ответ системы: Загрузка главной страницы.* 
2. Пользователь выбирает из каталога нужную ему марку и кликает на логотип марки | Пользователь ищет нужную ему марку через строку поиска и кликает на логотип марки. *Ответная реакция системы: Обновление и загрузка марок, удовлетворяющих условиям поиска. Переход и загрузка страницы марки.*
3. Пользователь выбирает интересующую его модель данной марки и кликает на её изображение | Пользователь выбирает интересующую его модель данной марки через строку поиска и кликает на её изображение. *Ответная реакция системы: Обновление и загрузка моделей, удовлетворяющих условиям поиска. Переход и загрузка страницы модели.*

**Результат:** Пользователь изучает информацию о поколениях и характеристиках данной модели. 

**Альтернативный сценарий:** 

* Пользователь не нашел нужную ему модель. 
* Пользователь нашел похожую модель. 
* На странице марки Пользователь захотел посмотреть статистику о ДТП


## Сценарий использования - «Получение информации о ДТП»:

Действующее лицо: Пользователь 

**Предусловие:** Пользователь уже находится на странице определенной марки (пункты 1 и 2 сценария «Получение информации о конкретной модели»).

Основной сценарий: 

1. Пользователь кликает на “Statistics” и переходит на следующую страницу. *Ответная реакция системы: загрузка страницы Statistics.*
2. Пользователь настраивает отображение статистики в виде графика по следующим характеристикам: по оси y - Общая смертность, Смертность с участием одного авто, Смертность с участием нескольких авто; по оси x - модели, года, тип или размер модели. Пользователь кликает на желаемые параметры. *Ответная реакция системы: Выбранные параметры выделяются цветом и жирной черной рамкой.*
3. Пользователь нажимает на кнопку Построить и смотрит на полученные результаты, отрисованные на графике ниже. *Ответная реакция системы: На странице в рамку, выделенную пунктиром, загружается график, построенный по заданным параметрам.*

**Результат:** Пользователь изучает полученные результаты. *(Пользователь хочет узнать иную статистику. Переход либо на шаг 2 (если интересует эта же марка), либо на главную страницу (если другая) - он может нажать на текст Cars | Home (верхний левый угол) соответственно. Ответная реакция системы: Обновление графика (Пользователь выбрал другие параметры и нажал “Построить”) | Переход на начало веб-каталога (если Пользователь нажал на Cars)* *с помощью ссылки-якоря| Переход на самый верх главной страницы (если Пользователь нажал на Home)* *с помощью ссылки-якоря. )*

**Альтернативный сценарий:** Пользователь не нашел нужную ему модель.


## Сценарий использования - «Пользователь не нашел нужную ему модель»:

Действующее лицо: Пользователь 

**Предусловие:** Пользователь уже находится на странице нужной марки (пункты 1 и 2 сценария «Получение информации о конкретной модели»).

Основной сценарий:

1. Пользователь заходит на главную страницу. *Ответная реакция системы: Загрузка главной страницы.*
2. Пользователь выбирает из списка нужную ему марку и кликает на ее логотип | Пользователь ищет нужную ему марку через строку поиска и кликает на ее логотип. *Ответная реакция системы: Обновление и загрузка марок, удовлетворяющих условиям поиска. Переход и загрузка страницы марки.*

**Результат**: Пользователь не нашел нужной ему модели. По желанию он может вернуться на главную страницу или перейти к веб-каталогу (Home | Cars(верхний левый угол)).

**Альтернативный сценарий:** 

* Пользователь нашел нужную ему модель. 
* Пользователь нашел похожую модель.
* На странице марки Пользователь захотел посмотреть статистику о ДТП.


## Сценарий использования - «Просмотр визуализации»:

Действующее лицо: Пользователь 

Основной сценарий:

1. Пользователь заходит на главную страницу. *Ответная реакция системы: Загрузка главной страницы.* 
2. Пользователь кликает на текст Visualization. *Ответная реакция системы: Переход и загрузка страницы визуализации.*
3. Пользователь настраивает отображение данных в виде графика по следующим характеристикам: по оси x - Значение максимальной скорости, Ускорение, Тип машины, Запас топлива, Тип топлива; по оси y - Выбор марки автомобиля из списка всех марок, или выбор сразу всех марок. Пользователь кликает на желаемые параметры. *Ответная реакция системы:  Выбранные параметры выделяются цветом и подставляются в окошко.*
4. Пользователь нажимает на кнопку Построить и смотрит на полученные результаты. *Ответная реакция системы: На странице в рамку, выделенную пунктиром, загружается график, построенный по заданным параметрам.*

**Результат:** Пользователь изучает полученные результаты. *(Пользователь хочет узнать иную статистику. Переход либо на шаг 3, либо на страницу конкретной марки (см. сценарий “Получение информации о ДТП”). Ответная реакция системы: Обновление графика (Пользователь выбрал другие параметры и нажал “Построить” | Переход на главную страницу.)* 

**Альтернативный сценарий:** 

* Пользователь захотел посмотреть статистику о ДТП
* Пользователь захотел узнать информацию о моделях


## Сценарий использования - «Выгрузка базы данных»:

Действующее лицо: Пользователь 

*Основной сценарий:* 

1. Пользователь заходит на главную страницу. *Ответная реакция системы: Загрузка главной страницы.* 
2. Пользователь кликает квадратную стрелку вниз на белом фоне в правом нижнем углу страницы. *Ответная реакция системы: начало загрузки БД на компьютер Пользователя.*

**Результат:** Пользователь получает базу данных.

**Альтернативный сценарий:** Пользователь захотел загрузить базу данных.


## Сценарий использования - «Загрузка базы данных»:

 Действующее лицо: Пользователь 

Основной сценарий: 

1. Пользователь заходит на главную страницу. *Ответная реакция системы: Загрузка главной страницы.*
2. Пользователь кликает квадратную стрелку вверх на белом фоне в правом нижнем углу страницы. *Ответная реакция системы: открывается окно выбора файла, затем загрузка и обработка полученной БД, загрузка главной обновленной страницы.*

**Результат:** Пользователь загрузил базу данных.

**Альтернативный сценарий:** Пользователь захотел выгрузить базу данных.


## Макет пользовательского интерфейса:

![maket 2](https://user-images.githubusercontent.com/42918083/138223956-aea44069-1688-41a6-b513-5bf24df307a9.png)
