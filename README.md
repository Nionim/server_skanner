# server_skanner--tvomel
Сканер майнкрафт серверов, для поиска существующих серверов по ноде/айпи и тд

## Принцип работы:
(ЭТОТ ЛИСТ ПРИМЕРНЫЙ! Я НЕ БУДУ ОПИСЫВАТЬ ВООБЩЕ ВСЁ! СКАЧАЙТЕ И САМИ УЗНАЙТЕ ПРИНЦИП РАБОТЫ!)
1) Ввод айпи/домена
   Если домен - он через несколько пунктов переводится в айпи
   Если айпи - продолжаем работу
2) Ввод информацию о том, что это.
   Домен? - переводим в айпи
   Айпи? - работаем дальше
3) С какого по какой порты сканировать?
   пример 20000 to 25565
4) Начало сканирования
   Сервер существует? - Получаем две строки его MOTD
   Сервер не существует? - Идем дальше и пропускаем его
5) Запись результатов в txt файл, для дальнейшего использования.
   IP:PORT
   MOTD1:
   MOTD2:
6) Завершение работы и сохранение txt файла

### Что готово?
- [ ] GUI (Возможно будет реализовано через дискорд бота (токен вставите сами))
   - [X] Интуитивно понятный "интерфейс" в консоли
- [X] Автоматический перевод домена в ip
   - [ ] Фикс ошибки из-за которой не воспринимаются некоторые домены (Очень редкая ошибка, но есть с **некоторыми** доменами)
- [ ] Поддержка прокси
   - [ ] Получение прокси в автоматическом режиме
- [X] Сканирование
   - [X] "Удобный" текст в консоли 
- [X] Запись в txt
   - [ ] Соответствующая подпись, если сервер не имеет MOTD - "Velocity or Bungee" - Это связано с тем, что многие такие сервера действительно являются Velocity/Bungeecord - Это значит, что на них нельзя зайти и как либо полезно с ними взаимодействовать. (Пока не делаю, тк не нада)


### Описание релизов:
V1.0: Создан первый прототип сканера
      Из функционала:
      1) Переводит домен в айпи и говорит вам его
      2) Есть выбор портов для скана (Пишите сами)
      3) Подсветка найденых серверов
      4) Запись найденых серверов в соответствующие файлы .txt (Где приписка "NONE" - Сервер скорее всего не работает)
      5) За 1 секунду сканит примерно 4-5 серверов (Это очень примерно, там скорее сильно больше)
   В целом нормальный релиз.

V2.0: Немного переписан код скана:
      1) Добавлен файл logos.py (Для будущего удобства)
      2) Улучшена читабельность кода
      3) На этот раз не удалял свои комментарии и даже их дополнил
   Отличие в основном внутри самого кода, но так же добавлено более красивое оформление в консоли
   (В планах сделать интерфейс через дискорд бота, где его токен вы будете вписывать сами, без риска его потерять (Код же будет лежать тут :)  ))

