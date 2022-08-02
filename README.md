-
.0# AgileCatBot.
.0

Telegram бот для кросс-ревью команд разработчиков 

## Что такое Agile Cat Bot?

Это программа, которая будет мониторить ваш Telegram чат и привлекать ревьюверов с других команд в общем чате разработки.
Программа позволяет не искать себе второго ревьювера по ЛС-ам, а с помощью простой команды делает это за вас.

## Преимущества
 - Открытый код :3
 - Шифрование всех важных данных (алгоритм 'aes-256-cbc'). Названия команд, id пользователей, чатов, ники в телеграм и другая информация надежно защищена.
 - Легкий и быстрый. Используется node-js + postgres

## Как использовать бота?

🔥🔥🔥 ВАЖНО 🔥🔥🔥

В связи с политикой безопасности Telegram, боты не умеют первыми писать пользователю. 
Данный бот очень тесно взаимодействует с ЛС пользователей, отправляя уведомления о действиях пользователя (запись удалена, обновлена и т.д.).

Поэтому, для работы с ботом необходимо проинициализировать ваш диалог с ним. Зайти в ЛС бота 
(@AgileCatBot) и нажмите кнопку "Запустить". Бот ответит вам, что его ЛС только для уведомлений, это нормально.
После этой процедуры вы сможете пользоваться ботом.

После инициализации бота в ЛС, если вы не являетесь администратором группы, начинайте с п. 4

1. Добавьте бота в желаемую группу и назначьте администратором. Бот должен уметь читать, удалять, изменять сообщения, но лучше назначить ему все права.

2. Запустите бота, он попросит у вас ключ активации. Получить ключ можно у @progryx. Введите ключ активации, бот напишет вам в ЛС, что он готов к работе или что ключ введен неверно.
В таком случае напишите мне же (@progryx), будем разбираться.

3. После активации (делается администратором группы), администратор должен создать желаемые команды разработчиков. Перейдите в настройки команд (Главное меню - Выбрать команду - Добавить команду) и добавьте столько команд, сколько требуется.
После создания команд разработки, выберите созданную команду, нажав по ее названию. После этого, все участники чата могут выбрать свою команду.

4. Выберите вашу команду в чате, чтобы бот понимал, кого тегать. (Главное меню - Выбрать команду - *Название команды*)

## Возможности бота

1. Если вы хотите, чтобы ваш ПР отревьювили ДВА человека:
    - напишите в чат: !https://ССЫЛКА_НА_ПР
    - выберите в меню или в списке команд команду /review.
    Бот распознает ее, и напишет вам сообщение, на которое вы должны ответить, прислав ссылку на ПР без модификаций (Пример: https://test.ru)
    
2. Если вы хотите, чтобы вас отревьювил еще один человек, введите команду /change и точно так же в реплай (ответ) бота вставьте ссылку на ПР без модификаций

3. Если вы хотите, чтобы вас отревьювила определенная команда разработки, выберите пункт меню "Ревью определенной командой". На ваш ПР тегнется вся выбранная команда.

4. Если вы хотите посмотреть информацию о себе или о какой-либо команде разработки, запустите команду /info и выберите соответствующий пункт.

5. Когда вы уходите в отпуск, запустите бота и выберите в меню "Режим отпуска". Бот не будет вас упоминать в течении одной недели. После этого срока бот автоматически добавляет вас обратно в выборку по ревьюверам.
Также режим можно отключить вручную, выбрав соответствующий пункт в главном меню.

## FAQ по устранению ошибок:
- Если у вас не получается выбрать команду, причина может быть в том, что вы не проинициализировали бота у него в ЛС.
Боты устроены таким образом, что не могут без вашего согласия отправлять вам сообщения. Поэтому нужно зайти в ЛС бота и нажать кнопку "Запуск"
