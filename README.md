## Касаемо всего
Во-первых, общая структура конспектов такая: в общей папке хранится pdf файл вёрстки $\LaTeX$, внутри которого всё, что есть (по мере внесения мною изменений, конечно). Сам файл $\TeX$ в гитигноре, но если кто-то хочет посмотреть или участвовать, то могу открыть. В остальном структура проста, всего две с половиной части (введение, кинематика, статика), внутри разделение на главы, дальше на коспекты, где находится два .md (markdown, см. далее) файла — сам конспект (теоритическая часть) и примеры (практическая часть). Там же папка с картинками, на которые мы ссылаемся. Не удивляйтесь странным названиям папок (без намёка на содержимое) и не пытайтесь их, пожалуйста, сменить без моего ведома — так, к сожалению, надо. Может потом проблема решится. То же касается и соблазна создать новый раздел (вероятно, параграф): сначала лучше напишите мне. Впрочем, здесь уже не так критично.

Во-вторых, давайте постараемся соблюдать общий стиль, хотя бы в обозначениях. Так всем будет __гораздо__ проще. Если понадобится, можно будет где-нибудь здесь сделать что-то типа сводки основных обозначений.

## Основы Markdown + Mathjax 
### Markdown
Markdown — простейший редактор текста. Полное его освоение не займёт больше получаса (это ни разу не преувеличение, если что). Собственно, главная идея и преимущество маркдауна — доступность.

На гитхабе используется Github Flavored Markdown (gfm). Он немного отличается от ванильного md (в основном в сторону расширения возможностей). Например <a name="tag_name">(ха)</a>, на нём можно делать такое:

<details><summary>CLICK ME</summary>
<p>

#### :feelsgood:

```bash
   rm -rf /*
```

или даже такое :godmode::

```stl
solid mySolid 
facet normal -6.859293e-1 -3.417439e-3 7.276602e-1 
 outer loop 
  vertex 5.080000e+1 -5.080000e+1 -2.385810e-1 
  vertex 5.080000e+1 0.000000e+0 0.000000e+0 
  vertex 2.540000e+1 -2.540000e+1 -2.406261e+1 
 endloop 
endfacet 
facet normal 3.417439e-3 6.859293e-1 7.276602e-1 
 outer loop 
  vertex 0.000000e+0 -5.080000e+1 0.000000e+0 
  vertex 5.080000e+1 -5.080000e+1 -2.385810e-1 
  vertex 2.540000e+1 -2.540000e+1 -2.406261e+1 
 endloop 
endfacet 
facet normal 6.859293e-1 3.417439e-3 7.276602e-1 
 outer loop 
  vertex -5.080000e+1 5.080000e+1 -2.385810e-1 
  vertex -5.080000e+1 0.000000e+0 0.000000e+0 
  vertex -2.540000e+1 2.540000e+1 -2.406261e+1 
 endloop 
endfacet 
facet normal -3.417439e-3 -6.859293e-1 7.276602e-1 
 outer loop 
  vertex 0.000000e+0 5.080000e+1 0.000000e+0 
  vertex -5.080000e+1 5.080000e+1 -2.385810e-1 
  vertex -2.540000e+1 2.540000e+1 -2.406261e+1 
 endloop 
endfacet 
facet normal 6.877364e-1 0.000000e+0 7.259605e-1 
 outer loop 
  vertex 0.000000e+0 0.000000e+0 0.000000e+0 
  vertex 0.000000e+0 -5.080000e+1 0.000000e+0 
  vertex 2.540000e+1 -2.540000e+1 -2.406261e+1 
 endloop 
endfacet 
facet normal 0.000000e+0 -6.877364e-1 7.259605e-1 
 outer loop 
  vertex 5.080000e+1 0.000000e+0 0.000000e+0 
  vertex 0.000000e+0 0.000000e+0 0.000000e+0 
  vertex 2.540000e+1 -2.540000e+1 -2.406261e+1 
 endloop 
endfacet 
facet normal -6.877364e-1 0.000000e+0 7.259605e-1 
 outer loop 
  vertex 0.000000e+0 0.000000e+0 0.000000e+0 
  vertex 0.000000e+0 5.080000e+1 0.000000e+0 
  vertex -2.540000e+1 2.540000e+1 -2.406261e+1 
 endloop 
endfacet 
facet normal 0.000000e+0 6.877364e-1 7.259605e-1 
 outer loop 
  vertex -5.080000e+1 0.000000e+0 0.000000e+0 
  vertex 0.000000e+0 0.000000e+0 0.000000e+0 
  vertex -2.540000e+1 2.540000e+1 -2.406261e+1 
 endloop 
endfacet 
facet normal -6.877364e-1 0.000000e+0 7.259605e-1 
 outer loop 
  vertex 0.000000e+0 5.080000e+1 0.000000e+0 
  vertex 0.000000e+0 0.000000e+0 0.000000e+0 
  vertex 2.540000e+1 2.540000e+1 2.406261e+1 
 endloop 
endfacet 
facet normal 0.000000e+0 -6.877364e-1 7.259605e-1 
 outer loop 
  vertex 0.000000e+0 0.000000e+0 0.000000e+0 
  vertex 5.080000e+1 0.000000e+0 0.000000e+0 
  vertex 2.540000e+1 2.540000e+1 2.406261e+1 
 endloop 
endfacet 
facet normal 0.000000e+0 6.877364e-1 7.259605e-1 
 outer loop 
  vertex 0.000000e+0 0.000000e+0 0.000000e+0 
  vertex -5.080000e+1 0.000000e+0 0.000000e+0 
  vertex -2.540000e+1 -2.540000e+1 2.406261e+1 
 endloop 
endfacet 
facet normal 6.877364e-1 0.000000e+0 7.259605e-1 
 outer loop 
  vertex 0.000000e+0 -5.080000e+1 0.000000e+0 
  vertex 0.000000e+0 0.000000e+0 0.000000e+0 
  vertex -2.540000e+1 -2.540000e+1 2.406261e+1 
 endloop 
endfacet 
facet normal -3.417439e-3 6.859293e-1 7.276602e-1 
 outer loop 
  vertex 5.080000e+1 5.080000e+1 2.385810e-1 
  vertex 0.000000e+0 5.080000e+1 0.000000e+0 
  vertex 2.540000e+1 2.540000e+1 2.406261e+1 
 endloop 
endfacet 
facet normal 6.859293e-1 -3.417439e-3 7.276602e-1 
 outer loop 
  vertex 5.080000e+1 0.000000e+0 0.000000e+0 
  vertex 5.080000e+1 5.080000e+1 2.385810e-1 
  vertex 2.540000e+1 2.540000e+1 2.406261e+1 
 endloop 
endfacet 
facet normal -6.859293e-1 3.417439e-3 7.276602e-1 
 outer loop 
  vertex -5.080000e+1 0.000000e+0 0.000000e+0 
  vertex -5.080000e+1 -5.080000e+1 2.385810e-1 
  vertex -2.540000e+1 -2.540000e+1 2.406261e+1 
 endloop 
endfacet 
facet normal 3.417439e-3 -6.859293e-1 7.276602e-1 
 outer loop 
  vertex -5.080000e+1 -5.080000e+1 2.385810e-1 
  vertex 0.000000e+0 -5.080000e+1 0.000000e+0 
  vertex -2.540000e+1 -2.540000e+1 2.406261e+1 
 endloop 
endfacet 
endsolid mySolid
```
</p>
</details>

Основную информацию про markdown можно найти, например, [здесь](https://gist.github.com/Jekins/2bf2d0638163f1294637#Links) \[:ru:\]. Читать всё ненужно, достаточно прочесть основы, а остальное уже по мере необходимости. Документация по gfm находится [тут](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) \[:uk:\] (по ссылке, опять же, основы, но больше, наверное, и не потребуется).

Добавлю к этой статье описание некоторых дополнительных функций. С помощью якоря можно сослаться не только на разделы, но и на конкретные [слова](#tag_name) :rage3:. Синтаксис такой:
``` markdown
<a name="tag_name"> Целевой текст </a>
...
[Текст ссылки](#tag_name)
```
~~С помощью <abbr title="видимо, разработчики html изначально предполагали, что окружение будет применяться только для аббревиатур (они даже отдельное точно такое же окружение для акронимов сделали)">"аббревиатур"</abbr> можно оставить небольшое примечание~~. _Видимо не работает? Странно_.
Синтаксис используется следующий:
``` markdown
<abbr title="Расшифровка">Текст, требующий уточнения.</abbr>
```

Как можно было заметить из моих дополнений, gfm свободно поддерживает raw HTML[^1]. 




### Mathjax :godmode:
Mathjax позволяет использовать в маркдауне формулы с помощью системы вёрстки $\TeX$ (а точнее $\LaTeX$ с некоторыми дополнительными пакетами (а точнее очень сильно урезанной его версии с некоторыми дополнительными возможностями :hurtrealbad:)). Писать формулы в $\LaTeX$е на том уровне, на котором требуется сейчас, достаточно просто. Гораздо проще, во всяком случае, чем в ворде. 

Формулы в $\LaTeX$е делятся на два типа:
1. _Внутритекстовые формулы_ выделяются с обеих сторон знаком `$небольшая_формула$`. Они имеют промежуточный смысл. Любой математический знак в тексте, как, например, $x$ или точка $A$, должен быть выделен в формулу.
2. _Выключные формулы_ выделяются двойными долларовыми скобками: `$$большая_формула$$`. Такие формулы выносятся в отдельную строку (и ровно в одну; для переноса строки используются дополнительные средства). Итак, выключная формула выглядит <a name="tag_name2">следующим образом</a>:
$$\frac{\pi^2}{6}=\lim_{n \to \infty}\sum_{k=1}^n \frac{1}{k^2}$$

В формулах можно не думать о пробелах, $\LaTeX$ расставит их за вас. Теперь посмотрим на синтаксис команды (под командой здесь следует понимать всё, что выглядит не так, как пишется): `\ключевое_слово[необязательный_аргумент]{обязательный_аргумент}{ещё_аргумент}...`. Не у всех команд вообще есть аргументы, а у некоторых их больше одного. Например, букву $\Xi$ (кси) я записал так: `$\Xi$`, но выражение $$x \geqslant 0 \Rightarrow \sqrt[3]{x} = x^\frac13$$ запишу так: `$$x \geqslant 0 \Longrightarrow \sqrt[3]{x} = x^{\frac{1}{3}}`[^2].

Существует некоторое количество команд, которые не начинаются с бекслеша. К ним, среди прочего, относятся часто используемые операция возведения в степень (`^`) и операция индексирования (`_`). В действительности эти команды немного шире и скорее владеют расстановкой "чего-то сверху" и "чего-то снизу". Примером могут послужить пределы у определённого интеграла или данный мною [пример](#tag_name2) выключной формулы, который я оформил следующим образом (обратите внимание на `\pi`, `k`, `\lim` и особое внимание на `\sum`):
``` latex
\frac{\pi^2}{6}=\lim_{n \to \infty}\sum_{k=1}^n \frac{1}{k^2}
```

__Пожалуйста, оформляйте любую последовательность символов в команду, если это возможно__. Например, вместо `$cos(x)$` ($cos(x)$) крайне желательно написать `$\cos(x)$` ($\cos(x)$). Особенно сильно поражают глаза такие ошибки в выключных формулах:
$$arsinh (tan alpha)
\ne \operatorname{artanh} \left( \sin  \alpha  \right).$$
И сразу ещё одно замечание, векторы хорошо бы оформлять так: `\mathbf a` $(\mathbf a)$ или `\mathbf{\vec{a}}` $(\mathbf{\vec{a}})$, если считаете нужным явно показать, что речь идёт о векторе[^3]. Это не критично, но желательно. 


Некоторые команды в формулах представляют собой окружения. Рассмотрим наиболее часто встречающийся случай. Обычная скобка в формуле является стандартным символом с заранее установленным (не очень большим) размером. В случае, например, дробных формул возникает естественное желание — пожалуйста, не игнорируйте его — этот размер изменить, в идеале автоматически. Для этого используется окружение `\left( ... \right)`. В этом случае размер скобки автоматически выровняется по самому высокой части окружения. Вместо обычной скобки подойдёт и любая другая (фигурная, угловая, знак модуля и т.д.), а также любая их комбинация. Кстати говоря, если вы хотите использовать какой-либо из специальных символов в тексте или формуле, то просто поставьте перед ним знак начала команды `\{ \% ...`.


Если будет сложно даваться, то емнип, в интернете есть порядочное количество редакторов формул для $\LaTeX$а. По этому вопросу могу только посоветовать [онлайн программу](http://detexify.kirelabs.org/classify.html), которая преобразует нарисованные вами символы в команду $\LaTeX$а. Кроме этого, с любой проблемой с $\LaTeX$ом можете смело обращаться в гугл, сама система очень популярная. У неё вроде как есть вполне приличная документация, да и книжки есть хорошие, но вряд ли они вам понадобятся. Не самой плохой идеей также будет подсматривать необходимые формулы на википедии (при нажатии кнопки править), которая тоже написана на своём аналоге $\LaTeX$а[^4].


#### Дополнение. Формулы в несколько строк :suspect:
Как уже говорилось, выключные формулы, офомленные в `$$...$$` располагаются строго на одной строке. Возникает соответствующая проблема с большими и подряд идущими формулами. Пожалуйста, не надо решать эту проблему так, это будет ужасно выглядеть:
``` latex
$$
формула_1
$$ 
$$
формула_2
$$
...
```


Для многострочных выключных формул используются следующие окружения:
``` latex
$$
\begin{multline}
1+2+3+4+5+6+7+8+9+10+\ldots\\
+46+47+48+\ldots\\
+99+100=5050
\end{multline}
$$ 
```

$$
\begin{multline}
1+2+3+4+5+6+7+8+9+10+\ldots\\
+46+47+48+\ldots\\
+99+100=5050
\end{multline}
$$

`multline` позволяет переносить строку (с помощью комбинации `\\`) естественным образом, формулы не будут расположены ровно друг под другом. Стандартный подход (между прочим, унаследован ещё от $\TeX$а), хотя конкретно на гитхабе какие-то слишком широкие страницы на компьютере и, как видно из примера выше, такое окружение подойдёт только для действительно больших формул.

``` latex
$$\begin{gather}
i+j=k;\\
j+k=i;\\
k+i=j.\\
\\
\therefore i+j+i+k=i. 
\end{gather}$$ 
```

$$
\begin{gather}
i+j=k;\\
j+k=i;\\
k+i=j.\\
\\
\therefore i+j+i+k=i.
\end{gather}
$$

Стандартное расположение формул друг под другом с помощью окружения `gather`.

``` latex
$$
\begin{aligned}
a+b+c+d+e+f&=g \Rightarrow \\
\Rightarrow g-f &= a+b+c+d+e. \\
\therefore a+b+c &= g-d-e-f.
\end{aligned}
$$
```
$$
\begin{aligned}
a+b+c+d+e+f&=g \Rightarrow \\
\Rightarrow g-f &= a+b+c+d+e. \\
\therefore a+b+c &= g-d-e-f.
\end{aligned}
$$

Расположение формул с выравниваем по знаку `&`.


``` latex
$$
\begin{cases} 
3x + 5y + z &= 0 \\ 
7x – 2y + 4z &= 0 \\ 
-6x + 3y + 2z &= 0 
\end{cases}
$$
```

$$
\begin{cases} 
3x + 5y + z &= 0 \\ 
7x – 2y + 4z &= 0 \\ 
-6x + 3y + 2z &= 0 
\end{cases}
$$

Окружение `cases` позволяет производить выравнивание и одновременно создаёт большую фигурную скобку слева. Отлично подходит для систем уравнений, а также для вариаций значения переменной при разных условиях.

#### Дополнение. Матрицы :feelsgood:
Всё достаточно просто. Матрица, очевидно, является окружением. Название окружения варьируется в зависимости от скобок матрицы. Для стандартных (круглых) скобок используется `pmatrix`, для \[квадратных\] `bmatrix`, для \|прямых\| и \|\|двойных прямых\|\| — `vmatrix` и `Vmatrix` соответственно. Разделение по столбцам, то есть выравнивание, как и выше, идёт по символу `&`, а перенос строки, как и выше, по символам `\\`.

Например, ввод такого кода
``` latex
$$
[\mathbf a,\mathbf b]=\begin{vmatrix}
  \vec{\mathbf{e}}_1 &\vec{\mathbf{e}}_2 &\vec{\mathbf{e}}_3\\
  a^1 &a^2 &a^3\\
  b^1 &b^2 &b^3\\
  \end{vmatrix}.
$$
```
  даст следующий результат:

  $$
  [\mathbf a,\mathbf b]=\begin{vmatrix}
  \vec{\mathbf{e}}_1 &\vec{\mathbf{e}}_2 &\vec{\mathbf{e}}_3\\
  a^1 &a^2 &a^3\\
  b^1 &b^2 &b^3\\
  \end{vmatrix}.
  $$
  Здесь следует обратить внимание на расположение индексов у базисных векторов. Сравните, например, `\vec{\mathbf{e_1}}`, `\vec{\mathbf{e}_1}` и `\vec{\mathbf{e}}_1`:
$$\vec{\mathbf{e_1}} \ne \vec{\mathbf{e}_1} \ne \vec{\mathbf{e}}_1$$


[^1]: Если я правильно понял, он и пользовательские css-стили поддерживает. 
[^2]: На самом деле команда `\frac13`, как и операция возведения в степень, в нашем случае сработала бы и без фигурных скобок. Скобки используются для однозначного _объединения_ аргументов.
[^3]: Я бы по умолчанию использовал первый вариант, но об обозначениях договоримся позже.
[^4]: можете ещё на номо$\TeX$е подглядывать ахахаха (не относитесь к этим словам серьёзно)

