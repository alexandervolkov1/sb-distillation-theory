# Теория переноса паров сурьмы в водороде

Научный документ на Typst содержит постановку задачи, вывод уравнений модели CPIM, численный метод, транспортные коэффициенты и таблицы обозначений.

Текст перенесён из [теоретического отчёта проекта sb-distillation](https://github.com/alexandervolkov1/sb-distillation/blob/4784a763ff7d0c385fdeb27f44311637af7b2950/notebooks/sb_distillation/report.clj).

## Сборка

Проверено с Typst 0.14.2. Выполните команду в каталоге проекта.

```powershell
typst compile --font-path .\fonts main.typ
```

Результат сохраняется в `main.pdf`. Шрифты встраиваются в PDF. Файлы шрифтов и их лицензии находятся в каталоге `fonts/`.

## Шрифты

Первые две строки `main.typ` задают шрифты текста и формул. По умолчанию используются New Computer Modern и Old Standard Math.

```typst
#let body-font = "New Computer Modern"
#let math-font = "OldStandard-Math"
```

Для альтернативной пары замените эти строки на следующие.

```typst
#let body-font = "Old Standard"
#let math-font = "OldStandard-Math"
```

`OldStandard-Math` — имя семейства Old Standard Math, которое показывает `typst fonts --font-path .\fonts`.

В комплект входят оригинальные обычное и полужирное начертания New Computer Modern и Old Standard и один математический шрифт. Сведения о полном комплекте New Computer Modern 5.1 и его архиве приведены в [лицензии шрифта](fonts/NewComputerModern-GFL.txt).
