# План: System Design + облачные сертификаты (26 недель)

**Цель:** удалённая работа с хорошей зарплатой в компании из EU, UK или US, либо релокация в EU или UK.
**Исходная точка:** опыт работы в Microsoft/.NET-стеке.
**Нагрузка:** будни (Д1–Д5) по 1–1,5 часа, Д6 (выходной) — 3 часа практики, Д7 — отдых или короткое повторение.

---

## 0. Что важно для этой цели

| Где вы работаете | Что проверяют при найме | Роль сертификата |
|---|---|---|
| Продуктовые компании в US и UK (удалённо) | Раунд System Design, кодинг, behavioral-интервью на английском | Небольшая: сертификат помогает пройти HR-фильтр, но не собеседование |
| Enterprise и консалтинг в EU и UK (много .NET и Azure) | Собеседование + «облачный опыт» | **Заметная**: AZ-305 и AWS SAA часто прямо указаны в вакансиях |
| Германия и DACH | То же + иногда архитектурные сертификаты | iSAQB CPSA-F даёт плюс (опционально) |
| Визы (EU Blue Card, UK Skilled Worker) | Оффер, диплом или опыт, зарплатный порог | Для визы сертификаты не нужны |

**Вывод:** основа успеха — навыки System Design и английский на собеседовании. Сертификаты — ускорители. Порядок в плане:

1. **Недели 1–8.** Фундамент распределённых систем и практика собеседований. Это главное.
2. **Недели 9–16.** Azure Solutions Architect Expert (AZ-104 → AZ-305). Самая быстрая победа благодаря вашему опыту, ценится в .NET-вакансиях в Европе.
3. **Недели 17–22.** AWS Solutions Architect Associate (SAA-C03). Самый востребованный облачный сертификат в US и UK.
4. **Недели 23–26.** Интенсив по собеседованиям и откликам. Откликаться можно начинать уже с 12-й недели.

> Коды экзаменов, цены (примерно $150–165) и требования меняются. Перед записью проверьте их на Microsoft Learn и на сайте AWS Certification.

---

## 1. Ресурсы

В плане по дням название ресурса ведёт сюда, к его полному описанию. Ссылка на тему в том же пункте открывает нужную главу, страницу или видео.

**Обозначения в плане:** 📖 книга · 🎬 видео или лекция · 📄 статья, документация, курс · 🧭 интерактив · 🧪 тест · 🛠 упражнение или лабораторная · 🧩 задача System Design · 🗣 собеседование или устная практика · 🎯 экзамен · 📬 отклики · ⏸ отдых

**🇷🇺 По-русски** в конце описания — русское издание, перевод или локализация, если они есть. Машинный перевод помечен. Без русской версии: видео и лекции (кроме HighLoad++), Hello Interview, всё по AWS (документация, Skill Builder, SAA-C03), а также экзамены AZ-104 и AZ-305 — они сдаются на английском.

### Книги
- <a id="r-ddia"></a>**📖 Designing Data-Intensive Applications (DDIA)** — Martin Kleppmann, O'Reilly, 1-е издание 2017. Главная книга по теории хранения данных, репликации, партиционированию, транзакциям и консенсусу. **Номера глав в плане даны по 1-му изданию.** Платная, около $40–60. Сайт книги: https://dataintensive.net/ · 🇷🇺 **По-русски:** 1-е издание: «Высоконагруженные приложения. Программирование, масштабирование, поддержка», Питер, 2018 — номера глав совпадают с планом: https://www.piter.com/collection/all/product/vysokonagruzhennye-prilozheniya-programmirovanie-masshtabirovanie-podderzhka-2 · 2-е издание на предзаказе, выход ожидается 15 октября 2026 (главы уже не совпадают): https://www.piter.com/collection/soon/product/vysokonagruzhennye-prilozheniya-programmirovanie-masshtabirovanie-podderzhka-2-e-izd-2
- <a id="r-xu"></a>**📖 System Design Interview, тома 1 и 2** — Alex Xu (том 2 с Sahn Lam). Разборы типовых задач собеседования со схемами: том 1 — 15 глав (от масштабирования до Google Drive), том 2 — 13 глав (геосервисы, платежи, мониторинг, бронирование). Платная: бумажная книга или онлайн-курс ByteByteGo с тем же текстом. Онлайн: https://bytebytego.com/courses/system-design-interview · 🇷🇺 **По-русски:** том 1 — «System Design. Подготовка к сложному интервью», Питер, 2022: https://www.piter.com/collection/programmirovanie-osnovy-i-algoritmy/product/system-design-podgotovka-k-slozhnomu-intervyu · том 2 — «System Design II. Распределенные системы. Подготовка к сложному интервью», Питер, 2026: https://www.piter.com/collection/top-2/product/system-design-ii-raspredelennye-sistemy-podgotovka-k-slozhnomu-intervyu

### Видео и лекции
- <a id="r-kleppmann"></a>**🎬 Martin Kleppmann — Distributed Systems (Cambridge)** — 8 лекций на YouTube по 40–60 минут + конспект в PDF. Лучшее бесплатное введение в теорию: модели систем, время и часы, broadcast, репликация, консенсус, консистентность, Spanner и совместное редактирование. Бесплатно. Плейлист: https://www.youtube.com/playlist?list=PLeKd45zvjcDFUEv_ohr_HdUFe97RItdiB · конспект: https://www.cl.cam.ac.uk/teaching/2122/ConcDisSys/dist-sys-notes.pdf
- <a id="r-mit"></a>**🎬 MIT 6.824 / 6.5840 Distributed Systems** — курс Robert Morris: лекции на YouTube, статьи (GFS, Raft, Spanner и др.) и лабораторные на Go. Бесплатно. Расписание со ссылками на лекции и статьи: https://pdos.csail.mit.edu/6.824/schedule.html
- <a id="r-harvard"></a>**🎬 Harvard CS75, лекция 9: Scalability** — David Malan, около 1 часа. Классическое введение в вертикальное и горизонтальное масштабирование, балансировку, кэш и репликацию. Бесплатно. https://www.youtube.com/watch?v=-W9F__D3oY4
- <a id="r-bytebytego"></a>**🎬 ByteByteGo (YouTube)** — Alex Xu. Короткие (5–10 мин) видео с наглядными анимированными схемами по отдельным темам. Бесплатно. https://www.youtube.com/@ByteByteGo
- <a id="r-nasser"></a>**🎬 Hussein Nasser (YouTube)** — бэкенд изнутри: базы данных, индексы, прокси, протоколы (HTTP/2, gRPC, WebSocket). Длинные подробные разборы. Бесплатно. https://www.youtube.com/@hnasr
- <a id="r-jordan"></a>**🎬 Jordan Has No Life (YouTube)** — глубокие разборы задач System Design и концепций распределённых систем, уровень senior. Бесплатно. https://www.youtube.com/@jordanhasnolife5163
- <a id="r-savill"></a>**🎬 John Savill's Technical Training (YouTube)** — лучшее бесплатное по Azure. **AZ-104 Study List** — плейлист «мастер-класса» по всем доменам экзамена: https://www.youtube.com/playlist?list=PLlVtbbG169nGlGPWs9xaLKT1KfwqREHbs · **AZ-305 Study Cram** — одно видео на несколько часов для повторения перед экзаменом: https://www.youtube.com/watch?v=vq9LuCM4YP4 · канал: https://www.youtube.com/@NTFAQGuy
- <a id="r-fcc"></a>**🎬 freeCodeCamp: AWS Solutions Architect Associate (SAA-C03)** — полный курс Andrew Brown (ExamPro), десятки часов с лабораторными. Бесплатно. https://www.youtube.com/watch?v=c3Cn4xYfxJY
- <a id="r-highload"></a>**🎬 HighLoad++ (YouTube, по-русски)** — доклады о реальной архитектуре высоконагруженных систем от инженеров российских и международных компаний. Бесплатно. https://www.youtube.com/@HighLoadChannel

### Статьи, документация, онлайн-курсы
- <a id="r-hello"></a>**📄 Hello Interview** — бесплатный фреймворк для собеседования (Delivery Framework), основные концепции, deep dives по технологиям и подробные разборы задач (bit.ly, Ticketmaster, WhatsApp и др.). Эталон для сверки своих решений. https://www.hellointerview.com/learn/system-design/in-a-hurry/introduction
- <a id="r-primer"></a>**📄 System Design Primer** — Donnie Martin, GitHub. Бесплатный справочник: подход к задаче, числа задержек, DNS, CDN, балансировщики, базы данных, кэш, асинхронность, плюс разобранные задачи. https://github.com/donnemartin/system-design-primer · 🇷🇺 **По-русски:** частично. Перевод первой половины на Habr («Букварь по дизайну систем», 2020): https://habr.com/ru/articles/501366/ · незаконченный README-ru в форке: https://github.com/voitau/system-design-primer/blob/master/README-ru.md
- <a id="r-papers"></a>**📄 Классические статьи** — по одной в месяц, затем разбор в лекциях [MIT 6.824](#r-mit). Бесплатно. [Dynamo (Amazon, 2007)](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf) · [Raft](https://raft.github.io/raft.pdf) · [Spanner (Google)](https://research.google/pubs/spanner-googles-globally-distributed-database-2/) · [Kafka (LinkedIn)](https://notes.stephenholiday.com/Kafka.pdf) · 🇷🇺 **По-русски:** переводов статей нет, есть русские разборы: [Raft (Dodo Engineering)](https://habr.com/ru/companies/dododev/articles/469999/) · [Spanner (Habr, 2013)](https://habr.com/ru/articles/207082/)
- <a id="r-azarch"></a>**📄 Azure Architecture Center** — эталонные архитектуры, деревья выбора сервисов и каталог Cloud Design Patterns (Saga, Retry, Circuit Breaker, CQRS и др.). Полезен и вне Azure. Бесплатно. https://learn.microsoft.com/azure/architecture/ · паттерны: https://learn.microsoft.com/azure/architecture/patterns/ · 🇷🇺 **По-русски:** машинный перевод Microsoft: https://learn.microsoft.com/ru-ru/azure/architecture/ · паттерны: https://learn.microsoft.com/ru-ru/azure/architecture/patterns/
- <a id="r-azwaf"></a>**📄 Azure Well-Architected Framework и Cloud Adoption Framework** — 5 столпов качества архитектуры (надёжность, безопасность, стоимость, эксплуатация, производительность) и landing zones для организаций. Бесплатно. https://learn.microsoft.com/azure/well-architected/ · https://learn.microsoft.com/azure/cloud-adoption-framework/ready/landing-zone/ · 🇷🇺 **По-русски:** машинный перевод Microsoft: https://learn.microsoft.com/ru-ru/azure/well-architected/ · https://learn.microsoft.com/ru-ru/azure/cloud-adoption-framework/ready/landing-zone/
- <a id="r-mslearn"></a>**📄 Microsoft Learn** — официальные бесплатные learning paths к AZ-104 и AZ-305, study guide с перечнем навыков и документация Azure. Study guide: [AZ-104](https://learn.microsoft.com/credentials/certifications/resources/study-guides/az-104) · [AZ-305](https://learn.microsoft.com/credentials/certifications/resources/study-guides/az-305) · 🇷🇺 **По-русски:** машинный перевод Microsoft, термины сверяйте с английским — экзамен на русском не сдаётся. Study guide: [AZ-104](https://learn.microsoft.com/ru-ru/credentials/certifications/resources/study-guides/az-104) · [AZ-305](https://learn.microsoft.com/ru-ru/credentials/certifications/resources/study-guides/az-305)
- <a id="r-dotnet"></a>**📄 Документация .NET и ASP.NET Core** — официальные статьи о gRPC, rate limiting и других частях платформы. Бесплатно. https://learn.microsoft.com/aspnet/core/ · 🇷🇺 **По-русски:** машинный перевод Microsoft: https://learn.microsoft.com/ru-ru/aspnet/core/
- <a id="r-awsdocs"></a>**📄 AWS Documentation** — официальные руководства по сервисам AWS. Для экзамена достаточно разделов «What is…» и «How it works». Бесплатно. https://docs.aws.amazon.com/
- <a id="r-awswa"></a>**📄 AWS Well-Architected Framework** — 6 столпов (у Azure 5 — добавлена устойчивость, sustainability) и whitepapers, в том числе о стратегиях DR. Бесплатно. https://aws.amazon.com/architecture/well-architected/
- <a id="r-skillbuilder"></a>**📄 AWS Skill Builder** — официальная платформа обучения AWS. Бесплатно: Exam Prep Standard Course к SAA-C03 и Official Practice Question Set (20 вопросов в формате экзамена). https://skillbuilder.aws/
- <a id="r-msio"></a>**📄 microservices.io** — Chris Richardson. Каталог паттернов микросервисов: Saga, Transactional Outbox, CQRS, декомпозиция. Бесплатно. https://microservices.io/patterns/ · 🇷🇺 **По-русски:** сайта на русском нет; книга Криса Ричардсона — «Микросервисы. Паттерны разработки и рефакторинга», Питер, 2019: https://www.piter.com/product/mikroservisy-patterny-razrabotki-i-refaktoringa
- <a id="r-techdocs"></a>**📄 Документация технологий** — PostgreSQL, Redis, Kafka, OpenTelemetry, MassTransit. Используется в упражнениях. Бесплатно. [PostgreSQL](https://www.postgresql.org/docs/current/) · [Redis](https://redis.io/docs/latest/) · [Kafka](https://kafka.apache.org/documentation/) · [OpenTelemetry](https://opentelemetry.io/docs/) · [MassTransit](https://masstransit.io/documentation/) · 🇷🇺 **По-русски:** документация PostgreSQL в переводе Postgres Professional (актуальная версия): https://postgrespro.ru/docs/postgresql/current/ · у Redis, Kafka, OpenTelemetry и MassTransit русской версии нет
- <a id="r-habr"></a>**📄 Habr (по-русски)** — хабы «Высокая производительность» и «Проектирование и рефакторинг»: статьи о реальной архитектуре. Бесплатно. https://habr.com/ru/hubs/hi/articles/ · https://habr.com/ru/hubs/refactoring/articles/

### Интерактив
- <a id="r-latency"></a>**🧭 Latency numbers (интерактив)** — Colin Scott. Числа задержек (кэш, RAM, SSD, сеть, межконтинентальный пинг) по годам. https://colin-scott.github.io/personal_website/research/interactive_latency.html
- <a id="r-raftviz"></a>**🧭 Визуализация Raft** — пошаговая анимация выбора лидера и репликации лога (The Secret Lives of Data) и интерактивный кластер на сайте Raft. http://thesecretlivesofdata.com/raft/ · https://raft.github.io/

### Тесты
- <a id="r-mspractice"></a>**🧪 Microsoft Practice Assessments** — бесплатные официальные пробные тесты на Microsoft Learn, примерно 50 вопросов, с пояснениями к ответам. Можно проходить многократно. [AZ-104](https://learn.microsoft.com/credentials/certifications/azure-administrator/practice/assessment?assessment-type=practice&assessmentId=21) · AZ-305: ссылка «Practice for the exam» на [странице сертификата](https://learn.microsoft.com/credentials/certifications/azure-solutions-architect/)
- <a id="r-examdemo"></a>**🧪 Microsoft Exam Sandbox** — демо интерфейса экзамена: типы вопросов, case studies, навигация. Бесплатно. https://aka.ms/examdemo
- <a id="r-measureup"></a>**🧪 MeasureUp** — официальный партнёр Microsoft по пробным экзаменам AZ-104 и AZ-305, близко к реальному формату. Платно. https://www.measureup.com/ · 🇷🇺 **По-русски:** есть машинный перевод тестов; полностью выверена только английская версия
- <a id="r-td"></a>**🧪 Tutorials Dojo — SAA-C03 Practice Exams** — Jon Bonso. Лучшие пробные тесты к AWS SAA: 6 полных тестов по 65 вопросов с подробными разборами. Платно, около $15–20. https://portal.tutorialsdojo.com/courses/aws-certified-solutions-architect-associate-practice-exams/

### Экзамены
- <a id="r-az104"></a>**🎯 AZ-104: Microsoft Azure Administrator** — сертификат Azure Administrator Associate; обязательный шаг к Solutions Architect Expert. Около 100 минут, 40–60 вопросов, проходной балл 700 из 1000. https://learn.microsoft.com/credentials/certifications/azure-administrator/
- <a id="r-az305"></a>**🎯 AZ-305: Designing Microsoft Azure Infrastructure Solutions** — вместе с AZ-104 даёт Azure Solutions Architect Expert. Есть case studies. Сертификат действует год, продление — бесплатный онлайн-тест. https://learn.microsoft.com/credentials/certifications/azure-solutions-architect/
- <a id="r-saa"></a>**🎯 AWS Certified Solutions Architect – Associate (SAA-C03)** — 130 минут, 65 вопросов, проходной балл 720 из 1000. Действует 3 года. https://aws.amazon.com/certification/certified-solutions-architect-associate/

### Пробные собеседования
- <a id="r-peer"></a>**🗣 Пробные собеседования с партнёром** — бесплатные peer-платформы (например, Exponent, бывший Pramp) и знакомые инженеры. Роли меняются: вы интервьюер, потом кандидат. https://www.tryexponent.com/practice
- <a id="r-paidmock"></a>**🗣 Платные пробные собеседования** — interviewing.io или Hello Interview: собеседование с инженером FAANG и подробный фидбек. Перед 23-й неделей, 1–2 штуки. https://interviewing.io/ · https://www.hellointerview.com/mock

### Инструменты и аккаунты
- <a id="r-excalidraw"></a>**🛠 Excalidraw** — бесплатная онлайн-доска для схем, популярна на собеседованиях. https://excalidraw.com · 🇷🇺 **По-русски:** интерфейс на русском
- <a id="r-azfree"></a>**🛠 Бесплатный аккаунт Azure** — стартовый кредит и бесплатные сервисы на 12 месяцев. Сразу настройте Budgets с алертами. https://azure.microsoft.com/free/ · калькулятор цен: https://azure.microsoft.com/pricing/calculator/ · 🇷🇺 **По-русски:** страницы на русском: https://azure.microsoft.com/ru-ru/free/ · https://azure.microsoft.com/ru-ru/pricing/calculator/
- <a id="r-awsfree"></a>**🛠 AWS Free Tier** — бесплатный аккаунт AWS для лабораторных. Сразу настройте Budgets с алертом. https://aws.amazon.com/free/
- <a id="r-anki"></a>**🛠 Anki** — бесплатные флеш-карточки с интервальным повторением. https://apps.ankiweb.net/ · 🇷🇺 **По-русски:** интерфейс на русском; руководство в переводе сообщества: https://andreykaiu.github.io/anki-manual-ru/
- <a id="r-leetcode"></a>**🛠 LeetCode / NeetCode** — задачи на кодинг для разминки; NeetCode даёт тематический список 150 задач. https://leetcode.com/problemset/ · https://neetcode.io/practice
- <a id="r-adr"></a>**🛠 Architecture Decision Records (ADR)** — шаблоны и примеры записей архитектурных решений. https://adr.github.io/

### Поиск работы
- <a id="r-jobs"></a>**📬 Площадки для откликов** — LinkedIn Jobs, Welcome to the Jungle (бывший Otta; удалённые вакансии в EU и UK), прямые обращения к рекрутерам. https://www.linkedin.com/jobs/ · https://www.welcometothejungle.com/
- <a id="r-salary"></a>**📬 Зарплаты** — levels.fyi (по городам, компаниям и грейдам) и Glassdoor. https://www.levels.fyi/ · https://www.glassdoor.com/

---

## 2. Повторяющийся шаблон практики (каждый Д6)

Каждую неделю: **одна задача за 45 минут вслух, на английском, со схемой в [Excalidraw](#r-excalidraw).**

1. Требования: функциональные и нефункциональные (5 мин).
2. Оценки на салфетке: QPS, объём хранения, пропускная способность (5 мин).
3. API и модель данных (5 мин).
4. Высокоуровневая схема (10 мин).
5. Deep dive в 1–2 узких места (15 мин).
6. Компромиссы и что сделали бы иначе (5 мин).

После этого сравните своё решение с эталонным разбором ([Hello Interview](#r-hello), [Alex Xu](#r-xu), [System Design Primer](#r-primer)). Запишите в `design-journal.md` три вещи, которые упустили.

---

## ФАЗА 1. Фундамент (недели 1–8)

### Неделя 1. Подход к задаче и оценки на салфетке
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [Hello Interview](#r-hello): [Delivery Framework](https://www.hellointerview.com/learn/system-design/in-a-hurry/delivery)</li><li>📄 [System Design Primer](#r-primer): [How to approach a system design interview question](https://github.com/donnemartin/system-design-primer#how-to-approach-a-system-design-interview-question)</li></ul> |
| Д2 | <ul><li>🧭 [Latency numbers](#r-latency): пройдите интерактив по годам</li><li>📄 [System Design Primer](#r-primer): [Powers of two](https://github.com/donnemartin/system-design-primer#powers-of-two-table), [Latency numbers](https://github.com/donnemartin/system-design-primer#latency-numbers-every-programmer-should-know)</li><li>🛠 **Упражнение:** оцените QPS и объём хранения в год для Twitter при 200M DAU</li></ul> |
| Д3 | <ul><li>🎬 [Kleppmann](#r-kleppmann): [лекция 1 — Introduction](https://www.youtube.com/playlist?list=PLeKd45zvjcDFUEv_ohr_HdUFe97RItdiB)</li><li>📖 [DDIA](#r-ddia), гл. 1: Reliable, Scalable, Maintainable Applications</li></ul> |
| Д4 | <ul><li>📖 [DDIA](#r-ddia): дочитать гл. 1</li><li>🛠 **Упражнение:** сформулируйте SLI и SLO для одного из своих проектов (латентность p99, доступность)</li></ul> |
| Д5 | <ul><li>🎬 [Harvard CS75: Scalability](#r-harvard) — или —</li><li>📖 [Alex Xu, т. 1](#r-xu), гл. 1: [Scale from zero to millions of users](https://bytebytego.com/courses/system-design-interview/scale-from-zero-to-millions-of-users)</li></ul> |
| Д6 | <ul><li>🧩 **Задача: URL shortener (bit.ly)** по шаблону</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Bitly](https://www.hellointerview.com/learn/system-design/problem-breakdowns/bitly)</li></ul> |

### Неделя 2. Модели данных и хранение
| День | Что делать |
|---|---|
| Д1 | <ul><li>📖 [DDIA](#r-ddia), гл. 2: реляционная, документная и графовая модели</li></ul> |
| Д2 | <ul><li>📖 [DDIA](#r-ddia), гл. 3, первая половина: хеш-индексы, SSTable, LSM-деревья</li></ul> |
| Д3 | <ul><li>📖 [DDIA](#r-ddia), гл. 3, вторая половина: B-деревья, OLTP и OLAP, колоночное хранение</li><li>🎬 [Hussein Nasser](#r-nasser): [видео о B-tree и LSM](https://www.youtube.com/@hnasr/search?query=LSM%20B-tree)</li></ul> |
| Д4 | <ul><li>🛠 **Упражнение (C#):** append-only key-value хранилище с in-memory hash-индексом и компакцией (примерно 150 строк)</li></ul> |
| Д5 | <ul><li>📄 [System Design Primer](#r-primer): [SQL or NoSQL](https://github.com/donnemartin/system-design-primer#sql-or-nosql)</li><li>📄 [Azure Architecture Center](#r-azarch): [выбор хранилища данных](https://learn.microsoft.com/azure/architecture/guide/technology-choices/data-store-decision-tree)</li><li>🛠 **Упражнение:** сравните Cosmos DB, DynamoDB, Cassandra и PostgreSQL по ключевым свойствам</li></ul> |
| Д6 | <ul><li>🧩 **Задача: Pastebin** по шаблону</li><li>📄 Сверка: [System Design Primer](#r-primer) — [Pastebin](https://github.com/donnemartin/system-design-primer/blob/master/solutions/system_design/pastebin/README.md)</li></ul> |

### Неделя 3. Сеть, API, балансировка
| День | Что делать |
|---|---|
| Д1 | <ul><li>📖 [DDIA](#r-ddia), гл. 4: форматы кодирования и эволюция схем (JSON, Protobuf, Avro)</li></ul> |
| Д2 | <ul><li>🎬 [Hussein Nasser](#r-nasser): [REST, gRPC, GraphQL, WebSocket, SSE, long polling](https://www.youtube.com/@hnasr/search?query=websockets%20long%20polling%20server%20sent%20events)</li><li>📄 [Hello Interview](#r-hello): [Networking Essentials](https://www.hellointerview.com/learn/system-design/core-concepts/networking-essentials)</li></ul> |
| Д3 | <ul><li>📄 [System Design Primer](#r-primer): [Load balancer](https://github.com/donnemartin/system-design-primer#load-balancer), [Reverse proxy](https://github.com/donnemartin/system-design-primer#reverse-proxy-web-server), [DNS](https://github.com/donnemartin/system-design-primer#domain-name-system), [CDN](https://github.com/donnemartin/system-design-primer#content-delivery-network)</li><li>Тема: балансировщики L4 и L7, API gateway</li></ul> |
| Д4 | <ul><li>🛠 **Упражнение (.NET):** gRPC-сервис; добавьте поле в схему и проверьте обратную совместимость со старым клиентом</li><li>📄 [Документация .NET](#r-dotnet): [версионирование gRPC-сервисов](https://learn.microsoft.com/aspnet/core/grpc/versioning)</li></ul> |
| Д5 | <ul><li>📖 [Alex Xu, т. 1](#r-xu), гл. 4: [Design a rate limiter](https://bytebytego.com/courses/system-design-interview/design-a-rate-limiter) — token bucket, leaky bucket, sliding window</li><li>📄 [Документация .NET](#r-dotnet): [rate limiting в ASP.NET Core](https://learn.microsoft.com/aspnet/core/performance/rate-limit) (`System.Threading.RateLimiting`)</li></ul> |
| Д6 | <ul><li>🧩 **Задача: распределённый rate limiter** (с Redis) по шаблону</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Distributed Rate Limiter](https://www.hellointerview.com/learn/system-design/problem-breakdowns/distributed-rate-limiter)</li></ul> |

### Неделя 4. Репликация
| День | Что делать |
|---|---|
| Д1 | <ul><li>🎬 [Kleppmann](#r-kleppmann): [лекция 2 — Models of distributed systems](https://www.youtube.com/playlist?list=PLeKd45zvjcDFUEv_ohr_HdUFe97RItdiB)</li></ul> |
| Д2 | <ul><li>📖 [DDIA](#r-ddia), гл. 5: leader и follower, синхронная и асинхронная репликация, отставание реплик</li></ul> |
| Д3 | <ul><li>📖 [DDIA](#r-ddia), гл. 5: multi-leader, leaderless, кворумы (W + R > N)</li><li>🎬 [Kleppmann](#r-kleppmann): [лекция 5 — Replication](https://www.youtube.com/playlist?list=PLeKd45zvjcDFUEv_ohr_HdUFe97RItdiB)</li></ul> |
| Д4 | <ul><li>🛠 **Упражнение:** PostgreSQL primary + replica в Docker. Измерьте отставание реплики и воспроизведите нарушение read-your-writes</li><li>📄 [Документация PostgreSQL](#r-techdocs): [streaming replication](https://www.postgresql.org/docs/current/warm-standby.html)</li></ul> |
| Д5 | <ul><li>🗣 **Упражнение:** гарантии консистентности read-your-writes, monotonic reads, consistent prefix — опишите своими словами на английском (полстраницы)</li></ul> |
| Д6 | <ul><li>🧩 **Задача: распределённое key-value хранилище** по шаблону</li><li>📖 Сверка: [Alex Xu, т. 1](#r-xu), гл. 6: [Design a key-value store](https://bytebytego.com/courses/system-design-interview/design-a-key-value-store)</li></ul> |

### Неделя 5. Партиционирование и кэширование
| День | Что делать |
|---|---|
| Д1 | <ul><li>📖 [DDIA](#r-ddia), гл. 6: партиционирование по ключу и по хешу, горячие ключи, вторичные индексы</li></ul> |
| Д2 | <ul><li>🎬 [ByteByteGo](#r-bytebytego): [consistent hashing](https://www.youtube.com/@ByteByteGo/search?query=consistent%20hashing)</li><li>📖 [Alex Xu, т. 1](#r-xu), гл. 5: [Design consistent hashing](https://bytebytego.com/courses/system-design-interview/design-consistent-hashing) — виртуальные узлы</li></ul> |
| Д3 | <ul><li>🛠 **Упражнение (C#):** consistent hashing с виртуальными узлами. Измерьте, сколько ключей переезжает при добавлении узла</li></ul> |
| Д4 | <ul><li>📄 [Hello Interview](#r-hello): [Caching](https://www.hellointerview.com/learn/system-design/core-concepts/caching) — cache-aside, write-through, write-behind</li><li>📄 [System Design Primer](#r-primer): [Cache](https://github.com/donnemartin/system-design-primer#cache) — инвалидация, TTL, cache stampede</li></ul> |
| Д5 | <ul><li>📄 [Hello Interview](#r-hello): [Redis deep dive](https://www.hellointerview.com/learn/system-design/deep-dives/redis) — структуры данных, Cluster</li><li>📄 [Документация Redis](#r-techdocs): [персистентность](https://redis.io/docs/latest/operate/oss_and_stack/management/persistence/)</li><li>🛠 Сопоставьте с Azure Cache for Redis и ElastiCache</li></ul> |
| Д6 | <ul><li>🧩 **Задача: news feed / timeline** (fan-out on write или on read)</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Facebook News Feed](https://www.hellointerview.com/learn/system-design/problem-breakdowns/fb-news-feed)</li></ul> |

### Неделя 6. Транзакции и распределённые бизнес-процессы
| День | Что делать |
|---|---|
| Д1 | <ul><li>📖 [DDIA](#r-ddia), гл. 7: ACID, уровни изоляции, аномалии (lost update, write skew)</li></ul> |
| Д2 | <ul><li>📖 [DDIA](#r-ddia), гл. 7: snapshot isolation и serializable</li><li>🛠 **Упражнение:** воспроизведите write skew в PostgreSQL двумя сессиями</li><li>📄 [Документация PostgreSQL](#r-techdocs): [Transaction Isolation](https://www.postgresql.org/docs/current/transaction-iso.html)</li></ul> |
| Д3 | <ul><li>📄 [microservices.io](#r-msio): [Transactional Outbox](https://microservices.io/patterns/data/transactional-outbox.html), [Saga](https://microservices.io/patterns/data/saga.html) (хореография и оркестрация)</li><li>📄 [Hello Interview](#r-hello): [Multi-step Processes](https://www.hellointerview.com/learn/system-design/patterns/multi-step-processes)</li><li>Тема: Inbox, идемпотентность и idempotency keys</li></ul> |
| Д4 | <ul><li>🛠 **Упражнение (.NET):** Outbox + RabbitMQ (вручную или через MassTransit), идемпотентный потребитель</li><li>📄 [Документация MassTransit](#r-techdocs): [Transactional Outbox](https://masstransit.io/documentation/patterns/transactional-outbox)</li></ul> |
| Д5 | <ul><li>📄 [Azure Architecture Center](#r-azarch): [Saga](https://learn.microsoft.com/azure/architecture/patterns/saga), [Compensating Transaction](https://learn.microsoft.com/azure/architecture/patterns/compensating-transaction), [Retry](https://learn.microsoft.com/azure/architecture/patterns/retry), [Circuit Breaker](https://learn.microsoft.com/azure/architecture/patterns/circuit-breaker)</li></ul> |
| Д6 | <ul><li>🧩 **Задача: платёжная система или Ticketmaster** (бронирование мест без двойной продажи)</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Ticketmaster](https://www.hellointerview.com/learn/system-design/problem-breakdowns/ticketmaster) или [Payment System](https://www.hellointerview.com/learn/system-design/problem-breakdowns/payment-system)</li></ul> |

### Неделя 7. Сбои, время, консенсус
| День | Что делать |
|---|---|
| Д1 | <ul><li>📖 [DDIA](#r-ddia), гл. 8: ненадёжные сети и часы, паузы процессов, fencing tokens</li></ul> |
| Д2 | <ul><li>🎬 [Kleppmann](#r-kleppmann): [лекции 3 — Time, clocks и 4 — Broadcast](https://www.youtube.com/playlist?list=PLeKd45zvjcDFUEv_ohr_HdUFe97RItdiB)</li></ul> |
| Д3 | <ul><li>📖 [DDIA](#r-ddia), гл. 9: линеаризуемость, CAP, PACELC</li><li>📄 [Hello Interview](#r-hello): [CAP Theorem](https://www.hellointerview.com/learn/system-design/core-concepts/cap-theorem)</li></ul> |
| Д4 | <ul><li>🧭 [Визуализация Raft](#r-raftviz)</li><li>🎬 [MIT 6.824](#r-mit): [лекция о Raft](https://pdos.csail.mit.edu/6.824/schedule.html)</li><li>🎬 [Kleppmann](#r-kleppmann): [лекция 6 — Consensus](https://www.youtube.com/playlist?list=PLeKd45zvjcDFUEv_ohr_HdUFe97RItdiB)</li></ul> |
| Д5 | <ul><li>🗣 **Упражнение:** на английском объясните одностраничным текстом, как Raft выбирает лидера и почему нужен кворум. Потом расскажите это вслух за 3 минуты</li></ul> |
| Д6 | <ul><li>🧩 **Задача: распределённый планировщик задач или сервис блокировок**</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Job Scheduler](https://www.hellointerview.com/learn/system-design/problem-breakdowns/job-scheduler)</li></ul> |

### Неделя 8. Потоки данных и observability. Контрольная точка
| День | Что делать |
|---|---|
| Д1 | <ul><li>📖 [DDIA](#r-ddia), гл. 11: логи сообщений (Kafka), CDC, event sourcing</li><li>📄 [Hello Interview](#r-hello): [Kafka deep dive](https://www.hellointerview.com/learn/system-design/deep-dives/kafka)</li></ul> |
| Д2 | <ul><li>📄 [Azure Architecture Center](#r-azarch): [выбор сервиса сообщений](https://learn.microsoft.com/azure/architecture/guide/technology-choices/messaging) — Service Bus, Event Hubs, Event Grid</li><li>Тема: Kafka и RabbitMQ; семантика at-least-once и exactly-once</li></ul> |
| Д3 | <ul><li>📖 [DDIA](#r-ddia), гл. 10 (обзорно): batch-обработка, MapReduce</li><li>📄 [Azure Architecture Center](#r-azarch): [CQRS](https://learn.microsoft.com/azure/architecture/patterns/cqrs)</li></ul> |
| Д4 | <ul><li>📄 [Документация OpenTelemetry](#r-techdocs): [What is OpenTelemetry](https://opentelemetry.io/docs/what-is-opentelemetry/) — логи, метрики, трейсы</li><li>🗣 **Упражнение:** сформулируйте, как бы вы объясняли свой опыт с Loki и Tempo на собеседовании</li></ul> |
| Д5 | <ul><li>🛠 Повторите заметки из `design-journal.md` за 7 недель</li></ul> |
| Д6 | <ul><li>🗣 [**Первое пробное собеседование с партнёром**](#r-peer) (на английском)</li><li>🧩 Задача: ad click aggregator или top-K. Сверка: [Hello Interview](#r-hello) — [Ad Click Aggregator](https://www.hellointerview.com/learn/system-design/problem-breakdowns/ad-click-aggregator), [Top K](https://www.hellointerview.com/learn/system-design/problem-breakdowns/top-k)</li></ul> |

---

## ФАЗА 2. Azure Solutions Architect Expert (недели 9–16)

**Материалы:** learning paths на [Microsoft Learn](#r-mslearn), [John Savill](#r-savill) (AZ-104 Study List и AZ-305 Study Cram), бесплатные [Practice Assessments](#r-mspractice).
**Лабораторные:** [бесплатный аккаунт Azure](#r-azfree) (стартовый кредит) или песочницы Microsoft Learn. **Ставьте лимиты бюджета (Budgets + alerts) и удаляйте ресурсы после лабораторных.**

### Неделя 9. AZ-104: идентичность и governance
| День | Что делать |
|---|---|
| Д1 | <ul><li>🎯 Запишитесь на [AZ-104](#r-az104) через 4 недели: дедлайн дисциплинирует</li><li>📄 [Microsoft Learn](#r-mslearn): [AZ-104: Manage identities and governance](https://learn.microsoft.com/training/paths/az-104-manage-identities-governance/) — Entra ID: пользователи, группы, лицензии</li></ul> |
| Д2 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [Azure RBAC](https://learn.microsoft.com/azure/role-based-access-control/overview) — кастомные роли, scope</li><li>🛠 **Лабораторная:** роль с минимальными правами</li></ul> |
| Д3 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [Azure Policy](https://learn.microsoft.com/azure/governance/policy/overview), management groups, теги, блокировки ресурсов</li></ul> |
| Д4 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [Budgets в Cost Management](https://learn.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets) — подписки и стоимость</li><li>🎬 [John Savill](#r-savill): [AZ-104 Study List](https://www.youtube.com/playlist?list=PLlVtbbG169nGlGPWs9xaLKT1KfwqREHbs) — видео по identity и governance</li></ul> |
| Д5 | <ul><li>🧪 [Practice Assessment AZ-104](#r-mspractice) №1, разбор ошибок</li></ul> |
| Д6 | <ul><li>🧩 **Задача System Design: чат (WhatsApp)** + сопоставление компонентов с сервисами Azure</li><li>📄 Сверка: [Hello Interview](#r-hello) — [WhatsApp](https://www.hellointerview.com/learn/system-design/problem-breakdowns/whatsapp)</li></ul> |

### Неделя 10. AZ-104: хранилища и вычисления
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [AZ-104: Implement and manage storage](https://learn.microsoft.com/training/paths/az-104-manage-storage/) — storage accounts, уровни, жизненный цикл</li><li>📄 [Microsoft Learn](#r-mslearn): [репликация LRS, ZRS, GRS, GZRS](https://learn.microsoft.com/azure/storage/common/storage-redundancy)</li></ul> |
| Д2 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [SAS](https://learn.microsoft.com/azure/storage/common/storage-sas-overview), приватные endpoints, Azure Files, AzCopy</li><li>🛠 **Лабораторная**</li></ul> |
| Д3 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [AZ-104: Deploy and manage compute](https://learn.microsoft.com/training/paths/az-104-manage-compute-resources/) — VM, [availability sets и zones](https://learn.microsoft.com/azure/virtual-machines/availability), VM Scale Sets</li></ul> |
| Д4 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [сравнение контейнерных сервисов](https://learn.microsoft.com/azure/container-apps/compare-options) — App Service, Container Instances, Container Apps, основы AKS</li></ul> |
| Д5 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [ARM и Bicep](https://learn.microsoft.com/azure/azure-resource-manager/bicep/overview)</li><li>🛠 **Лабораторная:** разверните App Service + Storage через Bicep</li></ul> |
| Д6 | <ul><li>🧩 **Задача: Dropbox / file sync**</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Dropbox](https://www.hellointerview.com/learn/system-design/problem-breakdowns/dropbox)</li></ul> |

### Неделя 11. AZ-104: сеть
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [AZ-104: Configure and manage virtual networks](https://learn.microsoft.com/training/paths/az-104-manage-virtual-networks/) — VNet, подсети, NSG, ASG, peering</li></ul> |
| Д2 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [User-Defined Routes](https://learn.microsoft.com/azure/virtual-network/virtual-networks-udr-overview), VPN Gateway, ExpressRoute (обзор)</li></ul> |
| Д3 | <ul><li>📄 [Azure Architecture Center](#r-azarch): [выбор балансировщика](https://learn.microsoft.com/azure/architecture/guide/technology-choices/load-balancing-overview)</li><li>🛠 Сравнительная таблица: Load Balancer, Application Gateway и WAF, Front Door, Traffic Manager</li></ul> |
| Д4 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [Private Link](https://learn.microsoft.com/azure/private-link/private-link-overview), Private DNS, service endpoints</li><li>🛠 **Лабораторная:** hub-spoke из двух VNet ([эталонная архитектура](https://learn.microsoft.com/azure/architecture/networking/architecture/hub-spoke))</li></ul> |
| Д5 | <ul><li>🧪 [Practice Assessment AZ-104](#r-mspractice) №2, разбор ошибок</li></ul> |
| Д6 | <ul><li>🧩 **Задача: YouTube / video streaming** (CDN, транскодинг)</li><li>📄 Сверка: [Hello Interview](#r-hello) — [YouTube](https://www.hellointerview.com/learn/system-design/problem-breakdowns/youtube)</li></ul> |

### Неделя 12. AZ-104: мониторинг, backup, экзамен
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [AZ-104: Monitor and back up resources](https://learn.microsoft.com/training/paths/az-104-monitor-backup-resources/) — Azure Monitor, алерты</li><li>📄 [Microsoft Learn](#r-mslearn): [основы KQL в Log Analytics](https://learn.microsoft.com/azure/azure-monitor/logs/get-started-queries)</li></ul> |
| Д2 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [Azure Backup](https://learn.microsoft.com/azure/backup/backup-overview), [Site Recovery](https://learn.microsoft.com/azure/site-recovery/site-recovery-overview)</li></ul> |
| Д3 | <ul><li>📄 [Microsoft Learn](#r-mslearn): повторение слабых доменов по [study guide AZ-104](https://learn.microsoft.com/credentials/certifications/resources/study-guides/az-104) и результатам Practice Assessment</li></ul> |
| Д4 | <ul><li>🧪 Полный пробный тест: [MeasureUp](#r-measureup) или бесплатный [Practice Assessment](#r-mspractice), цель — больше 80%</li></ul> |
| Д5 | <ul><li>⏸ Лёгкое повторение и отдых</li></ul> |
| Д6 | <ul><li>🎯 **Экзамен [AZ-104](#r-az104)**</li><li>📬 Обновите резюме и LinkedIn, начинайте откликаться на [вакансии](#r-jobs)</li></ul> |

### Неделя 13. AZ-305: identity, governance, мониторинг
| День | Что делать |
|---|---|
| Д1 | <ul><li>🎯 Запишитесь на [AZ-305](#r-az305) через 4 недели</li><li>📄 [Azure Well-Architected Framework](#r-azwaf): [5 столпов](https://learn.microsoft.com/azure/well-architected/pillars)</li></ul> |
| Д2 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [AZ-305: Design identity, governance, and monitor solutions](https://learn.microsoft.com/training/paths/design-identity-governance-monitor-solutions/) — Entra ID, [External ID (B2B и B2C)](https://learn.microsoft.com/entra/external-id/external-identities-overview), [managed identities](https://learn.microsoft.com/entra/identity/managed-identities-azure-resources/overview), [Key Vault](https://learn.microsoft.com/azure/key-vault/general/overview)</li></ul> |
| Д3 | <ul><li>📄 [Cloud Adoption Framework](#r-azwaf): [landing zones](https://learn.microsoft.com/azure/cloud-adoption-framework/ready/landing-zone/) — governance и мониторинг для организации</li></ul> |
| Д4 | <ul><li>🎬 [John Savill](#r-savill): [AZ-305 Study Cram](https://www.youtube.com/watch?v=vq9LuCM4YP4), первая часть</li></ul> |
| Д5 | <ul><li>🛠 **Упражнение:** напишите [ADR](#r-adr) «Выбор механизма аутентификации для B2C-приложения», 1 страница на английском</li></ul> |
| Д6 | <ul><li>🧩 **Задача: Uber / сервис на основе геолокации** (гео-индекс, геохэш)</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Uber](https://www.hellointerview.com/learn/system-design/problem-breakdowns/uber); 📖 [Alex Xu, т. 2](#r-xu), гл. 1: [Proximity service](https://bytebytego.com/courses/system-design-interview/proximity-service)</li></ul> |

### Неделя 14. AZ-305: данные
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [AZ-305: Design data storage solutions](https://learn.microsoft.com/training/paths/design-data-storage-solutions/) — Azure SQL, SQL Managed Instance, Cosmos DB, PostgreSQL Flexible</li></ul> |
| Д2 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [Cosmos DB: partition key](https://learn.microsoft.com/azure/cosmos-db/partitioning-overview), [уровни консистентности](https://learn.microsoft.com/azure/cosmos-db/consistency-levels) (свяжите с неделей 4), [RU](https://learn.microsoft.com/azure/cosmos-db/request-units)</li></ul> |
| Д3 | <ul><li>Тема: интеграция данных — Data Factory, Synapse и Fabric (обзор), Event Hubs, Stream Analytics</li><li>📄 [Microsoft Learn](#r-mslearn): соответствующие модули в [AZ-305: Design data storage solutions](https://learn.microsoft.com/training/paths/design-data-storage-solutions/)</li></ul> |
| Д4 | <ul><li>📄 [Azure Architecture Center](#r-azarch): [сервисы сообщений](https://learn.microsoft.com/azure/architecture/guide/technology-choices/messaging) — Service Bus, Event Grid</li><li>Тема: API Management, Logic Apps</li></ul> |
| Д5 | <ul><li>🧪 [Practice Assessment AZ-305](#r-mspractice) №1</li></ul> |
| Д6 | <ul><li>🧩 **Задача: поисковый автокомплит (typeahead)**</li><li>📖 Сверка: [Alex Xu, т. 1](#r-xu), гл. 13: [Design a search autocomplete system](https://bytebytego.com/courses/system-design-interview/design-a-search-autocomplete-system)</li></ul> |

### Неделя 15. AZ-305: непрерывность бизнеса и инфраструктура
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [AZ-305: Design business continuity solutions](https://learn.microsoft.com/training/paths/design-business-continuity-solutions/) — RPO и RTO</li><li>📄 [Microsoft Learn](#r-mslearn): [стратегии DR](https://learn.microsoft.com/azure/reliability/disaster-recovery-overview), multi-region: active-active и active-passive</li></ul> |
| Д2 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [HA в Azure SQL](https://learn.microsoft.com/azure/azure-sql/database/high-availability-sla), [глобальное распределение Cosmos DB](https://learn.microsoft.com/azure/cosmos-db/distribute-data-globally)</li></ul> |
| Д3 | <ul><li>📄 [Azure Architecture Center](#r-azarch): [дерево выбора вычислительного сервиса](https://learn.microsoft.com/azure/architecture/guide/technology-choices/compute-decision-tree) — VM, App Service, Functions, Container Apps, AKS</li></ul> |
| Д4 | <ul><li>📄 [Microsoft Learn](#r-mslearn): [AZ-305: Design infrastructure solutions](https://learn.microsoft.com/training/paths/design-infranstructure-solutions/) — hub-spoke, [Virtual WAN](https://learn.microsoft.com/azure/virtual-wan/virtual-wan-about), Front Door или Application Gateway</li><li>📄 [Microsoft Learn](#r-mslearn): [Azure Migrate](https://learn.microsoft.com/azure/migrate/migrate-services-overview)</li></ul> |
| Д5 | <ul><li>🛠 **Упражнение:** спроектируйте multi-region архитектуру для своего проекта: схема + оценка стоимости в [Pricing Calculator](#r-azfree)</li></ul> |
| Д6 | <ul><li>🧩 **Задача: web crawler**</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Web Crawler](https://www.hellointerview.com/learn/system-design/problem-breakdowns/web-crawler)</li></ul> |

### Неделя 16. AZ-305: экзамен
| День | Что делать |
|---|---|
| Д1 | <ul><li>🧪 [Microsoft Exam Sandbox](#r-examdemo): разбор формата case studies</li></ul> |
| Д2 | <ul><li>🧪 [Practice Assessment AZ-305](#r-mspractice) №2</li><li>📄 Повторение слабых доменов по [study guide AZ-305](https://learn.microsoft.com/credentials/certifications/resources/study-guides/az-305)</li></ul> |
| Д3 | <ul><li>🎬 [John Savill](#r-savill): [AZ-305 Study Cram](https://www.youtube.com/watch?v=vq9LuCM4YP4), вторая часть</li></ul> |
| Д4 | <ul><li>🧪 Полный пробный тест: [MeasureUp](#r-measureup) или [Practice Assessment](#r-mspractice), цель — больше 80%</li></ul> |
| Д5 | <ul><li>⏸ Отдых</li></ul> |
| Д6 | <ul><li>🎯 **Экзамен [AZ-305](#r-az305) → Azure Solutions Architect Expert**</li><li>📬 Добавьте бейдж Credly в LinkedIn</li></ul> |

---

## ФАЗА 3. AWS Solutions Architect Associate (недели 17–22)

**Материалы:** [курс freeCodeCamp](#r-fcc) (Andrew Brown) по SAA-C03, [AWS Skill Builder](#r-skillbuilder) (бесплатные Exam Prep и Official Practice Question Set), [тесты Tutorials Dojo](#r-td) (платные, лучшие).
**Лайфхак:** соотносите каждый сервис AWS с уже знакомым Azure-аналогом.

| Azure | AWS |
|---|---|
| Entra ID + RBAC | IAM (+ IAM Identity Center) |
| VNet / NSG | VPC / Security Groups, NACL |
| Blob Storage | S3 |
| VM / VMSS | EC2 / Auto Scaling Groups |
| App Service / Functions | Elastic Beanstalk / Lambda |
| AKS / Container Apps | EKS / ECS + Fargate |
| Azure SQL / Cosmos DB | RDS, Aurora / DynamoDB |
| Service Bus / Event Grid / Event Hubs | SQS, SNS / EventBridge / Kinesis |
| Front Door / Application Gateway | CloudFront / ALB |
| Azure Monitor | CloudWatch |

### Неделя 17. IAM, VPC
| День | Что делать |
|---|---|
| Д1 | <ul><li>🎯 Запишитесь на [SAA-C03](#r-saa) через 6 недель</li><li>🛠 Создайте аккаунт [AWS Free Tier](#r-awsfree) + [Budgets с алертом на $5](https://docs.aws.amazon.com/cost-management/latest/userguide/budgets-managing-costs.html)</li><li>📄 [AWS Docs](#r-awsdocs): [IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html) — пользователи, роли, политики, STS</li><li>🎬 [freeCodeCamp SAA-C03](#r-fcc): разделы по IAM</li></ul> |
| Д2 | <ul><li>📄 [AWS Docs](#r-awsdocs): [Organizations и SCP](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html), [IAM Identity Center](https://docs.aws.amazon.com/singlesignon/latest/userguide/what-is.html)</li></ul> |
| Д3 | <ul><li>📄 [AWS Docs](#r-awsdocs): [VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) — подсети, route tables, IGW, NAT Gateway, SG и NACL</li></ul> |
| Д4 | <ul><li>🛠 **Лабораторная:** VPC с публичной и приватной подсетью, EC2 в приватной, доступ через [SSM Session Manager](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager.html)</li></ul> |
| Д5 | <ul><li>📄 [AWS Docs](#r-awsdocs): VPC peering, [Transit Gateway](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html), [VPC endpoints и PrivateLink](https://docs.aws.amazon.com/vpc/latest/privatelink/what-is-privatelink.html)</li></ul> |
| Д6 | <ul><li>🧩 **Задача: notification service** (push, email, SMS) + отображение на сервисы AWS</li><li>📖 Сверка: [Alex Xu, т. 1](#r-xu), гл. 10: [Design a notification system](https://bytebytego.com/courses/system-design-interview/design-a-notification-system)</li></ul> |

### Неделя 18. Вычисления и хранилища
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [AWS Docs](#r-awsdocs): EC2 — типы инстансов, [модели покупки](https://aws.amazon.com/ec2/pricing/) (On-Demand, Spot, RI, Savings Plans)</li></ul> |
| Д2 | <ul><li>📄 [AWS Docs](#r-awsdocs): [ELB](https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/how-elastic-load-balancing-works.html) (ALB, NLB), [Auto Scaling](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html)</li><li>🛠 **Лабораторная:** ALB + ASG</li></ul> |
| Д3 | <ul><li>📄 [AWS Docs](#r-awsdocs): [S3: классы хранения](https://docs.aws.amazon.com/AmazonS3/latest/userguide/storage-class-intro.html), жизненный цикл, репликация, шифрование, [presigned URL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/using-presigned-url.html)</li></ul> |
| Д4 | <ul><li>📄 [AWS Docs](#r-awsdocs): [обзор хранилищ AWS](https://aws.amazon.com/products/storage/) — EBS, EFS, FSx, Storage Gateway: когда что выбирать</li></ul> |
| Д5 | <ul><li>📄 [AWS Docs](#r-awsdocs): [Lambda](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html), API Gateway, [ECS/Fargate](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS_Fargate.html), EKS (обзор)</li></ul> |
| Д6 | <ul><li>🧩 **Задача: Google Docs / совместное редактирование** (OT или CRDT)</li><li>🎬 [Kleppmann](#r-kleppmann): [лекция 8 — Case studies](https://www.youtube.com/playlist?list=PLeKd45zvjcDFUEv_ohr_HdUFe97RItdiB)</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Google Docs](https://www.hellointerview.com/learn/system-design/problem-breakdowns/google-docs)</li></ul> |

### Неделя 19. Базы данных и интеграция
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [AWS Docs](#r-awsdocs): [RDS Multi-AZ](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.MultiAZ.html) и [read replicas](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_ReadRepl.html) — разница!, Aurora, [RDS Proxy](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/rds-proxy.html)</li></ul> |
| Д2 | <ul><li>📄 [AWS Docs](#r-awsdocs): [DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.html) — ключи, GSI и LSI, capacity modes, DAX, Streams</li><li>📄 [Hello Interview](#r-hello): [DynamoDB deep dive](https://www.hellointerview.com/learn/system-design/deep-dives/dynamodb)</li></ul> |
| Д3 | <ul><li>📄 [AWS Docs](#r-awsdocs) (обзор): [ElastiCache](https://docs.aws.amazon.com/AmazonElastiCache/latest/dg/WhatIs.html), [Redshift](https://docs.aws.amazon.com/redshift/latest/mgmt/welcome.html), [Athena](https://docs.aws.amazon.com/athena/latest/ug/what-is.html)</li></ul> |
| Д4 | <ul><li>📄 [AWS Docs](#r-awsdocs): [SQS, SNS или EventBridge](https://docs.aws.amazon.com/decision-guides/latest/sns-or-sqs-or-eventbridge/sns-or-sqs-or-eventbridge.html) (SQS standard и FIFO), [Kinesis](https://docs.aws.amazon.com/streams/latest/dev/introduction.html), [Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html)</li></ul> |
| Д5 | <ul><li>🧪 [AWS Skill Builder](#r-skillbuilder): Official Practice Question Set, разбор ошибок</li></ul> |
| Д6 | <ul><li>🧩 **Задача: система бронирования отелей**</li><li>📖 Сверка: [Alex Xu, т. 2](#r-xu), гл. 7: [Hotel reservation system](https://bytebytego.com/courses/system-design-interview/hotel-reservation-system)</li></ul> |

### Неделя 20. Устойчивость и безопасность
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [AWS Docs](#r-awsdocs): [Route 53: политики маршрутизации](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html), [CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html), [Global Accelerator](https://docs.aws.amazon.com/global-accelerator/latest/dg/what-is-global-accelerator.html)</li></ul> |
| Д2 | <ul><li>📄 [AWS Well-Architected](#r-awswa): [стратегии DR](https://docs.aws.amazon.com/whitepapers/latest/disaster-recovery-workloads-on-aws/disaster-recovery-options-in-the-cloud.html) — backup & restore, pilot light, warm standby, multi-site</li></ul> |
| Д3 | <ul><li>📄 [AWS Docs](#r-awsdocs): [KMS](https://docs.aws.amazon.com/kms/latest/developerguide/overview.html), [Secrets Manager](https://docs.aws.amazon.com/secretsmanager/latest/userguide/intro.html), [WAF и Shield](https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html), [GuardDuty](https://docs.aws.amazon.com/guardduty/latest/ug/what-is-guardduty.html), [Cognito](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html)</li></ul> |
| Д4 | <ul><li>📄 [AWS Docs](#r-awsdocs): [CloudWatch](https://docs.aws.amazon.com/cloudwatch/), [CloudTrail](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-user-guide.html), [Config](https://docs.aws.amazon.com/config/latest/developerguide/WhatIsConfig.html)</li></ul> |
| Д5 | <ul><li>🧪 [Tutorials Dojo](#r-td): тест №1, разбор ошибок</li></ul> |
| Д6 | <ul><li>🧩 **Задача: metrics / monitoring system** (time-series хранилище)</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Metrics Monitoring](https://www.hellointerview.com/learn/system-design/problem-breakdowns/metrics-monitoring); 📖 [Alex Xu, т. 2](#r-xu), гл. 5: [Metrics monitoring and alerting](https://bytebytego.com/courses/system-design-interview/metrics-monitoring-and-alerting-system)</li></ul> |

### Неделя 21. Стоимость и Well-Architected
| День | Что делать |
|---|---|
| Д1 | <ul><li>📄 [AWS Well-Architected](#r-awswa): [6 столпов](https://docs.aws.amazon.com/wellarchitected/latest/framework/the-pillars-of-the-framework.html) — сравните с [5 столпами Azure](#r-azwaf)</li></ul> |
| Д2 | <ul><li>📄 [AWS Docs](#r-awsdocs): [Cost Explorer](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/), [Spot](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-spot-instances.html), [Savings Plans](https://docs.aws.amazon.com/savingsplans/latest/userguide/what-is-savings-plans.html), выбор классов хранения</li></ul> |
| Д3 | <ul><li>📄 [AWS Docs](#r-awsdocs) (обзор): [DMS](https://docs.aws.amazon.com/dms/latest/userguide/Welcome.html), [DataSync](https://docs.aws.amazon.com/datasync/latest/userguide/what-is-datasync.html), [Snow family](https://aws.amazon.com/snow/)</li></ul> |
| Д4 | <ul><li>🧪 [Tutorials Dojo](#r-td): тест №2</li></ul> |
| Д5 | <ul><li>🛠 Повторение слабых доменов по результатам тестов</li></ul> |
| Д6 | <ul><li>🗣 [**Второе пробное собеседование**](#r-peer) (желательно с незнакомым человеком)</li></ul> |

### Неделя 22. Экзамен SAA-C03
| День | Что делать |
|---|---|
| Д1 | <ul><li>🧪 [Tutorials Dojo](#r-td): тест №3</li></ul> |
| Д2 | <ul><li>🛠 Разбор ошибок, повторение</li></ul> |
| Д3 | <ul><li>🧪 Финальный тест [Tutorials Dojo](#r-td), цель — больше 80%</li></ul> |
| Д4 | <ul><li>⏸ Лёгкое повторение</li></ul> |
| Д5 | <ul><li>⏸ Отдых</li></ul> |
| Д6 | <ul><li>🎯 **Экзамен [AWS SAA-C03](#r-saa)**</li></ul> |

---

## ФАЗА 4. Интенсив по собеседованиям и поиск работы (недели 23–26)

### Неделя 23. Задачи старшего уровня
| День | Что делать |
|---|---|
| Д1 | <ul><li>🎬 [Kleppmann](#r-kleppmann): [лекция 8 — Spanner и TrueTime](https://www.youtube.com/playlist?list=PLeKd45zvjcDFUEv_ohr_HdUFe97RItdiB)</li><li>📄 [Классические статьи](#r-papers): Spanner</li><li>Тема: multi-region и геораспределённые данные</li></ul> |
| Д2 | <ul><li>📄 [Azure Architecture Center](#r-azarch): [Strangler Fig](https://learn.microsoft.com/azure/architecture/patterns/strangler-fig), [микросервисы и границы сервисов](https://learn.microsoft.com/azure/architecture/microservices/) (DDD bounded contexts)</li></ul> |
| Д3 | <ul><li>🧩 Задача на время: **распределённый кэш**</li><li>📄 Сверка: [Hello Interview](#r-hello) — [Distributed Cache](https://www.hellointerview.com/learn/system-design/problem-breakdowns/distributed-cache)</li></ul> |
| Д4 | <ul><li>🧩 Задача на время: **платёжный шлюз с exactly-once эффектом**</li><li>📖 Сверка: [Alex Xu, т. 2](#r-xu), гл. 11: [Payment system](https://bytebytego.com/courses/system-design-interview/payment-system)</li></ul> |
| Д5 | <ul><li>🗣 Составьте 5 историй в формате STAR на английском: конфликт, провал, лидерство, сложное техническое решение, влияние на бизнес</li><li>📄 [Hello Interview](#r-hello): [Behavioral Interview](https://www.hellointerview.com/learn/behavioral/overview/introduction)</li></ul> |
| Д6 | <ul><li>🗣 [**Платное пробное собеседование**](#r-paidmock) с инженером FAANG</li></ul> |

### Недели 24–26. Ритм «собеседование + отклики»
| День | Что делать |
|---|---|
| Д1 | <ul><li>📬 10 откликов: [площадки и рекрутеры](#r-jobs)</li></ul> |
| Д2 | <ul><li>🧩 Задача System Design на время + самопроверка по [Alex Xu](#r-xu) или [Hello Interview](#r-hello)</li></ul> |
| Д3 | <ul><li>🗣 Behavioral: прогон историй STAR вслух, запись на видео</li></ul> |
| Д4 | <ul><li>🧩 Задача на время по разбору [Hello Interview](#r-hello), которую ещё не решали</li></ul> |
| Д5 | <ul><li>🛠 Кодинг-разминка: 1–2 задачи medium на [LeetCode](#r-leetcode) (продуктовые компании его тоже проверяют)</li></ul> |
| Д6 | <ul><li>🗣 [Пробное собеседование с партнёром](#r-peer)</li><li>🛠 Ретроспектива по `design-journal.md`</li></ul> |

---

## Упражнения на протяжении всего плана

- **Портфолио.** На каждые 4 недели — один [ADR](#r-adr) или design doc по своим проектам (выбор брокера, трассировка, аутентификация). Публикуйте их в GitHub-репозитории `architecture-notes` на английском. Такую ссылку можно положить в резюме.
- **Флеш-карточки** ([Anki](#r-anki), бесплатно): числа задержек, лимиты сервисов, соответствия Azure ↔ AWS, уровни консистентности.
- **Английский.** Все упражнения на объяснение делайте вслух и на английском: собеседование по System Design — это в первую очередь коммуникация.
- **Статьи для глубины** (по одной в месяц): [Dynamo, Raft, Spanner, Kafka](#r-papers). Затем разбор в лекциях [MIT 6.824](#r-mit).
- **Для кругозора:** доклады [HighLoad++](#r-highload), статьи на [Habr](#r-habr), разборы [Jordan Has No Life](#r-jordan).

## Опционально, после 26-й недели

- **iSAQB CPSA-F**, если целитесь в Германию, Австрию или Швейцарию: https://www.isaqb.org/certifications/cpsa-foundation-level/
- **AWS Solutions Architect Professional**, если цель — роль архитектора: https://aws.amazon.com/certification/certified-solutions-architect-professional/
- Сравнение зарплат: [levels.fyi и Glassdoor](#r-salary).

## Контрольные точки

| Неделя | Критерий готовности |
|---|---|
| 8 | Решаете типовую задачу за 45 минут и объясняете компромиссы на английском |
| 12 | Сдан AZ-104, резюме обновлено, начаты отклики |
| 16 | Сдан AZ-305 (Azure Solutions Architect Expert) |
| 22 | Сдан AWS SAA-C03 |
| 26 | Минимум 6 пробных собеседований, 40+ откликов, есть первые технические собеседования |
