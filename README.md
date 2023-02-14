# [Список вопросов](#6.-Список-ответов)
##  [1. Сети](#1.-Сети)
### [1.1. Модель OSI](#1.1%20Модель%20OSI)
#### [1.1.1 Перечисли уровни модели OSI?](#1.2.1%20Перечисли%20уровни%20модели%20OSI?)
#### [1.1.2 Какие протоколы на каких уровнях?](#1.2.2%20Какие%20протоколы%20на%20каких%20уровнях?)
#### [1.1.3 Какие приложения работают на каких уровнях, примеры?](#1.2.3%20Какие%20приложения%20работают%20на%20каких%20уровнях,%20примеры?)

### 1.2 TCP UDP ICMP BGP NAT DHCP netplan nmcli
1.2.1 почему где то udp, где-то tcp используют
1.2.2 почему вместо udp не пользовать tcp
1.2.3 флаги tcp
- В чем отличие tcp/udp?
1.2.4 установка соединения (кто кому как зачем и почему шлет какие пакеты), как происходит разрыв соединения
1.2.5 протокол ip
1.2.6 протокол icmp
1.2.7 размер пакета пинга
- Основные отличия ipv4 от ipv6*
- Что такое CIDR?
- Для чего нужна маска подсети?
- Какое максимальное и минимальное количество ip адресов возможно в подсети?
	- перечислить для каждой маски  общее количество IP и реальное (на что могут быть зарезервированы и сколько)
	- как вычисляется количество IP в той или иной подсети?
	- как вычисляется маска подсети?
	- Максимальная и минимальная маска?
	- Сколько адересов в какой маске, как посчитать?
- чем проверять доступность портов
- Вот если бы была возможность заново переизобрести интернет, то какой транспортный протокол ты бы выбрал?
- На какой порт стучит icmp?
- Описать 3-way handshake 
- TCP (в т.ч. Handshake), UDP, IP, ICMP, DNS, NAT, IPv6 vs IPv4, SLAAC, DHCP, HTTP, HTTPS
- Что такое NAT и для чего нужен?
- Как работает NAT в облаке?
- Что такое DHCP? Как он работает? И что он вещает?
- Перечислить сетевые уровни? (тоже самое, что и про OSI - уровни модели OSI)
- На каком сетевом уровне работает ping?
- Как работает ping?
- Что такое mtu и mss?
- Для чего используются и mss?
- Как задать mss?*
- Сеть как настроить?
- Шлюз по-умолчанию и next hop?
- Уникален ли IP-адрес?
  

### 1.3 WWW:
- в чем разница между http и https?
- что такое протокол http?
- какой уровень OSI http?
- как работает http?
- какие есть версии?
- чем разница между http1.0 1.1 2.0?
- Какие бывают коды ответ HTTP? По группам и основноые из каждой.
- Как посмотреть заголовки?

### 1.4 SSL сертификаты:
- что внутри?
- как происходит шифрование?
- установка https сессии?
- где взять серт?
- Для чего SSL сертификат? 
- Какие бывают
- Как сгенерировать?
- Расскажи о SSL/TLS handshake? Как это работает?

### 1.5 SSH
#### [1.5.1 На каком порту работает SSH демон?](#1.5.1%20На%20каком%20порту%20работает%20SSH%20демон?)
#### [1.5.2 Если SSH порт менялся и мы не знаем его номер, то как это можно узнать?](#1.5.2%20Если%20SSH%20порт%20менялся%20и%20мы%20не%20знаем%20его%20номер,%20то%20как%20это%20можно%20узнать?)
[1.5.3 Какие бывают варианты аутентификации по SSH?](#1.5.3%20Какие%20бывают%20варианты%20аутентификации%20по%20SSH?)
- Какие ключи используются для аутентификации на сервере по SSH?
- Как проверить соответствие закрытого SSH ключа открытому
- Как работает SSH-аутентификация пользователя посредством пары ключей?
- Знаком ли ты с X11 Forwarding?


## 3. ОС Linux

### 3.1 Линукс:
- что такое pid?
- что за процесс с pid 1, что делает
- права доступа
- load average
- чем мониторить цпу, озу, диски
- системные вызовы
- ссылки
- чем посмотреть переменные среды
- Какой командой посмотреть версию ядра?
- Как скопировать файлы с одного сервера на другой
- Как узнать релиз дистрибутива на сервере?


### 3.2 Диски и ФС
- что происходит от включения компа и до загрузки системы --> gpt/mbr?
- как подключить диск и начать с ним работать (разбивка/создание фс/и тд)?
- Как примонтировать диск?
- Что такое inode, как это работает?
- Что такое симлинк?
- Что такое жесткая ссылка, как работает
- Что такое gpt ?
- Что такое mbr? 
- "Представь, что тебе нужно создать файл, но ты не можешь (Связано с inode'ами), почему, как диагностировать, как решить?
- Права - owner, group, anybody. Как их подсчитать и как назначить?
- Разобраться как запускается сервер на линуксе:
	- MBR/GPT
	- BIOS
	- POST
	- GRUB
	- Init
	- initramfs 
	- SystemD
	- udev
- Как проверить свободное пространство на диске?
- Как узнать сколько весит файл или папка?
- Как увеличили диск? Как расширить раздел диска на ВМ? Последовательность команд.
- Ошибка: Out of inodes (ext)?
- Что такое Sticky bit? Как с ним работать?
- Что такое setuid / setgid? Как с ними работать?


### 3.2 Процессы
- Какие бывают
- Как с ними работать
- Как посмотреть
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
- Потоки ввода вывода
- Как проверить нагрузку на процессор? Что означает load average?
- Как остановить процессы ?
- Что такое oom и как работает?
- Статусы процессов?
- Какие syscall знаешь?


### Файловая система и память
- Какие бывают файловые системы?
- tmpfs
- procfs (/proc)
- sysfs (/sys)
- разделы
- структура файловой системы линукса
- Что такое swap?
- виртуальная память
- анонимная память
- общая память
- аллокация памяти
- страницы памяти
- виды файлов
- символические и жесткие ссылки
- рейды (1, 0, 5, 10)
- файловые дескрипторы
- перенаправление 2>&1
- - Структура файловой системы ОС Linux?
- Где хранятся файлы настроек сетевых соединений?
- Где хранятся устройства в файловой системе?
- Для чего требуется /dev/null?
- Как примонтировать папку или раздел
- Какие бывают права доступа?
- Какие бывают ссылки в Linux?
- Что такое inode?
- Что означают права доступа на файл 0644?
- В чем разница между /bin,/sbin,/usr/bin,/usr/sbin?
- В чем разница между ext2, ext3, ext4?
- Расскажи о xfs?
- Расскажи о btrfs?
- Расскажи о nfs?
- Расскажи о virtiofs? Зачем? Как работает в облаке? Как смонтировать? Сколько стоит? Сравни с s3 хранилищем.


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
- Как проверить опертивную память RAM
-  Как пососмотреть сетевые интерфейсы?
- Как посмотреть сетевые маршруты?
- Как проверить удаленную доступность хоста?
- Как проверить потери пакетов.
- Как включить режим отладки у консольных команд?
- Утилиты диагностики сетей?
- **58. Как работать с** 
	- tcpdump 
	- tcpshark
	- wireshark
- Поля утилит top/htop (см. LA)?
-  Как посмотреть переменные окружения?



### 5. Shell
- Изобрази цикл на bash?
`for i in {10..14}; do ping -c 3 10.10.10.$i;done`
- Изобрази вложенный цикл?
- Изобрази ветвления на bash?
- Как искать по истории команд?

### 6. Контейнеризация.
- Чем контейнеризация отличается от виртуализации?
- Какая ОС может быть в контейнере?
- Связаны ли хостовая ОС и в контейнере?
- На чем основана контейнеризация?
- Почему "один процесс - один контейнер" ?
- Как видны процессы на хосте и в контейнере? в контейнере pid 1 -> pid xxx на хосте. pid yyy на хосте а контейнере не виден.

## 6. DNS:
- Как проверить DNS записи домена?
-  Какие записи RR (resource records) бывает?
- как устроен
- что происходит по порядку после например ввода адреса в браузере?
- делегирование
- какие записи есть
- зачем прописывать адрес днс сервера 8.8.8.8,как он работает
- ptr запись
- утилиты
- Разница между записяси ANAME  CNAME DNAME?
- Что такое TTL? Какое бывате?
- Что такое SOA? Из чего состоит?
- Для чего и как работает CNAME?
- Что такое PTR запись? Как работает?
- Как делегировать домен?
- Что такое TTL в DNS? Какие бывают? Как работает?
- Как происхит разрешение доменны имён в общем виде при запросе адреса домена в браузере?

## 7.  Контейниризацию и ее суть. Как работает?
## 8. Что такое шардирование и как работает.
## 9. Что такое кубернейтес и как работает
## 10. Безопаность
- Настройка аудита для доступа к файлу и контроль логинов c помощью auditd
```
aulast 
aulastlog

cat /etc/audit/rules.d/audit.rules 
## First rule - delete all
-D

## Increase the buffers to survive stress events.
## Make this bigger for busy systems
-b 8192

## This determine how long to wait in burst of events
--backlog_wait_time 60000

## Set failure mode to syslog
-f 1

-a exit,always -S open -F loginuid=1000

-w /etc/group -p wa
-w /etc/passwd -p wa
-w /etc/shadow -p wa
-w /etc/sudoers -p wa

-w /etc/audit/ -p r
-w /etc/audit/rules.d/audit.rules -p -wa
-w /etc/dnf -p r
-w /etc/dnf/dnf.conf -p wa
```

## 11.  SQL: Что такое SQL, NoSQL, NewSQL и какая между ними разница.
## 12. 
###################################
# 6.  Список ответов
## 1. Сети
### 1.1.  Модель OSI
#### 1.1.1 Перечисли уровни модели OSI?
#### 1.1.2 Какие протоколы на каких уровнях?
#### 1.1.3 Какие приложения работают на каких уровнях, примеры?

### 1.2 TCP UDP ICMP BGP
- почему где то udp, где-то tcp используют

### 1.5 SSH
#### 1.5.1 На каком порту работает SSH демон?
**Ответ:**  22 по умолчанию, если не менялся.
#### 1.5.2 Если SSH порт менялся и мы не знаем его номер, то как это можно узнать?
**Ответ:** посканировать порты, например SSH.
#### 1.5.3 Какие бывают варианты аутентификации по SSH?
**Ответ:** 
- по ключу
- по паролю
#### 1.5.4 Какие ключи используются для аутентификации на сервере по SSH?
**Ответ:**
#### 1.5.5 Как проверить соответствие закрытого SSH ключа открытому
**Ответ:**
#### 1.5.6 Как работает SSH-аутентификация пользователя посредством пары ключей?
**Ответ:**
#### 1.5.7 Знаком ли ты с X11 Forwarding?
**Ответ:**
