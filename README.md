# XML
GIT Homework 1
Все шаги сценария выполняйте в терминале GitBush, Terminal, в папке под гитом.

 1. Создать внешний репозиторий c названием XML.
 
        В веб интерфейсе github: create new repository XML --public
 
 2. Клонировать репозиторий XML на локальный компьютер.
 
        $ git clone git@github.com:mariiaAks/XML.git
 
 3. Внутри локального XML создать файл “new.xml”.
 
        $ cd XML
        $ touch new.xml
 
 4. Добавить файл под гит.
 
        $ git add new.xml
 
 5. Закоммитить файл.
 
        $ git commit -m "Add new file new.xml"
 
 6. Отправить файл на внешний GitHub репозиторий.
 
        $ git push 
 
 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
 
        $ vim new.xml
        INSERT (кнопка i)
 
        <?xml version="1.0" encoding="UTF-8"?>
        <personalInfo>
          <firstName>Мария</firstName>
	        <middleName>Романовна</middleName>
	        <lastName>Щербатова</lastName>
	        <age>38</age>
	        <amountPets>0</amountPets>
	        <futureSalary>100000</futureSalary>
        </personalInfo>
 
        Esc :wq 
 
 8. Отправить изменения на внешний репозиторий.
 
        $ git add new.xml
        $ git commit -m "Change file new.xml: add personalInfo"
        $ git push
 
 9. Создать файл preferences.xml
 
        $ touch preferences.xml
 
 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
 
    $ vim preferences.xml
    INSERT (кнопка i)
 
    <?xml version="1.0" encoding="UTF-8"?>
    <preferences>
        <favoriteMovie>Летят журавли</favoriteMovie>
	      <favoriteTVSeries>Склифосовский</favoriteTVSeries>
	      <favoriteFood>Солянка</favoriteFood>
	      <favoriteSeason>Лето</favoriteSeason>
	      <travelCountry>Дания</travelCountry>
    </preferences>

    Esc :wq 
 
 11. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
  
    $ cat > sklls.xml
  
      <?xml version="1.0" encoding="UTF-8"?>
      <skills>
          <theory>что такое тестирование, багрепорты, документация, виды, методы, направления тестирования</theory>
	        <architecture>клиент-серверная архитектура, структура http запросов и ответов</architecture>
	        <API testing>Тестирование API через Postman</API testing>
	        <web testing>DevTools браузеров, снифинг web трафика через Charles и Fiddler</web testing>
	        <mobile testing>Android studio, перехват мобильного через Charles и Fiddler</mobile testing>
	         <database>Установка и настройка БД Postgres, основы SQL</database>
      </skills>
 
    Ctrl+C
 
 12. Сделать коммит в одну строку.
 
    $ git add preferences.xml sklls.xml && git commit -m "Add 2 files preferences.xml sklls.xml"

 13. Отправить сразу 2 файла на внешний репозиторий.
 
    $ git push
 
 14. На веб интерфейсе создать файл bug_report.xml.
 
    Add file - Create new file - Commit new file
 
 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 
    Commit changes
 
 16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
 
    Edit file bug_report.xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <bugreport>
	      <bug_id>1</bug_id>
	      <title>Dash line not visible on widget</title>
	      <severity>major</severity>
	      <priority>high</priority>
	      <summary></summary>
	      <preconditions>
		        <precondition>Clear screen</precondition>
	      </preconditions>
	      <stepToReproduce>
		        <step>Add several widgets</step>
		        <step>Change size some widgets</step>
	      </stepToReproduce>
	      <environments>
		        <environment>Redmi Note 7 MIUI 12.5.1.0 android 10 QKQ1.190910.002</environment>
		        <environment>Honor 20 pro (YAL-L41), Android 10</environment>
	      </environments>
	      <expectedResult>"Widgets have a dotted line on all 4 sides</expectedResult>
	      <actualResult>Widgets don't have dotted lines</actualResult>
	      <attachments></attachments>
        </bugreport>

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 
    Commit changes
 
 18. Синхронизировать внешний и локальный репозиторий XML
  
    $ git pull
