
### <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/82/Gnu-bash-logo.svg/2560px-Gnu-bash-logo.svg.png" title="bash logo" alt="bash logo" width="400" height="150"/> 
### Работа с командной строкой BASH
<hr>
Мной был установлен и настроен GitBASH и VSCode. С помощью которых можно взаимодействовать с сервером.<br>
 С заданием и решением к ним можно ознакомиться ниже.



<body>
<table border="1">
  <tr><th>№</th><th>Команда</th><th>Описание</th></tr>
  <tr><td>1</td><td>$ cd ~</td><td>Открыть домашнюю директорию</td></tr>
  <tr><td>2</td><td>$ pwd</td><td>Определить имя папки, в которой вы находитесь</td></tr>
  <tr><td>3</td><td>$ mkdir test1</td><td>Создать внутри этой папки каталог с именем test1</td></tr>
  <tr><td>4</td><td>$ cd test1</td><td>Перейти в папку test1</td></tr>
  <tr><td>5</td><td>$ touch {1,2,3}.txt</td><td>Создать файл 1,2 и 3 внутри каталога test1</td></tr>
  <tr><td>6</td><td>$ ls</td><td>Проверить содержимое каталога test1</td></tr>
  <tr><td>7</td><td>$ cd ..</td><td>Перейти в домашнюю директорию</td></tr>
  <tr><td>8</td><td>$ mkdir test2</td><td>Создать папку test2 внутри домашней директории</td></tr>
  <tr><td>9</td><td>$ rmdir test2</td><td>Удалить папку test2</td></tr>
  <tr><td>10</td><td>$ rm test1/2.txt</td><td>Удалить файл 2 из папки test1</td></tr>
  <tr><td>11</td><td>$ mkdir test3 & touch test3/{1,2}.txt</td><td>Создать папку в домашней директории test3<br> и добавить в нее два файла</td></tr>
  <tr><td>12</td><td>$ rm -rf test3</td><td>Удалить папку test3</td></tr>
  <tr><td>13</td><td>$ mkdir test4</td><td>Создать папку test4 в домашней директории</td></tr>
  <tr><td>14</td><td>$ mv test1/{1,3}.txt test4</td><td>Переместить файлы 1 и 3 из папки test1 в папку test4</td></tr>
  <tr><td>15</td><td>$ echo -e "line\nline\nline" >> test4/1.txt</td><td>Добавить в файл 1 три строки со словами line</td></tr>
  <tr><td>16</td><td>$ cat test4/1.txt</td><td>Посмотреть содержимое файла 1</td></tr>
  <tr><td>17</td><td>$ echo -e "line\nline\nline" >> test4/3.txt</td><td>Добавьте в файл 3 три строки со словами line</td></tr>
  <tr><td>18</td><td>$ cat test4/{1,3}.txt</td><td>Просмотрите содержимое двух файлов (1 и 3) сразу</td></tr>
  <tr><td>19</td><td>$ vim test4/1.txt(Во всех строках вместо "line" ввел "Zero")<br>:wq (для выхода из режима редактора)</td><td>Используя один из редакторов замените все строки в файле 1</td></tr>

</table>



Таблица2
<body>
<table border="1">
  <tr><th>№</th><th>Команда</th><th>Описание</th></tr>
  <tr><td>1</td><td>$ cd ~</td><td>Зайти в домашнюю директорию</td></tr>
  <tr><td>2</td><td>$ mkdir test3</td><td>Создать папку test3</td></tr>
  <tr><td>3</td><td>$ echo -e "row1\nrow2\nrow3\nrow4" <br>
  > test3/4.txt && echo -e "row1\nrow2\nrow3\nrow4" <br>
  > test3/5.txt && echo -e "row1\nrow2\nrow3\nrow4" <br>
  > test3/6</td><td>Добавить в папку test3 три файла 4, 5 и 6,<br> в каждом из которых должно быть по 4 строки row1, row2, row3, row4</td></tr>
  <tr><td>4</td><td>$ grep "row2" test3/5.txt</td><td>Найдите строку row2 в файле 5</td></tr>
  <tr><td>5</td><td>$ grep -R "row" test3</td><td>Найдите строку row в папке test3</td></tr>
  <tr><td>6</td><td>$ grep -c "row" test3/6.txt</td><td>Посчитайте сколько строк с содержимым row в файле 6</td></tr>
  <tr><td>7</td><td>$ find test3 -name "5.txt"</td><td>Найдите файл 5 внутри папки test3</td></tr>
  <tr><td>8</td><td>$ find test3 -name "5.txt" -delete</td><td>Используя команду find, удалите файл 5</td></tr>
  <tr><td>9</td><td>$ echo "test" >> test3/4.txt</td><td>Используя команду echo, добавьте слово test в файл 4</td></tr>
  <tr><td>10</td><td>$ sed  -i 's/test/fail/g' test3/4.txt</td><td>Замените слово test в файле 4 на fail</td></tr>
  <tr><td>11</td><td>$ echo  "test" >> test3/4.txt</td><td>Добавьте в файл 4 слово test так, чтобы сохранилось содержимое</td></tr>
  <tr><td>12</td><td>$ ps aux</td><td>Просмотрите все процессы для юзеров не <br>только в консоли, которые происходят в системе</td></tr>
  <tr><td>13</td><td>$ kill 666</td><td>Убейте процесс 666 в консоли</td></tr>
  <tr><td>14</td><td>$ ping artsiomrusau.com</td><td>Узнайте доступность ресурса artsiomrusau.com, используя ping</td></tr>
  <tr><td>15</td><td>$ ping -n 5 artsiomrusau.com</td><td>Отправьте 5 пакетов на сайт artsiomrusau.com</td></tr>
  <tr><td>16</td><td>$  curl -X 'GET' \<br>
	>   'https://petstore.swagger.io/v2/pet/findByStatus?status=available' \<br>
	>   -H 'accept: application/json'</td><td>Используя GET и команду curl, получите информацию<br> о зарегистрированных питомцах на https://petstore.swagger.io/</td></tr>
  <tr><td>17</td><td>$ curl -X 'POST' \
  'https://petstore.swagger.io/v2/user' \
  -H 'accept: application/json' \<br>
  -H 'Content-Type: application/json' \<br>
  -d '{<br>
  "id": 589,<br>
  "username": "Moni",<br>
  "firstName": "Monika",<br>
  "lastName": "Blansh",<br>
  "email": "Moni@test.test",<br>
  "password": "34567",<br>
  "phone": "12345678",<br>
  "userStatus": 0
}'</td><td>Используя POST и команду curl, создайте нового пользователя<br> на https://petstore.swagger.io/</td></tr>
  </table>