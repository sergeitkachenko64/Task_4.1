[< к содержанию](./README.md)

## git blame

Команда ***git blame*** — это универсальная утилита для устранения проблем. Она имеет множество вариантов применения. Общее назначение ***git blame*** — отображение метаданных автора, связанных со строками, которые были внесены в файл при коммите. Эта команда позволяет изучить определенные этапы изменений файла и узнать, кто внес последние изменения в строку. Таким образом можно проследить историю кода и выяснить, какой именно код был внесен в репозиторий, как это было сделано и по какой причине.

---

Команда ***git blame*** работает только на конкретных файлах, поэтому, чтобы получить полезный результат, нужно указать путь к файлу. Если выполнить ***git blame*** без настройки параметров, отобразится только меню справки по командам. В данном примере используется файл README.MD. Файл README принято размещать в корне репозитория Git проекта с открытым кодом в качестве источника документации по проекту.

```bash=markdown
git blame README.MD
```

[< к содержанию](./README.md)