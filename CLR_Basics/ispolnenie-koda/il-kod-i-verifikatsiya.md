# IL-код и верификация 

IL - стековый язык \(все интсрукции заносят операнды в исполнительный стек и извлекают результаты оттуда же\)

IL-код обеспечивает безопасность приложения и его устойчивать перед ошибками \(главный плюс\)

В процессе компиляции IL в машинные инструкции, CLR выполняет процедуру, называемую **верификацией**

* Верификация - анализ высокоуровневого кода IL и проверка безопасности всех операций

CLR предоставляет возможность выполнения нескольких управляемых приложений в одном процессе ОС, что улучшает производительность, уменьшает затраты ресурсов и обеспечивает тот же уровень защиты.

В Winows каждый процесс обладает собственным вирт. адресом, т.к приложение может считать данные или записать их по недопустимому адресу. Всё делается так, чтобы один процесс не мог повредить другому. Каждый управляемый EXE файл работает в отдельном адресном пространстве, состоящем из одного домена.

**AppDomain - **домен приложений, там выполняется каждое управляемое приложение.







