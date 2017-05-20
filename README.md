# Geese And Guns
### Про гру
Суть гри заключається у тому, щоб за **1 хвилину** вцілити у якомога більшу кількість пташок.
### Принцип роботи
Для визначення потрапляння у ціль (пташку) використано наступний алгоритм:
* Замість рендеру гри на короткий проміжок відобразити цілком залитий чорним екран
* Зняти дані про рівень рівень освітленості з *фіотодіоду*
* Відобразити замість пташки білий квадрат на короткий проміжок часу
* Зняти дані про рівень рівень освітленості з *фіотодіоду* вдруге
* Якщо інформація про рівень освітленості першого разу і другого суттєво відрізняється, то в ціль **влучено**
![Схема](https://raw.githubusercontent.com/potterua/GeeseAndGuns/master/chart.png)
### Підключення
Підключення *пістолету* до *Arduino* здійснюється за допомогою **4 проводків**:
1. Відповідає за зчитування інформації з фотодіоду *(аналоговий пін **A4**)*
2. Відповідає за  перевірку стана спускового гачка *(цифвроий пін **D7**)*
3. Напргуа **(5V)**
4. Заземлення **(GND)**
### Принципова схема пістолета
![Схема](https://github.com/potterua/GeeseAndGuns/raw/master/scheme.png)
### Перший запуск гри
1. Встановити драйвер для роботи з *COM* портом *Arduino UNO* [**[Завантажити]**](https://www.arduino.cc/en/Main/Software)
2. Перезавантажити комп'ютер
3. Запустити гру
