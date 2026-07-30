
**Кроки:**
1. According to the lecture materials, install, configure, and start the Suricata IDS. 
2. Stop Suricata, add two custom rules based on the example in the presentation materials. It is 
recommended to modify the alert message text. 
3. Start Suricata, ensure that the additional rules are loaded, and test their functionality. 
4. Provide screenshots with a brief explanation for each step.




Запуск ssh сесії
![](pic1.png)

Активація та перевірка статусу сурікати
![](pic2.png)

Зміна конфігурації suricata.yaml
![](pic3.png)

Оновлення правил безпеки sudo suricata-update
![](pic4.png)

запуск та перегляд статистики

sudo tail /var/log/suricata/suricata.log

sudo tail -f /var/log/suricata/stats.log
![](pic5.png)

Тестування роботи командами

sudo tail -f /var/log/suricata/fast.log 

curl http://testmynids.org/uid/index.html
![](pic6.png)

Вивід "eve.json" з фільтром event_type=stats
![](pic7.png)

Вивід "eve.json" з фільтром event_type=alert
![](pic8.png)

Створення своїх правил local.rules
![](pic9.png)
![](pic10.png)

Тестуваня своїх правил
![](pic11.png)