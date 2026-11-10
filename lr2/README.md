# ЛР № 2. Балансировка такси по зонам города

Вариант 14. В четырёх зонах есть свободные машины, а в четырёх других их не хватает. Ищу самый дешёвый способ выровнять баланс с учётом лимитов маршрутов.

[Открыть в Colab](https://colab.research.google.com/github/Vechnoilive/optimization_methods/blob/main/lr2/lr2.ipynb) · [Отчёт](LR2_V14_Zarechkin.pdf) · [Отчёт по звёздочке](Star2_LR2_Dual_Model_V14.pdf)

В Colab выбери **Среда выполнения → Выполнить всё**. Первая ячейка ставит зависимости. Если Colab попросит перезапустить сеанс, запусти ячейки заново.

Балансы и направления взяты из шаблона. Тарифы и ёмкости маршрутов немного меняются при генерации. Данные лежат в `data.json`. Seed генерации — `10011`. В `results` лежат планы, сценарии, проверки и лог HiGHS контрольного прогона. Результаты звёздочки лежат в `results/star`.

## Локальный запуск

Из корня репозитория в Python 3.12.

```bash
python -m pip install -r requirements.txt jupyter nbconvert
jupyter nbconvert --to notebook --execute --stdout lr2/lr2.ipynb > lr2_executed.ipynb
```
