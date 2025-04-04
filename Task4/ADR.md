﻿### <a name="_b7urdng99y53"></a>**Название задачи: Открытие депозитов онлайн (MVP)** 
### <a name="_hjk0fkfyohdk"></a>**Автор: Давлетов Альберт**
### <a name="_uanumrh8zrui"></a>**Дата: 30.03.2025**
### <a name="_3bfxc9a45514"></a>**Функциональные требования**
Опишите здесь верхнеуровневые Use Cases. Их нужно оформить в виде таблицы с пошаговым описанием:

|**№**|**Действующие лица или системы**|**Use Case**|**Описание**|
| :-: | :- | :- | :- |
| 1 | Оператор кол-центра банка | Получить актуальные ставки по депозитам | 1. Оператор кол-центра банка должен иметь прямой доступ к актуальным условиям по депозитам.<br/>2. Оператор уведомляет клиента о текущих условиях. |
|   2   | Оператор партнерского кол-центра | Получить ставки по депозитам через файл, почту | 1. Партнерский кол-центр не имеет прямой доступ к системам банка.<br/>2. Партнерский кол-центр должен иметь актуальный файл с текущими условиями по депозитам.<br/> 3. Актуальные ставки по депозитам и условия банк должен отправлять партнерскому кол-центру раз в неделю. |
|   3   | Менеджер банка (бэк офис) | Отпавляет актуальные условия по депозитам партнерскому кол-центру | Менеджер банка на регулярной основе или по мере обновления условий по депозитам должен выгружать всю информацию и отправлять партнерскому кол-центру|

### <a name="_u8xz25hbrgql"></a>**Нефункциональные требования**
Опишите здесь нефункциональные требования и архитектурно-значимые требования.

|**№**|**Требование**|
| :-: | :- |
|   1   | Партнерский кол-центр всегда должен иметь актуальные данные по депозитам. |
|   2   | Если условия по депозитам содержат конфиденциальные данные, то файл нужно отправлять только по корпоративной почте и в зашифрованном виде. |
|   3   | Менеджер банка может только выгружать файл с условиями по депозитам и не может их изменить. |

### <a name="_qmphm5d6rvi3"></a>**Решение**

Смотри диаграмму решения.


### <a name="_bjrr7veeh80c"></a>**Альтернативы**

- Дополнительный сервис для партнерского кол-центра, где можно получить всю актуальную информацию по депозитам.
- Ручная выгрузка данных по депозитам в Excel файл и его отправка партнерскому кол-центру.

**Недостатки, ограничения, риски**

- Человеческий фактор при отправке актуальных данных по депозитам. Менеджер может отправить данные с задержкой или отправить неверные данные.
- Отправка данных по почте не является безопасным способом получения данных.


**Список крупных задач для будущего планирования**

1. Сервис для получения актуальных ставок. Нужен для кол-центра банка.

2. Документация и обновление скриптов для операторов кол-центра.

3. Реализовать функционал выгрузки актуальных ставок, условий по депозитам из АБС.

4. Создание еженедельной таски для менеджеров бэк-офиса по отправке актуальных ставок по депозитам партнерскому кол-центру.

5. Документация и обновление скриптов для операторов партнерского кол-центра.
