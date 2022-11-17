			XML


 21. Создать внешний репозиторий c названием XML.

https://github.com/VladimirD25/XML.git

 22. Клонировать репозиторий XML на локальный компьютер.

VladimirDobranitsa@Vladimir MINGW64 /d/github
$ git clone https://github.com/VladimirD25/XML.git
Cloning into 'XML'...
warning: You appear to have cloned an empty repository.

 23. Внутри локального XML создать файл “new.xml”.

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ touch new.xml

 24. Добавить файл под гит.

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ git add new.xml

 25. Закоммитить файл.

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ git commit -m "add new.xml"
[main (root-commit) e71a181] add new.xml
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.xml

 26. Отправить файл на внешний GitHub репозиторий.

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 218 bytes | 218.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/VladimirD25/XML.git
 * [new branch]      main -> main

 27. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
 
VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ vim new.xml

<about_me>
<first_name>Vladimir</first_name>
<second_name>Olegovich</second_name>
<last_name>Dobranitsa</last_name>
<age>35</age>
<pets>none</pets>
<future_salary>$400</future_salary>
</about_me>

 28. Отправить изменения на внешний репозиторий.

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ git commit -am "modify new.xml"
warning: in the working copy of 'new.xml', LF will be replaced by CRLF the next
time Git touches it
[main 312d42d] modify new.xml
 1 file changed, 8 insertions(+)

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 375 bytes | 375.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/VladimirD25/XML.git
   e71a181..312d42d  main -> main

 29. Создать файл preferences.xml

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ touch preferences.xml

 30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
 
VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ vim preferences.xml

<preferences>
<favorite_movie>movies_by_Guy_Ritchie</favorite_movie>
<favorite_tv_show>Billions</favorite_tv_show>
<favorite_dish>cannelloni</favorite_dish>
<favorite_season>spring</favorite_season>
<country_to_visit>Norway</country_to_visit>
</preferences>

 31. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
 
VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ cat > skills.xml
<courses_skills>
<skills>Basic theory SDLC, STLC.
        Client-server architecture.
        HTTP.
        What is JSON, XML.
        API testing via Postman (JS, API autotests).
        Removing and reading logs from an external server.
        Sniffing http web traffic via Charles and Fiddler.
        Dev Tools of web browsers.
        Mobile testing.
        Feature iOS, Android, guidelines.
        ADB (android device management).
        Setting up proxy and vpn on iOS and Android.
        Interception (sniffing) of mobile traffic via Charles and Fiddler on iOS and Android.
        Command line (terminal) Linux.
        Basics of bash scripting, automation of routine tasks on the server.
        Access to remote servers.
        SQL basics.
        Load testing in Jmeter.
        Scrum development methodology.
        Python. Basic learning.
</skills>
</courses_skills>

 32. Сделать коммит в одну строку.

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ git commit -m "add preferences.xml skills.xml"
[main 18b3258] add preferences.xml skills.xml
 2 files changed, 29 insertions(+)
 create mode 100644 preferences.xml
 create mode 100644 skills.xml

 33. Отправить сразу 2 файла на внешний репозиторий.

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 906 bytes | 453.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/VladimirD25/XML.git
   312d42d..18b3258  main -> main

 34. На веб интерфейсе создать файл bug_report.xml.

https://github.com/VladimirD25/XML/blob/main/bug_report.xml

 35. Сделать Commit changes (сохранить) изменения на веб интерфейсе.

add bug_report.xml

 36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.

<bug_report> 
<id>B1</id>
<summary>Incomplete digits displaying of the number of items in the cart when entering a three-digit value</summary>
<preconditions>site is opened. 
               any item added to cart. 
               cart is opened.</preconditions>
<steps_to_reproduce>1) enter '99' in the number of units of goods, press 'Enter'. 
                    2) click on '+' button.</steps_to_reproduce>

<expected_result>Full displaying of digits for the number of items in the cart</expected_result>
<actual_result>the digits of the number of items in the cart are not displayed completely</actual_result>
<severity>minor</severity>
<priority>low</priority>
<environment>windows 10 Chrome 107.0.5304.88</environment>
<attachment>link</attachment>
<reporter>Vladimir</reporter>
</bug_report>

 37. Сделать Commit changes (сохранить) изменения на веб интерфейсе.

modify bug_report.xml

 38. Синхронизировать внешний и локальный репозиторий XML

VladimirDobranitsa@Vladimir MINGW64 /d/github/xml (main)
$ git pull
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 1.71 KiB | 72.00 KiB/s, done.
From https://github.com/VladimirD25/XML
   18b3258..acf9a2f  main       -> origin/main
Updating 18b3258..acf9a2f
Fast-forward
 bug_report.xml | 18 ++++++++++++++++++
 1 file changed, 18 insertions(+)
 create mode 100644 bug_report.xml


