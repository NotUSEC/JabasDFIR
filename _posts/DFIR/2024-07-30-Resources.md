---
layout: post
title: Полезные ссылки
permalink: _posts/DFIR/resources
---

# DFIR notes
Список полезных сайтов, видосов, форумов
{% for note in site.dfir-notes %}* [{{note.title}}]({{note.url}})
{% endfor %}

# Полезные сервисы
* [MITRE ATT&CK](https://attack.mitre.org/matrices/enterprise/) - Матрица угроз.
* [The DFIR report](https://thedfirreport.com) - Сайт с кучей информации по DFIR. В основном описание техник и тактик злоумышленников.
* [RegExr](https://regexr.com) - Сервис для написания и тестирования регулярных выражений.
* [Cyber Chef](https://gchq.github.io/CyberChef/) - Сервис с возможность кодирования, декодирования, шифрования и расшифрованиния информации. Есть режим обработки зашифрованной информации при помощи ИИ, которая в ~20% случае выдаёт верный вариант расшифровки. Так же можно установить локально на своё устройство, для возможности работы без подключения к интернету.
* [hexed.it](https://hexed.it) - Online-HEX редактор.
* [NoMoreRansom](www.nomoreransom.org/ru/decryption-tools.html) - Сборник дешифраторов от различной рансомвари.
* [Malware Traffic Analysis](https://www.malware-traffic-analysis.net) - Сервис с образцами вредоносной активности в формате **.pcap**. Подойдёт и для обучения, и для составления собственных правил к IDPS.
* [unprotect.it](https://unprotect.it) - Сайт с описанием актуальных угроз. Содержит и PoC для Red-Team, и IoC для Blue-Team.
* [lolbas-project](lolbas-project.github.io) - Содержит в себе список легитимных утилит Windows, и потенциальные методы их эксплуатаци. Полезно в целях ограничения запуска каких-либо из указанных служб/утилит, исходя из рисков.

# Песочницы
* [Any.Run](https://app.any.run) - Песочница с динамическим и статическим анализом. Позволяет взаимодействовать с виртуальным окружением.
* [Virustotal](https://www.virustotal.com/gui/home/upload) - По большей части статический анализ, но есть и раздел с песочницами которые иногда всё таки работают.
* [Hybrid analysis](https://www.hybrid-analysis.com), [Sandboxie](https://github.com/sandboxie-plus/Sandboxie) - Песочницы с динамическим и статическим анализом, сам не пользовался.
* [tria.ge](https://tria.ge) - Песочница с динамическим и статическим анализом, требуется регистрация для взаимодействия. Сам не пользовался, по отзывам работает так же эффективно как и any.run (местами лучше)
* [Windows Sandbox](https://learn.microsoft.com/ru-ru/windows/security/application-security/application-isolation/windows-sandbox/windows-sandbox-overview) - встроенный модуль Windows, который необходимо догрузить. Позволяет быстро развернуть пустую ВМ Windows, в которой можно анализировать файлы как угодно. Есть возможность создания шаблона, чтобы сразу было предустановлено необходимое ПО. Из минусов - при выходе ВПО за пределы виртуализации, вред будет нанесён хост-машине.
* [DRAKVUF](https://github.com/tklengyel/drakvuf), [DRAKVUF SandBox](https://github.com/CERT-Polska/drakvuf-sandbox), [DRAKVUF плагины](https://habr.com/ru/companies/pt/articles/566698/) - Opensource-песочница, устанавливается как утилита на Linux-машине. Может эмулировать и Windows и Linux окружения. Доступ к управлению через веб-интерфейс, и не позволяет взаимодействовать с виртуальным окружением.
* [PT SandBox](https://www.ptsecurity.com/ru-ru/products/sandbox/) и [Kaspersky SandBox](https://support.kaspersky.com/KSB/2.0/ru-RU/223822.htm) - Корпоративные песочницы, для автоматического анализа на потоке, при помощи статических и динамических методов анализа.

# Форумы в клирнете
* [РУ Сфера](ru-sfera.pw/forums) - ИБ-форум
* [RTFM Wiki](rtfm.wiki/security/opennet_security_top) - Список безопасных и не безопасных утилит под Linux. По сути Wiki, но почему бы ему здесь и не быть.



# Методички
* [KAPE Presentation](https://docs.google.com/presentation/d/1su_DDs71_ZUzTdI7oRx_DcxNE608Ia2A2Qo6sITqIFI/edit?usp=sharing) - Презентации по KAPE
* [Home Lab Presentation](https://docs.google.com/presentation/d/1NKSB0CqVIPa-RxK0DOfrdyoU3F016baJBhjrx49ZbO8/edit?usp=sharing) - Презентации для домашней Forensic-лаборатории
* [SANS Posters](https://www.sans.org/security-resources/posters/) - Постеры и cheat-sheet по DFIR и не только
* [NetSecNinja](netsecninja.github.io/tools/) - Содержит список ссылок на другие утилиты и сервисы, некоторые из которых недоступны из РФ или уже устарели.
* [Secrity Certification Roadmap](https://pauljerimy.com/security-certification-roadmap/) - Схема сертификации по различным ИБ-направлениям. Периодчески обновляется
* [Red Team Resources by C0UNT1NGST4RS](https://github.com/C0UNT1NGST4RS/RedTeam-Resources) - Список с ресурсами побольше ¯\_(ツ)_/¯
