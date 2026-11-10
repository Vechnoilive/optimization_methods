# ЛР № 1. Смешение углей для ТЭС

Вариант 14. Нужно закупить 1000 т угля у пяти поставщиков. Ищу самый дешёвый план, который укладывается в нормы по зольности и сере.

[Открыть в Colab](https://colab.research.google.com/github/Vechnoilive/optimization_methods/blob/main/lr1/lr1.ipynb) · [Отчёт](LR1_V14_Zarechkin.pdf) · [Отчёт по звёздочке](Star1_LR1_Elastic_Filter_V14.pdf)

В Colab выбери **Среда выполнения → Выполнить всё**. Первая ячейка ставит зависимости. Если Colab попросит перезапустить сеанс, запусти ячейки заново.

Цены, лимиты, зольность и содержание серы получены небольшим случайным разбросом от шаблона. Данные лежат в `data.json`. Seed генерации — `10011`. В `results` лежат планы, сценарии, проверки и лог HiGHS контрольного прогона. Результаты звёздочки лежат в `results/star`.

## Локальный запуск

Из корня репозитория в Python 3.12.

```bash
python -m pip install -r requirements.txt jupyter nbconvert
jupyter nbconvert --to notebook --execute --stdout lr1/lr1.ipynb > lr1_executed.ipynb
```
