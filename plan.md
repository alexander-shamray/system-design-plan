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

### Бесплатные: видео и курсы
- **Martin Kleppmann — Distributed Systems (Cambridge)**: 8 лекций на YouTube + конспект в PDF. Лучшее бесплатное введение в теорию. https://www.cl.cam.ac.uk/teaching/2122/ConcDisSys/
- **MIT 6.824 / 6.5840 Distributed Systems**: лекции Robert Morris на YouTube, статьи и лабораторные. https://pdos.csail.mit.edu/6.824/
- **ByteByteGo (YouTube)**: короткие видео с наглядными схемами (Alex Xu).
- **Hussein Nasser (YouTube)**: базы данных, прокси, протоколы, бэкенд изнутри.
- **Jordan Has No Life (YouTube)**: разборы задач System Design, глубокие.
- **John Savill's Technical Training (YouTube)**: AZ-104 Master Class, AZ-305 Study Cram. Лучшее бесплатное по Azure.
- **freeCodeCamp (YouTube)**: полные курсы к сертификатам AWS SAA-C03 и Azure (Andrew Brown / ExamPro).
- **HighLoad++ (YouTube, по-русски)**: доклады о реальной архитектуре высоконагруженных систем.

### Бесплатные: текст и интерактив
- **System Design Primer**: https://github.com/donnemartin/system-design-primer
- **Hello Interview**: бесплатные разборы задач и фреймворк для интервью. https://www.hellointerview.com/learn/system-design
- **Визуализация Raft**: http://thesecretlivesofdata.com/raft/ и https://raft.github.io
- **Задержки, которые надо знать (интерактив)**: https://colin-scott.github.io/personal_website/research/interactive_latency.html
- **Azure Architecture Center + Cloud Design Patterns**: https://learn.microsoft.com/azure/architecture/
- **Microsoft Learn**: learning paths и **бесплатные Practice Assessments** к AZ-104 и AZ-305.
- **AWS Skill Builder**: бесплатные Exam Prep Standard Course и Official Practice Question Set к SAA-C03.
- **AWS Well-Architected Framework**: https://aws.amazon.com/architecture/well-architected/
- **Excalidraw** (рисовать схемы): https://excalidraw.com
- **Habr**: хабы «Высокая производительность» и «Проектирование и рефакторинг».

### Платные (желательно купить)
- Martin Kleppmann, *Designing Data-Intensive Applications* (DDIA). Русское издание: «Высоконагруженные приложения». **Номера глав в плане даны по 1-му изданию.**
- Alex Xu, *System Design Interview*, тома 1 и 2.
- Практические тесты: Tutorials Dojo (AWS) или MeasureUp (Azure), около $15–20.

### Пробные собеседования
- Пробные собеседования друг с другом: бесплатные peer-платформы (например, Exponent, бывший Pramp) и знакомые инженеры.
- Для оплачиваемых пробных собеседований с инженерами FAANG: interviewing.io или Hello Interview (перед 23-й неделей, 1–2 штуки).

---

## 2. Повторяющийся шаблон практики (каждый Д6)

Каждую неделю: **одна задача за 45 минут вслух, на английском, со схемой в Excalidraw.**

1. Требования: функциональные и нефункциональные (5 мин).
2. Оценки на салфетке: QPS, объём хранения, пропускная способность (5 мин).
3. API и модель данных (5 мин).
4. Высокоуровневая схема (10 мин).
5. Deep dive в 1–2 узких места (15 мин).
6. Компромиссы и что сделали бы иначе (5 мин).

После этого сравните своё решение с эталонным разбором (Hello Interview, Alex Xu, System Design Primer). Запишите в `design-journal.md` три вещи, которые упустили.

---

## ФАЗА 1. Фундамент (недели 1–8)

### Неделя 1. Подход к задаче и оценки на салфетке
| День | Что делать |
|---|---|
| Д1 | Hello Interview: «Delivery Framework». System Design Primer: раздел «How to approach a system design interview question». |
| Д2 | Числа задержек (интерактив по ссылке выше) + Primer: «Powers of two», «Latency numbers». **Упражнение:** оцените QPS и объём хранения в год для Twitter при 200M DAU. |
| Д3 | Лекция Kleppmann №1 (Introduction). DDIA гл. 1: Reliable, Scalable, Maintainable. |
| Д4 | Дочитать DDIA гл. 1. **Упражнение:** сформулируйте SLI/SLO для одного из своих проектов (латентность p99, доступность). |
| Д5 | Лекция о масштабировании в Гарварде (ссылка в Primer, раздел «Scalability») или видео ByteByteGo о масштабировании от 0 до миллиона пользователей. |
| Д6 | **Задача: URL shortener (bit.ly)** по шаблону, затем сверка с Hello Interview. |

### Неделя 2. Модели данных и хранение
| День | Что делать |
|---|---|
| Д1 | DDIA гл. 2: реляционная, документная и графовая модели. |
| Д2 | DDIA гл. 3, первая половина: хеш-индексы, SSTable, LSM-деревья. |
| Д3 | DDIA гл. 3, вторая половина: B-деревья, OLTP и OLAP, колоночное хранение. Видео Hussein Nasser о B-tree и LSM. |
| Д4 | **Упражнение (C#):** append-only key-value хранилище с in-memory hash-индексом и компакцией (примерно 150 строк). |
| Д5 | SQL или NoSQL: когда что выбирать (Primer, раздел «Database»). Сравните Cosmos DB, DynamoDB, Cassandra и PostgreSQL по ключевым свойствам. |
| Д6 | **Задача: Pastebin** (Primer) + сравнение хранилищ. |

### Неделя 3. Сеть, API, балансировка
| День | Что делать |
|---|---|
| Д1 | DDIA гл. 4: форматы кодирования и эволюция схем (JSON, Protobuf, Avro). |
| Д2 | REST, gRPC, GraphQL, WebSocket, SSE, long polling (видео Hussein Nasser). |
| Д3 | Балансировщики L4 и L7, reverse proxy, API gateway, DNS, CDN (Primer). |
| Д4 | **Упражнение (.NET):** gRPC-сервис; добавьте поле в схему и проверьте обратную совместимость со старым клиентом. |
| Д5 | Rate limiting: token bucket, leaky bucket, sliding window. Изучите `System.Threading.RateLimiting` в ASP.NET Core. |
| Д6 | **Задача: распределённый rate limiter** (с Redis) по шаблону. |

### Неделя 4. Репликация
| День | Что делать |
|---|---|
| Д1 | Лекция Kleppmann №2 (Models of distributed systems). |
| Д2 | DDIA гл. 5: leader и follower, синхронная и асинхронная репликация, отставание реплик. |
| Д3 | DDIA гл. 5: multi-leader, leaderless, кворумы (W + R > N). Лекция Kleppmann №5 (Replication). |
| Д4 | **Упражнение:** PostgreSQL primary + replica в Docker. Измерьте отставание реплики и воспроизведите нарушение read-your-writes. |
| Д5 | Гарантии консистентности: read-your-writes, monotonic reads, consistent prefix. Опишите своими словами на английском (полстраницы). |
| Д6 | **Задача: распределённое key-value хранилище** (Alex Xu, т. 1, гл. 6 или аналог). |

### Неделя 5. Партиционирование и кэширование
| День | Что делать |
|---|---|
| Д1 | DDIA гл. 6: партиционирование по ключу и по хешу, горячие ключи, вторичные индексы. |
| Д2 | Consistent hashing, виртуальные узлы (видео ByteByteGo). |
| Д3 | **Упражнение (C#):** consistent hashing с виртуальными узлами. Измерьте, сколько ключей переезжает при добавлении узла. |
| Д4 | Стратегии кэширования: cache-aside, write-through, write-behind; инвалидация, TTL, cache stampede. |
| Д5 | Redis изнутри (обзор): структуры данных, персистентность, Cluster. Сопоставьте с Azure Cache for Redis и ElastiCache. |
| Д6 | **Задача: news feed / timeline** (fan-out on write или on read). |

### Неделя 6. Транзакции и распределённые бизнес-процессы
| День | Что делать |
|---|---|
| Д1 | DDIA гл. 7: ACID, уровни изоляции, аномалии (lost update, write skew). |
| Д2 | Snapshot isolation и serializable. **Упражнение:** воспроизведите write skew в PostgreSQL двумя сессиями. |
| Д3 | Паттерны Outbox и Inbox, Saga (хореография и оркестрация), идемпотентность и idempotency keys. |
| Д4 | **Упражнение (.NET):** Outbox + RabbitMQ (вручную или через MassTransit), идемпотентный потребитель. |
| Д5 | Azure Architecture Center: Cloud Design Patterns — Saga, Compensating Transaction, Retry, Circuit Breaker. |
| Д6 | **Задача: платёжная система или Ticketmaster** (бронирование мест без двойной продажи). |

### Неделя 7. Сбои, время, консенсус
| День | Что делать |
|---|---|
| Д1 | DDIA гл. 8: ненадёжные сети и часы, паузы процессов, fencing tokens. |
| Д2 | Лекции Kleppmann №3 (Time, clocks) и №4 (Broadcast). |
| Д3 | DDIA гл. 9: линеаризуемость, CAP, PACELC. |
| Д4 | Raft: интерактив thesecretlivesofdata + лекция MIT 6.824 о Raft. Лекция Kleppmann №6 (Consensus). |
| Д5 | **Упражнение:** на английском объясните одностраничным текстом, как Raft выбирает лидера и почему нужен кворум. Потом расскажите это вслух за 3 минуты. |
| Д6 | **Задача: распределённый планировщик задач или сервис блокировок.** |

### Неделя 8. Потоки данных и observability. Контрольная точка
| День | Что делать |
|---|---|
| Д1 | DDIA гл. 11: логи сообщений (Kafka), CDC, event sourcing. |
| Д2 | Kafka, RabbitMQ, Azure Service Bus, Event Hubs: когда что выбирать. Семантика at-least-once и exactly-once. |
| Д3 | DDIA гл. 10 (обзорно): batch-обработка, MapReduce. CQRS. |
| Д4 | Observability: логи, метрики, трейсы, OpenTelemetry. Сформулируйте, как бы вы объясняли свой опыт с Loki и Tempo на собеседовании. |
| Д5 | Повторите заметки из `design-journal.md` за 7 недель. |
| Д6 | **Первое пробное собеседование с партнёром** (на английском). Задача: ad click aggregator или top-K. |

---

## ФАЗА 2. Azure Solutions Architect Expert (недели 9–16)

**Материалы:** learning paths на Microsoft Learn, John Savill (AZ-104 Master Class и AZ-305 Study Cram), бесплатные Practice Assessments.
**Лабораторные:** бесплатный аккаунт Azure (стартовый кредит) или песочницы Microsoft Learn. **Ставьте лимиты бюджета (Budgets + alerts) и удаляйте ресурсы после лабораторных.**

### Неделя 9. AZ-104: идентичность и governance
| День | Что делать |
|---|---|
| Д1 | Запишитесь на AZ-104 через 4 недели: дедлайн дисциплинирует. MS Learn: Entra ID — пользователи, группы, лицензии. |
| Д2 | RBAC, кастомные роли, scope. **Лабораторная:** роль с минимальными правами. |
| Д3 | Azure Policy, management groups, теги, блокировки ресурсов. |
| Д4 | Подписки и стоимость: Cost Management, Budgets. John Savill: соответствующие главы. |
| Д5 | Первый Practice Assessment на MS Learn, разбор ошибок. |
| Д6 | **Задача System Design: чат (WhatsApp)** + сопоставление компонентов с сервисами Azure. |

### Неделя 10. AZ-104: хранилища и вычисления
| День | Что делать |
|---|---|
| Д1 | Storage accounts: уровни, репликация (LRS, ZRS, GRS, GZRS), жизненный цикл. |
| Д2 | SAS, приватные endpoints, Azure Files, AzCopy. **Лабораторная.** |
| Д3 | VM, availability sets и availability zones, VM Scale Sets. |
| Д4 | App Service, Container Instances, Container Apps, основы AKS. |
| Д5 | ARM и Bicep. **Лабораторная:** разверните App Service + Storage через Bicep. |
| Д6 | **Задача: Dropbox / file sync.** |

### Неделя 11. AZ-104: сеть
| День | Что делать |
|---|---|
| Д1 | VNet, подсети, NSG, ASG, peering. |
| Д2 | VPN Gateway, ExpressRoute (обзор), User-Defined Routes. |
| Д3 | Load Balancer, Application Gateway и WAF, Front Door, Traffic Manager: сравнительная таблица. |
| Д4 | Private DNS, Private Link, service endpoints. **Лабораторная:** hub-spoke из двух VNet. |
| Д5 | Practice Assessment №2, разбор ошибок. |
| Д6 | **Задача: YouTube / video streaming** (CDN, транскодинг). |

### Неделя 12. AZ-104: мониторинг, backup, экзамен
| День | Что делать |
|---|---|
| Д1 | Azure Monitor, Log Analytics (основы KQL), алерты. |
| Д2 | Azure Backup, Site Recovery. |
| Д3 | Повторение слабых доменов по результатам Practice Assessment. |
| Д4 | Полный пробный тест (MeasureUp или бесплатный), цель — больше 80%. |
| Д5 | Лёгкое повторение и отдых. |
| Д6 | **Экзамен AZ-104.** Обновите резюме и LinkedIn, начинайте откликаться на вакансии. |

### Неделя 13. AZ-305: identity, governance, мониторинг
| День | Что делать |
|---|---|
| Д1 | Запишитесь на AZ-305 через 4 недели. Изучите Well-Architected Framework: 5 столпов. |
| Д2 | Проектирование identity: Entra ID, B2B и B2C (External ID), managed identities, Key Vault. |
| Д3 | Проектирование governance и мониторинга для организации: landing zones (Cloud Adoption Framework). |
| Д4 | John Savill: AZ-305 Study Cram, первая часть. |
| Д5 | **Упражнение:** напишите ADR «Выбор механизма аутентификации для B2C-приложения», 1 страница на английском. |
| Д6 | **Задача: Uber / сервис на основе геолокации** (гео-индекс, геохэш). |

### Неделя 14. AZ-305: данные
| День | Что делать |
|---|---|
| Д1 | Выбор хранилища: Azure SQL, SQL Managed Instance, Cosmos DB, PostgreSQL Flexible. |
| Д2 | Cosmos DB: partition key, уровни консистентности (свяжите с неделей 4), RU. |
| Д3 | Интеграция данных: Data Factory, Synapse и Fabric (обзор), Event Hubs, Stream Analytics. |
| Д4 | Интеграция приложений: Service Bus, Event Grid, API Management, Logic Apps. |
| Д5 | Practice Assessment AZ-305 №1. |
| Д6 | **Задача: поисковый автокомплит (typeahead).** |

### Неделя 15. AZ-305: непрерывность бизнеса и инфраструктура
| День | Что делать |
|---|---|
| Д1 | RPO и RTO, стратегии DR, multi-region: active-active и active-passive. |
| Д2 | Высокая доступность для SQL и Cosmos DB, георепликация. |
| Д3 | Вычисления: VM, App Service, Functions, Container Apps, AKS — дерево решений из Architecture Center. |
| Д4 | Сеть: hub-spoke, Virtual WAN, Front Door или Application Gateway. Миграции (Azure Migrate). |
| Д5 | **Упражнение:** спроектируйте multi-region архитектуру для своего проекта (схема + оценка стоимости в Pricing Calculator). |
| Д6 | **Задача: web crawler.** |

### Неделя 16. AZ-305: экзамен
| День | Что делать |
|---|---|
| Д1 | Разбор кейсов (case studies — формат экзамена). |
| Д2 | Practice Assessment №2, повторение слабых доменов. |
| Д3 | John Savill: AZ-305 Study Cram, вторая часть. |
| Д4 | Полный пробный тест, цель — больше 80%. |
| Д5 | Отдых. |
| Д6 | **Экзамен AZ-305 → Azure Solutions Architect Expert.** Добавьте бейдж Credly в LinkedIn. |

---

## ФАЗА 3. AWS Solutions Architect Associate (недели 17–22)

**Материалы:** курс freeCodeCamp (Andrew Brown) по SAA-C03, AWS Skill Builder (бесплатные Exam Prep и Official Practice Question Set), тесты Tutorials Dojo (платные, лучшие).
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
| Д1 | Запишитесь на SAA-C03 через 6 недель. Создайте аккаунт AWS Free Tier + **Budgets с алертом на $5**. Изучите IAM: пользователи, роли, политики, STS. |
| Д2 | Организации AWS, SCP, IAM Identity Center. |
| Д3 | VPC: подсети, route tables, IGW, NAT Gateway, SG и NACL. |
| Д4 | **Лабораторная:** VPC с публичной и приватной подсетью, EC2 в приватной, доступ через SSM. |
| Д5 | VPC peering, Transit Gateway, VPC endpoints, PrivateLink. |
| Д6 | **Задача: notification service** (push, email, SMS) + отображение на сервисы AWS. |

### Неделя 18. Вычисления и хранилища
| День | Что делать |
|---|---|
| Д1 | EC2: типы инстансов, модели покупки (On-Demand, Spot, RI, Savings Plans). |
| Д2 | ELB (ALB, NLB), Auto Scaling. **Лабораторная:** ALB + ASG. |
| Д3 | S3: классы хранения, жизненный цикл, репликация, шифрование, presigned URL. |
| Д4 | EBS, EFS, FSx, Storage Gateway: когда что выбирать. |
| Д5 | Lambda, API Gateway, ECS/Fargate, EKS (обзор). |
| Д6 | **Задача: Google Docs / совместное редактирование** (OT или CRDT; лекция Kleppmann №8). |

### Неделя 19. Базы данных и интеграция
| День | Что делать |
|---|---|
| Д1 | RDS, Aurora (Multi-AZ и read replicas — разница!), RDS Proxy. |
| Д2 | DynamoDB: ключи, GSI и LSI, capacity modes, DAX, Streams. |
| Д3 | ElastiCache, Redshift, Athena (обзор). |
| Д4 | SQS (standard и FIFO), SNS, EventBridge, Kinesis, Step Functions. |
| Д5 | Первый тест из Official Practice Question Set, разбор ошибок. |
| Д6 | **Задача: система бронирования отелей.** |

### Неделя 20. Устойчивость и безопасность
| День | Что делать |
|---|---|
| Д1 | Route 53: политики маршрутизации, CloudFront, Global Accelerator. |
| Д2 | Стратегии DR на AWS: backup & restore, pilot light, warm standby, multi-site. |
| Д3 | KMS, Secrets Manager, WAF, Shield, GuardDuty, Cognito. |
| Д4 | CloudWatch, CloudTrail, Config. |
| Д5 | Тест Tutorials Dojo №1, разбор ошибок. |
| Д6 | **Задача: metrics / monitoring system** (time-series хранилище). |

### Неделя 21. Стоимость и Well-Architected
| День | Что делать |
|---|---|
| Д1 | AWS Well-Architected: 6 столпов (сравните с 5 столпами Azure). |
| Д2 | Оптимизация стоимости: Cost Explorer, выбор классов хранения, Spot. |
| Д3 | Миграция: DMS, DataSync, Snow family (обзор). |
| Д4 | Тест Tutorials Dojo №2. |
| Д5 | Повторение слабых доменов. |
| Д6 | **Второе пробное собеседование** (желательно с незнакомым человеком). |

### Неделя 22. Экзамен SAA-C03
| День | Что делать |
|---|---|
| Д1 | Тест Tutorials Dojo №3. |
| Д2 | Разбор ошибок, повторение. |
| Д3 | Финальный тест, цель — больше 80%. |
| Д4 | Лёгкое повторение. |
| Д5 | Отдых. |
| Д6 | **Экзамен AWS SAA-C03.** |

---

## ФАЗА 4. Интенсив по собеседованиям и поиск работы (недели 23–26)

### Неделя 23. Задачи старшего уровня
| День | Что делать |
|---|---|
| Д1 | Multi-region и геораспределённые данные, Spanner (лекция Kleppmann №8, TrueTime). |
| Д2 | Эволюция монолита в микросервисы, strangler fig, границы сервисов (DDD bounded contexts). |
| Д3 | Задача на время: распределённый кэш. |
| Д4 | Задача на время: платёжный шлюз с exactly-once эффектом. |
| Д5 | Составьте 5 историй в формате STAR на английском: конфликт, провал, лидерство, сложное техническое решение, влияние на бизнес. |
| Д6 | **Платное пробное собеседование** с инженером FAANG (interviewing.io или Hello Interview). |

### Недели 24–26. Ритм «собеседование + отклики»
| День | Что делать |
|---|---|
| Д1 | 10 откликов (LinkedIn, Otta/Welcome to the Jungle, Hired-подобные, прямые обращения к рекрутерам). |
| Д2 | Задача System Design на время + самопроверка. |
| Д3 | Behavioral: прогон историй STAR вслух, запись на видео. |
| Д4 | Задача на время по разбору Hello Interview, которую ещё не решали. |
| Д5 | Кодинг-разминка (1–2 задачи LeetCode medium): продуктовые компании его тоже проверяют. |
| Д6 | Пробное собеседование с партнёром + ретроспектива по `design-journal.md`. |

---

## Упражнения на протяжении всего плана

- **Портфолио.** На каждые 4 недели — один ADR или design doc по своим проектам (выбор брокера, трассировка, аутентификация). Публикуйте их в GitHub-репозитории `architecture-notes` на английском. Такую ссылку можно положить в резюме.
- **Флеш-карточки** (Anki, бесплатно): числа задержек, лимиты сервисов, соответствия Azure ↔ AWS, уровни консистентности.
- **Английский.** Все упражнения на объяснение делайте вслух и на английском: собеседование по System Design — это в первую очередь коммуникация.
- **Статьи для глубины** (по одной в месяц): Dynamo (Amazon, 2007), Raft, Google Spanner, Kafka. Затем разбор в лекциях MIT 6.824.

## Опционально, после 26-й недели

- **iSAQB CPSA-F**, если целитесь в Германию, Австрию или Швейцарию.
- **AWS Solutions Architect Professional**, если цель — роль архитектора.
- Сравнение зарплат: levels.fyi (по городам и компаниям), Glassdoor.

## Контрольные точки

| Неделя | Критерий готовности |
|---|---|
| 8 | Решаете типовую задачу за 45 минут и объясняете компромиссы на английском |
| 12 | Сдан AZ-104, резюме обновлено, начаты отклики |
| 16 | Сдан AZ-305 (Azure Solutions Architect Expert) |
| 22 | Сдан AWS SAA-C03 |
| 26 | Минимум 6 пробных собеседований, 40+ откликов, есть первые технические собеседования |
