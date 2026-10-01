Этап 1.1: Основы x64 и эксплуатация (4 месяца)
Ресурс: Курс "Practical Binary Analysis" или тим-курсы от RET2 Systems.
Задание: Прорешать все лабы по pwn с сайта pwnable.tw или pwnable.xyz, начиная с простых. Написать сплоиты на Python+pwntools для переполнения буфера, форматных строк, use-after-free.
Цель: Научиться писать ROP-цепочки для обхода NX, обходить ASLR с утечкой.
Этап 1.2: Windows Kernel Exploitation (4 месяца)
Ресурс: Курс "Windows Kernel Exploitation" от Corelan или Advanced Windows Exploitation от OffSec (OSED).
Задание: Разработать сплоит для уязвимости в драйвере HEVD (HackSys Extreme Vulnerable Driver). Пройти путь от IOCTL фаззинга до LPE.
Этап 1.3: Разработка вредоносного ПО и C2 (4 месяца)
Задача: Написать свой асинхронный C2 на Go с HTTP/HTTPS-транспортом, шифрованием RC4, поддержкой команд (шелл, загрузка/скачивание файлов). Имплементировать техники обхода EDR: unhooking ntdll.dll, indirect syscalls, обход ETW.
Проверка: Протестировать свой C2 в лабе с Defender и Sysmon, убедиться, что логи минимальны.
