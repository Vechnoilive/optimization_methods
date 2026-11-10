# ЛР № 2. Переброска пустых контейнеров

Вариант 11. В трёх портах есть лишние пустые контейнеры, а трём другим их не хватает. Ищу самый дешёвый способ перевезти контейнеры с учётом лимитов маршрутов.

[Открыть в Colab](https://colab.research.google.com/github/Vechnoilive/optimization_methods/blob/main/lr2/lr2.ipynb) · [Отчёт](LR2_V11_Zarechkin.pdf) · [Отчёт по звёздочке](Star2_LR2_Dual_Model.pdf)

В Colab выбери **Среда выполнения → Выполнить всё**. Первая ячейка устанавливает зависимости. Если Colab попросит перезапустить сеанс, запусти ячейки заново.

Данные лежат в `data.json`. Балансы портов и маршруты взяты из шаблона. Разброс добавлен только к тарифам и пропускным способностям. Если файла нет, ноутбук создаст его с `seed=10012`. Планы, сценарии, проверки и лог HiGHS сохраняются в `results`.
Файлы задания со звёздочкой сохраняются в `results/star`.

## Локальный запуск

Из корня репозитория в Python 3.12.

```bash
python -m pip install -r requirements.txt jupyter nbconvert
jupyter nbconvert --to notebook --execute --stdout lr2/lr2.ipynb > lr2_executed.ipynb
```
