[< к содержанию](./README.md)

## git clean

Команда ***git clean*** в некоторой степени является командой отмены действия. Можно также сказать, что ***git clean*** дополняет другие команды, такие как ***git reset*** и ***git checkout***. Эти две команды нужны в работе с файлами, ранее добавленными в индекс отслеживания Git, в то время как ***git clean*** используется для операций с неотслеживаемыми файлами. Неотслеживаемые файлы — это файлы, которые созданы в рабочем каталоге репозитория, но еще не добавлены в индекс отслеживания репозитория с помощью команды ***git add***. 

---

Параметр *-n* запускает тестовый прогон команды ***git clean***. Этот прогон позволяет определить файлы, которые будут удалены, без фактического удаления. Рекомендуется всегда сначала выполнять тестовый прогон ***git clean***:

```bash=markdown
git clean -n
Would remove untracked_file
```

Параметр *force* инициирует фактическое удаление неотслеживаемых файлов из текущего каталога. Этот параметр является обязательным, если для параметра конфигурации *clean.requireForce* не установлено значение *false*. При этом не будут удалены неотслеживаемые папки или файлы, указанные в файле ***.gitignore***:

```bash=markdown
git clean -f
Would remove untracked_file
```

[< к содержанию](./README.md)