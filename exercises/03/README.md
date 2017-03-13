Упражнение 3
============

Студент
----------------------
Да се реализира клас `Student`, представящ студент във ФМИ.
Нека кажем, че всеки студент има винаги по 5 предмета от предишния семестър.
Класът да включва следните член-данни:
* Име(сиимволен низ до 30 символа)
* Курс(положително число от 1 до 4)
* Факултетен номер(цяло положително число)
* Оценки от предишния семестър (Масив от 5 цели числа, *Забележка*: ако студентът е първи курс и първи семестър, масивът е пълен с 0)

Член-данните да са капсулирани (това означава член-данните да бъдат `private`).


Класът трябва да има конструктор по подразбиране,конструктор с параметри,селектори(getters) и мутатори(setters).

Да се дефинира член-функция `getGPA()`, която връща средната оценка на студента от предишния семестър.
Пример:
```cpp
int grades[5] = { 6,5,4,6,5 };

Student gosho("Gosho",1,75251,grades);

pesho.getGPA() // трябва да върне 5.2	
```

Да се дефинира член-функция `print`, която извежда информация за студента.
Пример:
```cpp
int grades[5] = { 6,5,4,6,4 };

Student pesho("Pesho",1,755255,grades);

pesho.print(); // Това трябва да изведе на стандартния изход: Name: Pesho, Course: 2, FN: 755255, GPA: 5.00
```


Група
----------
Да се реализира клас `Group`, представящ група на студенти във ФМИ.
Класът да включва следните член-данни:
* Брой на студенти в групата(цяло неотрицателно число)
* Студенти(Масив с големина броя студенти в групата)

Член-данните да са капсулирани (това означава член-данните да бъдат `private`).


Класът трябва да има конструктор по подразбиране,конструктор с параметри,селектори(getters) и мутатори(setters).

Да се дефинира член-функция `getScholarshipStudents()`, която връща броя на студентите в групата, които взимат стипендия.
Един студент взима стипендия ако средния успех му е по-голям от 4.50 .

Да се дефинира член-функция `getGroupGPA()`, която връща средната оценка на цялата група.

Да се дефинира член-функция `findStudent(char[30] name)`, която търси дали съществува студент с такова име в групата(Връща индекс).

Да се дефинира член-функция `findStudent(int FN)`, която търси дали съществува студент с такъв факултетен номер в групата(Връща индекс).

Да се дефинира член-фунцкия `changeFN(char[30] name,int newFN)` която променя факултетния номер на студента с името, подадено като аргумент, или казва че не съществува такъв студент.

Да се дефинира член-функция `print`, която извежда всички студенти в групата.


*ДА СЕ НАПИШЕ ФУНКЦИЯ, КОЯТО СЪЗДАВА ГРУПА ОТ 5 СТУДЕНТА. СЛЕД СЪЗДАВАНЕТО НА ГРУПАТА ДА СЕ КАЖЕ КОЛКО СТУДЕНТИ ВЗИМАТ СТИПЕНДИЯ, КАКЪВ Е СРЕДНИЯ УСПЕХ НА ГРУПАТА И ДА СЕ ИЗПЕЧАТАТ ВСИЧКИ СТУДЕНТИ В ГРУПАТА.*

