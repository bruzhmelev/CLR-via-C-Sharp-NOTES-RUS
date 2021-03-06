# Управляемые моудли

Вне зависимости от типа компилятора, результатом будет **управляемый модуль**

**УМ **-** **стандартный переносимый исполняемый \(portable executable, PE\) файл 32-разрядной \(PE32\) или 64-разрядной Windows \(PE32+\), который требует для своего выполнения CLR.

![](/assets/Компиляция.исходного.кода.в.управляемые.модули.png)Компиляция исходного кода в управляемые модули

### Части управляемого модуля

1. **Заголовок PE32 или PE32+** - обозначает тип файла: GUI, CUI, DLL; имеет временную метку \(когда файл был собран\) PE -32 файл выполняется в 32-ух и 64-ёх разрядных системах, PE32+ - только в 64-ёх разр.

2. **Заголок CLR** - cодержит информацию \(интерпретируемую CLR и утилитами\), которая превращает этот модуль в управляемый. Заголовок включает нужную версию CLR, некоторые флаги, метку метаданных MethodDef точки входа в управляемый модуль \(метод Main\), а также месторасположение/размер метаданных модуля, ресурсов, строгого имени, некоторых флагов и пр.

3. **Метаданные**  - каждый управляемый модуль содержит таблицы метаданных. Есть два основных вида таблиц — это таблицы, описывающие типы данных и их члены, определенные в исходном коде, и таблицы, описывающие типы данных и их члены, на которые имеются ссылки в исходном коде

4. **Код IL \(Intermediate Language\)** - rод, создаваемый компилятором при компиляции исходного кода. Впоследствии CLR компилирует IL в машинные команды

   ---



