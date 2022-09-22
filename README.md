# hr_analytics_sql
# Analysis of employers database and possible relations between data about them and their work-performance
For Russian scroll down. 
### The task
Several tables with data about employers in a company are located in a server. I need to retrive this data and analyse it using sql only through sqlalchemy and pandas. And then prepare some recomendations for hr-department of a company. 
### What tools have been used?
<br> sql
<br>sqlalchemy
<br>matplolib
vpandas 
### Observations made
1. Men of any age have been working for company in average for 4-5 years. 
2. Women have the lowest amount of years employed by the age of 30 and after 45 their experience start to rise. 
<br>Some managers were determined whose staff show low efficiency at work. 
<br>Employers with the lowest salaries are often quit because of money issues, change of professions or general sense of unhappiness. 
* There are head-hunting resources that should be abandoned due to their high cost and low efficiency. 
<br><br>
# Анализ базы сотрудников компании и возможных корреляций между различными характерстиками сотрудников. 
### Задача 
На основе таблиц в базе данных, в которых содержится информация о сотрудниках, подготовить рекомендации для отдела кадров. 
### Какие иснтрументы использовались? 
<br>sql
<br>sqlalchemy
<br>matplolib
<br>pandas 
### Общие рекомендации.

<br><br> ВЛИЯЕТ ЛИ СЕМЕНОЕ ПОЛОЖЕНИЕ НА ЛОЯЛЬНОСТЬ? В целом меньше всего отрабатывают люди в семейном статусе 4, при чем женщины. Дольше всего отрабатывают в семейном статусе 3, причем мужчины. В статусах 1 и 0 отрабатывают примерно средне, как мужчины, так и женщины. 
<br><br> ЕСТЬ ЛИ ЗАВИСИМОСТЬ МЕЖДУ ВОЗРАСТОМ, ПОЛОМ И ВРЕМЕНЕМ ОТРАБОТКИ? В целом вижу тенденцию, что мужчины, в среднем, остаются на работе примерно одинаковое количество времени вне зависимости от возраста - примерно чуть больше 4 лет. У женщнин есть явный спад количества дней отработки к 30 годам. Может быть, связано с тем, что к 30 женщины уходят в декрет? И возвращаются где-то в 33-35, потому что к 40 годам они работают в компании уже около 5 лет? И потом срок стажа растет, к 50 годам.
<br><br> ЕСТЬ ЛИ ЗАВИСИМОСТЬ ВРЕМЕНИ ОТРАБОТКИ ОТ МЕНЕДЖЕРА? Нужно обратить внимание на менеджеров Ketsia Liebig & Janet King, у них какие-то очень высокие показатели увольнений за проступки. Eric Dougall, Lynn Daneault, Amy Dunn, Debra Houlihan каждутся приличными менеджерами, у них нет увольнений по причине. Brannon Miller имеет какие-то очень высокие показатели по увольнению из-за непосещения. Почему?
<br><br> ЗАВИСИМОСТИ МЕЖДУ ПРИЧИНАМИ УВОЛЬНЕНИЙ, КОЛИЧЕСТВОМ УВОЛЬНЕНИЙ И УРОВНЕМ ЗП. Интересно, что больше всего увольнений в диапазоне зарплат до 27 долларов в час, что не самая высокая зарплата, иными словами, следующая после зарплат явно молодых людей (тех, кто ушел учиться или в армию). При этом причины увольнения - деньги, перевод на другую должность (возможно, где больше платят), а также отсутствие удовлетворенности (возможно, потому что мало платят). Может быть, стоит пересмотреть зарплаты? Похоже, стоит обратить на должность Production Technician - меньше всего платят им, и именно оттуда бегут из-за недостаточности оплаты, перевода на другую должность или общего неблагополучия. Зарплаты там вообще до 20 долларов в час.
<br><br> С КАКИХ РЕСУРСОВ ПРИХОДИТ БОЛЬШЕ ТЕХ СОТРУДНИКОВ, КОТОРЫЕ ОСТАЮТСЯ РАБОТАТЬ НА ПОДОЛЬШЕ? Определенно стоит пересмотреть сотрудничество с MBTA ads - на них много расходов, а сотрудники оттуда в среднем работают не так много, как хотелось бы, да и набрать удалось не то, чтобы самое большое количество людей по сравнению с другими ресурсами, и обратить внимание на Pay Per Click - Google, Search Engine - Google Bing Yahoo, Professional Society- расходы не самые высокие, однако удалось набрать оттуда достаточно много сотрудников с нормальной лояльностью. Также стоит взглянуть на Employee Referral - затрат ноль, набрано много сотрудников, но лояльность не самая высокая. Определенно стоит отказаться от Careerbuilder, Pay Per Click - они стоят денег, а удалось набрать всего по 1 человеку с каждого ресурса.
