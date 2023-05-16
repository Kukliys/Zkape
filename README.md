# Zkape


## На выбор предоставлено 4 режима работы:
- 1 - Check eligibility
- 2 - Clime tokens $ZAT
- 3 - Swap $ZAT to $ETH
- 4 - Clime tokens and swap to $ETH (SyncSwap)

Для режима работы 1 время между запуском аккаунтов составляет 1 секунду.

Для режимов работы 2-4, в файле `config.txt` прописывается интервал между запуском акканутов в секундах:
`interval = 10,30`

В 4м режиме работы время между клеймом токенов и свопом может составить от 90 до 180 секунд. Если такое время вас не устраивает необходимо самостоятельно поменять время в файле `zkape.py` в строках кода 169 и 376 на желаемые.  

При обычной загруженности сети ETH для 4го режима работы потребуется ~0.002 - 0.003 $ETH.

### Потоки
В каждом из режимов предусмотрена возможность использования потоков для ускорения работы.
Если количество прокси не совпадает с количеством приватных ключей, для работы будет использоваться первая прокси из `proxy.txt` и обычный режим работы (без потоков).  

**Для работы с потоками необходимо равенство количества прокси и количества приватных ключей.**  

При работе с локального IP программа работает в обычном режиме(без потоков).


#### Формат прокси:
`login,password@ip,port`


## !
Используя консоль, необходимо в директории со скриптом установить необходимые для работы библиотеки, при помощи команды `pip install requirements.txt`
