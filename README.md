
### Задание 1
Вам поручили перейти на систему автоматизированной сборки **CMake**.
Исходные файлы находятся в директории [formatter_lib](formatter_lib).
В этой директории находятся файлы для статической библиотеки *formatter*.
Создайте `CMakeList.txt` в директории [formatter_lib](formatter_lib),
с помощью которого можно будет собирать статическую библиотеку *formatter*.

Шаг 1

Клонируем файл с гитхаба

<img width="785" alt="Снимок экрана 2023-03-27 в 19 12 14" src="https://user-images.githubusercontent.com/102604371/228526090-b6d2572f-6ffb-4e1c-aca9-5211460fb7f0.png">

Шаг 2

Прописываем CMakeLists

<img width="773" alt="Снимок экрана 2023-03-27 в 19 25 02" src="https://user-images.githubusercontent.com/102604371/228526215-88d61e51-ca79-4612-a853-8cfa22017528.png">

Шаг 3

Билдим файл

<img width="762" alt="Снимок экрана 2023-03-27 в 19 28 00" src="https://user-images.githubusercontent.com/102604371/228526312-4ed429a8-fd98-44a4-80dd-15d6052325c3.png">


<img width="767" alt="Снимок экрана 2023-03-27 в 19 29 26" src="https://user-images.githubusercontent.com/102604371/228526322-4d141ef7-a971-4111-813a-3257eb54fa00.png">




### Задание 2
У компании "Formatter Inc." есть перспективная библиотека,
которая является расширением предыдущей библиотеки. Т.к. вы уже овладели
навыком созданием `CMakeList.txt` для статической библиотеки *formatter*, ваш 
руководитель поручает заняться созданием `CMakeList.txt` для библиотеки 
*formatter_ex*, которая в свою очередь использует библиотеку *formatter*.

Шаг 1

Прописываем CMakeLists для formatter_ex и связываем его с formatter

<img width="767" alt="Снимок экрана 2023-03-27 в 19 47 49" src="https://user-images.githubusercontent.com/102604371/228526408-7f99d387-32ee-4c6c-9c19-1e7b8fd7c213.png">



Шаг 2

Билдим

<img width="758" alt="Снимок экрана 2023-03-27 в 19 49 56" src="https://user-images.githubusercontent.com/102604371/228526556-44dd0808-f141-47f5-aeee-cb140803392f.png">




### Задание 3
Конечно же ваша компания предоставляет примеры использования своих библиотек.
Чтобы продемонстрировать как работать с библиотекой *formatter_ex*,
вам необходимо создать два `CMakeList.txt` для двух простых приложений:
* *hello_world*, которое использует библиотеку *formatter_ex*;
* *solver*, приложение которое испольует статические библиотеки *formatter_ex* и *solver_lib*.

Шаг 1

Прописываем CMAkeLists для solver

<img width="777" alt="Снимок экрана 2023-03-27 в 20 11 36" src="https://user-images.githubusercontent.com/102604371/228526735-bdf97345-3668-4135-bacd-116c86f8798d.png">

Шаг 2

Подключаем и связываем библиотеки

<img width="756" alt="Снимок экрана 2023-03-27 в 20 20 20" src="https://user-images.githubusercontent.com/102604371/228526807-4b88d3f4-3250-40f7-817e-83db7fa30b48.png">

Шаг 3 

Добавляем субкаталоги к сборке

<img width="766" alt="Снимок экрана 2023-03-27 в 20 33 45" src="https://user-images.githubusercontent.com/102604371/228526871-2a56766a-9ea0-4d72-8b7e-ff02674c1cdd.png">

Шаг 4 

Билдим

<img width="757" alt="Снимок экрана 2023-03-27 в 20 39 00" src="https://user-images.githubusercontent.com/102604371/228526936-b73918c3-a2c4-4f59-becb-2cbb6630ae7a.png">

Шаг 5

Получаем результат

<img width="765" alt="Снимок экрана 2023-03-27 в 20 39 53" src="https://user-images.githubusercontent.com/102604371/228527064-7147a9eb-cec5-4459-81cf-580b5c820714.png">

Шаг 6

Билдим

<img width="755" alt="Снимок экрана 2023-03-27 в 20 41 56" src="https://user-images.githubusercontent.com/102604371/228527167-5beeeeb6-38b1-4b98-8b87-baa52d2da715.png">


Шаг 7

Получаем результат

<img width="764" alt="Снимок экрана 2023-03-27 в 20 43 01" src="https://user-images.githubusercontent.com/102604371/228527268-b7af0154-85ad-4402-87f7-76dce74def36.png">


