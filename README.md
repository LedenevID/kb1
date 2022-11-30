# [[#^085e43| 1. Список вопросов]]

## 1. Сети:
### 1.1 модель OSI:
- какие уровни
- какие протоколы на уровнях
### 1.2 tcp / udp/icmp
- отличия между tcp и udp
- почему где то udp, где-то tcp используют
- почему вместо udp не пользовать tcp
- флаги tcp
- установка соединения (кто кому как зачем и почему шлет какие пакеты), как происходит разрыв соединения
- протокол ip
- протокол icmp
- размер пакета пинга
- чем проверять доступность портов
- Вот если бы была возможность заново переизобрести интернет, то какой транспортный протокол ты бы выбрал?
- На какой порт стучит icmp?
- Описать 3-way handshake 
- TCP (в т.ч. Handshake), UDP, IP, ICMP, DNS, NAT, IPv6 vs IPv4, SLAAC, DHCP, HTTP, HTTPS
  

## 2 WWW:
### 2.1 http/https:
- в чем разница
- что такое
- как работает
- какие есть версии


### 2.2 SSL сертификаты:
- что внутри
- как происходит шифрование
- установка https сессии
- где взять серт, какие есть?

## 3. ОС Linux

### 3.1 Линукс:
- что происходит от включения компа и до загрузки системы --> gpt/mbr?
- как подключить диск и начать с ним работать (разбивка/создание фс/и тд)
- что такое pid
- что за процесс с pid 1, что делает
- права доступа
- load average
- чем мониторить цпу, озу, диски
- системные вызовы
- ссылки
- чем посмотреть переменные среды


### 3.2 Диски
- Как примонтировать диск
- Что такое inode, как это работает
- Что такое симлинк
- Что такое жесткая ссылка, как работает
- что такое gpt 
- что такое mbr 
- "Представь, что тебе нужно создать файл, но ты не можешь? Связано с inode'ами"
- права - owner, group, anybody. Как их подсчитать и как назначить?
- Разобраться как запускается сервер на линуксе:
	- MBR/GPT
	- BIOS
	- POST
	- GRUB
	- Init
	- initramfs 
	- SystemD
	- udev

### 3.2 Процессы
- Какие бывают
- Как с ними работать
-  как посмотреть
- как убить
- какие сигналы можно отправить
- что такое сигналы
- таблица процессов
- жизненный цикл процесса
- зачем нужны зомби
- как убить зомби
- как создать демона
- как порождаются процессы
- межпроцессное взаимодействие
- nohup
- kill
- ps
- lsof
- strace
- системные вызовы

### Файловая система и память
- Какие бывают
- tmpfs
- procfs (/proc)
- sysfs (/sys)
- разделы
- структура файловой системы линукса
- виртуальная память
- анонимная память
- общая память
- аллокация памяти
- страницы памяти
- свап
- виды файлов
- символические и жесткие ссылки
- рейды (1, 0, 5, 10)
- файловые дескрипторы
- перенаправление 2>&1


## 4. Инструменты диагностики:
- top как работает, что и как можно посмотреть
- Как примонтировать диск
- что где посмотреть, какие команды, последовательность
- классика: как выйти из vi, что еще по vi.
- как посмотреть кто залогинен в системе
- примеры работы утилит, назначение и флаги:
	- ss 
	- ps
	- nc
	- dig

### Shell
- Цикл на bash
`for i in {10..14}; do ping -c 3 10.10.10.$i;done`
- скриптинг


## 6. DNS:
- как устроен
- что происходит по порядку после например ввода адреса в браузере?
- делегирование
- какие записи есть
- зачем прописывать адрес днс сервера 8.8.8.8,как он работает
- ptr запись
- утилиты

## 7.  Контейниризацию и ее суть. Как работает?
## 8. Что такое шардирование и как работает.
## 9. Что такое кубернейтес и как работает
10. SQL: Что такое SQL, NoSQL, NewSQL и какая между ними разница.
11. 
###################################
#  7. Список ответов:

^085e43

## 1. Сети
### 1.1 модель OSI
- Уровни модели OSI:
 какие протоколы на уровнях



В inode содержится нужная нам информация: список блоков файловой системы для искомого файла

Как найти номер inode для указанного файла?