================================================================
Repeating of math hyphenation mark in inline equations
(C) 2009-2010 Denis Ryabov.

Based on ideas and code from M.I.Grinchuk "TeX and Russian
                Traditions of Typesetting", TUGboat 17 (1996) 4.

CHANGELOG:
-------------------- 0.99 [**-*******-201*] --------------------
[#] don't hyphenate trailing mathsign (e.g. in $2+2=$)
[#] don't change redefined symbols (\le, \ge, \to, etc.)
-------------------- 0.98 [31-January-2010] --------------------
[+] hyphenation on :=
[+] correct work with 'icomma' package and option 'icomma' of
    'eulervm' package
[+] correct work with 'program' package
[+] symbols have been added from  boisik, euler, fourier,
    lucbmath, lucidabr, lucmin, lucmtime, luctime, mathbbol,
    mdwmath, sbbm, stmaryrd and wasysym packages.
[-] remove shrinking of space in math (breaked url package)
[#] don't hyphenate after punctuation (',', ';', '\colon' etc.)
[#] create broken commands as robust
[#] some fixes of redeclaring of AMS commands
[#] commented hyphenation on \ldots и \cdots, as TeX doesn't
    here by default
-------------------- 0.97 [08-October-2009] --------------------
[#] problem with operators like '+^\leq'
-------------------- 0.96 [29-September-2009] ------------------
[#] problem with '-' in AMS \DeclareMathOperator
[#] problem with \ldots in text mode
-------------------- 0.95 [28-September-2009] ------------------
[#] problem with sub/sup-scripts after relations
[+] hyphenation on \ldots
[+] AMS/Lucida left brackets (lvert, lVert, ulcorner, llcorner)
    support
[+] mathbbol.sty left bracket (Lbrack) support
[^] huge code refactoring
-------------------- 0.91 [21-September-2009] ------------------
[#] problem with space after brackets
-------------------- 0.90 [20-September-2009] ------------------
[!] first public release


KNOWN ISSUES:
expressions like $\sum -y$ require manual insertion of \nobr
before - (that is $\sum \nobr-y$)
expressions like $x+\ldots+y$ may be broken on pluses
'xy' package: should be loaded after 'rmathbr' to work properly
'breqn' package: cannot work together with 'rmathbr'
================================================================

Перенос строчных формул в русском стиле (с дублированием знаков)
(C) 2009-2010 Денис Рябов.

Основано на идеях и коде из M.I.Grinchuk "TeX and Russian
                Traditions of Typesetting", TUGboat 17 (1996) 4.

ИЗМЕНЕНИЯ:
-------------------- 0.99 [** ******* 201*] --------------------
[#] не переносить стоящий в конце формулы знак операции
    (как, например, в $2+2=$)
[#] не менять переопределенные символы (\le, \ge, \to и др.)
-------------------- 0.98 [31 января 2010] ---------------------
[+] перенос на :=
[+] корректная работа с опцией icomma пакета eulervm и пакетом
    icomma
[+] корректная работа с пакетом program
[+] добавлены символы из пакетов boisik, euler, fourier,
    lucbmath, lucidabr, lucmin, lucmtime, luctime, mathbbol,
    mdwmath, sbbm, stmaryrd и wasysym
[-] убрано уменьшение пробелов в математических формулах
    (нарушало работу пакета url)
[#] не делать переносы после знаков пунктуации , ; \colon и др.
[#] переносимые команды создаются как крепкие
[#] исправлено объявление некоторых AMS-команд
[#] перенос на \ldots и \cdots закомментирован, т.к. TeX на них
    по-умолчанию не переносит
-------------------- 0.97 [08 октября 2009] --------------------
[#] решена проблема с операторами типа '+^\leq'
-------------------- 0.96 [29 сентября 2009] -------------------
[#] решена проблема с '-' в AMS \DeclareMathOperator
[#] решена проблема с \ldots в текстовой моде
-------------------- 0.95 [28 сентября 2009] -------------------
[#] решена проблема с над- и подстрочными индексами после знаков
[+] перенос на \ldots
[+] учитываются открывающие скобки из AMS/Lucida (lvert, lVert,
    ulcorner, llcorner)
[+] учитываются открывающие скобки из mathbbol.sty (Lbrack)
[^] код пакета в значительной степени переработан
-------------------- 0.91 [21 сентября 2009] -------------------
[#] решена проблема с отступами после скобок
-------------------- 0.90 [20 сентября 2009] -------------------
[!] первая публичная версия


ИЗВЕСТНЫЕ ПРОБЛЕМЫ:
в выражениях типа $\sum -y$ нужно вручную вставлять \nobr
перед - (то есть писать $\sum \nobr-y$)
в выражениях типа $x+\ldots+y$ разрешены переносы на +
пакет xy: для корректной работы должен загружать после rmathbr
пакет breqn: не может работать совместно с rmathbr
================================================================