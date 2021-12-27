# Аттрактор Рёсслера

Аттрактор Рёсслера – хаотический аттрактор для системы Рёсслера, системы нелинейых дифференциальных уравнений, предложенных Отто Рёсслером. Система задается следующими уравнениями:

$$
{\displaystyle \left\{{\begin{matrix}{\frac {dx}{dt}}=-y-z\\{\frac {dy}{dt}}=x+ay\\{\frac {dz}{dt}}=b+z(x-c)\end{matrix}}\right.}
$$

a, b, c – параметры. При определенных параметрах, система проявляет хаотический характер. Сам Рёсслер изучал хаотический аттрактор с параметрам $a=0.2,\ b=0.2, \ c=5.7$, однако позднее стали чаще использовать параметры $a=0.1,\ b=0.1, \ c=14$. Аттрактор Рёсслера придумали с целью найти систему, которая ведет себя также как аттрактор Лоренца, но которую проще качественно анализировать. В результате так и оказалось, аттрактор Рёсслера можно считать минимальным по трем причинам: его фазовое пространство – 3 (что минимально для хаотической динамики), нелинейность в нем минимальна (только одно квадратичное слагаемое) и траектория аттрактора имеет одну долю (в то время как аттрактор Лоренца имеет две).

Пример хаотичности:

<table>
<tr>
<img width="50%" src="https://sun9-56.userapi.com/impg/k4JZLgwi1fYU1cMCK5U6DxXbo1H9PzsoqonHng/omhFeZ4Ht3U.jpg?size=794x516&quality=96&sign=31c93b2e056e80fe46147b8fa124f377&type=album" />
<tr/> <tr>
<img width="50%" src="https://sun9-78.userapi.com/impg/db6d97g9oIegNXoGxwkC0Q31oyzog4ot1Bu0SQ/dR5pp8701ww.jpg?size=724x660&quality=96&sign=4613cb0500901f3446c67df4039994c6&type=album" />
</tr>
</table>

## Анализ

Во первых, стоит отметить, что при a < 0 система сходится в конкретную точку.


<table>
<tr>
<img width="40%" src="https://sun9-14.userapi.com/impg/AkEIpK-zrk4CzJs5zGlNtuXiStfTZzr_w5l2iQ/ByIeBKgB9iE.jpg?size=804x510&quality=96&sign=266abfadc68bf5cc60242e35f67a690c&type=album" />
<tr/> <tr>
<img width="50%" src="https://sun9-41.userapi.com/impg/hsEErzjMJO2uR7LQxDzYX1g0jZwbYD2tN-YpVA/W2rJcC632Yg.jpg?size=1268x686&quality=96&sign=23cbc802af807169e4826adb2baaa833&type=album" />
</tr>
</table>

При параметрах $ a=b=0,\ 2.6\leq c\leq 4.2$ система обладает устойчивым предельным циклом.

<table>
<tr>
<img width="40%" src="https://sun9-52.userapi.com/impg/_cuiTfowQOVlcc5DLenkjDYHn-TZcePvnPTPEw/JnZxqzycF1M.jpg?size=782x518&quality=96&sign=3f25266960ff93bb1921577fa2e961a4&type=album" />
<tr/> <tr>
<img width="50%" src="https://sun9-65.userapi.com/impg/F8H2zrpDFdJABgWsRn4OBND-9wh6A-FsclvlbA/LN6oXaZWD5M.jpg?size=932x536&quality=96&sign=07914700bccd78690fff51c1f8807032&type=album" />
</tr>
</table>

Далее мы будем рассматривать вариант с $a=0.2,\ b=0.2, \ c=5.7$.

<table>
<tr>
<img width="40%" src="https://sun9-23.userapi.com/impg/qwNcDfhkiryiUAS-gBe5bvy8i-t7KXVAdPKv4Q/Gf07OBSIQSc.jpg?size=748x490&quality=96&sign=113927a31e352207da76bce624ad8bd6&type=album" />
<tr/> <tr>
<img width="45%" src="https://sun9-55.userapi.com/impg/N_EkNzbSLkre1crkJ7j9Ws2kQwbPVSbV22tC_g/u5ZIQpmtlJ4.jpg?size=762x636&quality=96&sign=ee96d9f4058ddd2b4a56a9aa4d5d71dd&type=album" />
</tr>
</table>


Некоторые свойства аттрактора Рёсслера можно исследовать с помощью линейных методов, например собственных векторов, но для основных свойств потребуются нелинейные методы, такие как отображение Пуанкаре и бифуркации.

Заметим, что при $$z=0$$ пропадает нелинейность в уравнениях и система приобретает вид:

$${\begin{cases}{\frac  {dx}{dt}}=-y\\{\frac  {dy}{dt}}=x+ay\end{cases}}$$

Мы можем найти собственные значения с помощью якобиана ${\begin{pmatrix}0&-1\\1&a\\\end{pmatrix}}$, которые равны ${\displaystyle (a\pm {\sqrt {a^{2}-4}})/2}(a\pm {\sqrt  {a^{2}-4}})/2$. Отсюда можно заметить, что при $ {\displaystyle 0<a<2}$ собственные значения комплексные с положительной вещественной частью, поэтому траектория является нестабильной и отталкивается по спирали от центра. Если вернутся к исходной системе, то когда $x$ становится больше $c$, $z$ начинает расти, соответственно уменьшая $x$. Таким образом происходит постоянный переход с горизонтальной "плоскости" на вертикальную, причем можно сказать, что параметр $c$ регулирует ширину нижней спирали. 

### Неподвижные точки

Найдем особые точки системы. Для этого приравняем уравнения к нулю и решим систему:

$$
{\begin{cases}x={\frac  {c\pm {\sqrt  {c^{2}-4ab}}}{2} = 0}\\y=-\left({\frac  {c\pm {\sqrt  {c^{2}-4ab}}}{2a}}\right) = 0\\z={\frac  {c\pm {\sqrt  {c^{2}-4ab}}}{2a} = 0}\end{cases}}
$$ 

Соответсвующие векторы неподвижных точек:

$$
\left({\frac  {c+{\sqrt  {c^{2}-4ab}}}{2}},{\frac  {-c-{\sqrt  {c^{2}-4ab}}}{2a}},{\frac  {c+{\sqrt  {c^{2}-4ab}}}{2a}}\right) \\
\left({\frac  {c-{\sqrt  {c^{2}-4ab}}}{2}},{\frac  {-c+{\sqrt  {c^{2}-4ab}}}{2a}},{\frac  {c-{\sqrt  {c^{2}-4ab}}}{2a}}\right)
$$

Как видно на графике, одна из этих точек находится в центре аттрактора, другая же отдалена от него.

<img width="60%" align="center" src="https://sun9-78.userapi.com/impg/ySU4fjqlSQl5X5DvUpeVJQrHJP9Dd96OmxANGQ/pBpQvzKAtcw.jpg?size=746x496&quality=96&sign=3365fe8e228107b3c979a0bfaa9e869f&type=album" />

<table>
<tr>
<img width="40%" src="https://sun9-19.userapi.com/impg/XnrorLBx1vDS0XfQlmmILCTcs_4DlT5J2mTwMA/Df-STLKgibU.jpg?size=936x688&quality=96&sign=02e5963d4a9807b2d18c856ab1474f73&type=album" />
<tr/> <tr>
<img width="45%" src="https://sun9-14.userapi.com/impg/TZkjeRwxTALyKXvFI0lLHxRf6nxWwJDpJBSUWw/6FM3ffqbjW0.jpg?size=620x644&quality=96&sign=65ca1ab7d81acb7145eb69d541ea1bea&type=album" />
</tr>
</table>

### Собственные значения

Анализировать каждую из этих неподвижных точек можно с помощью собственных векторов и собственных значений. Запишем якобиан для всей системы:

$${\begin{pmatrix}0&-1&-1\\1&a&0\\z&0&x-c\\\end{pmatrix}}$$

Для нахождения собственных значений решим уравнение:

$$-\lambda ^{3}+\lambda ^{2}(a+x-c)+\lambda (ac-ax-1-z)+x-c+az=0\,$$

Подставляя стандартные параметры ($$a=0.2,\ b=0.2, \ c=5.7$$), находим собственные значения для центральной неподвижной точки:

$$\lambda _{{1}}=0.0971028+0.995786i\, \\
{\displaystyle \lambda _{2}=0.0971028-0.995786i\,}\, \\
{\displaystyle \lambda _{3}=-5.68718\,}$$

C соответствующими собственными векторами:

$$v_{{1}}={\begin{pmatrix}0.7073\\-0.07278-0.7032i\\0.0042-0.0007i\\\end{pmatrix}} \\
v_{{2}}={\begin{pmatrix}0.7073\\0.07278+0.7032i\\0.0042+0.0007i\\\end{pmatrix}} \\
v_{{3}}={\begin{pmatrix}0.1682\\-0.0286\\0.9853\\\end{pmatrix}}$$


<img src="https://upload.wikimedia.org/wikipedia/commons/1/1c/Eigenvectors.png"/>

На графике выше изображено действие собственных векторов. Векторы $v_1, v_2$ отвечают за постепенное расширение спирали, вектор $v_3$ отвечает за движение вверх. Фиолетовая линия – траектория движения в обратном времени от точки, отложенной на $v_3$ над неподвижной точкой. Эта линия показывает, что происходит с траекториями, на которые сильно действует вектор $v3$. По этой линии можно судить о притягивающем влиянии $v_3$, отталкивающем влиянии $v_1,v_2$ и их совместном действии.

На всякий случай посмотрим на фазовый портрет, хотя по графику и собственным значениям видно, что это особая точка является устойчивым фокусом:


<img src="https://sun9-3.userapi.com/impg/8EonySRvMqt9Ky8jK2QEiMu7NztJ17Ph1-e_vg/8wa2rPsYQF0.jpg?size=741x496&quality=96&sign=2d45df289aecfacb1e26c465057a2e39&type=album" width=70%/>

Вторая неподвижная точка лежит далеко от траектории аттрактора, ее влияние незначительно, поэтому не будем на ней останавливаться.

### Отображение Пуанкаре

Для анализа хаотической динамики используется отображение Пуанкаре. Для этого фиксируется плоскость и запоминаются события прохождения траектории через эту прямую. Посмотрим на различные плоскости для аттрактора Рёсслера.

Обычно в качестве разделяющей плоскости берут плоскости, проходящие через оси. Для аттрактора Рёсслера брать плоскость $z=0$ не имеет смысла, так как почти все нижнее движение по спирали лежит в этой плоскости. 

С нашим набором параметров, брать плоскость $$y=0$$ также не имеет смысла так, как она пересекает только нижнюю спираль:
<img src="https://sun9-40.userapi.com/impg/A3CuDTPNfxC7_Pb319KrckUuOeXzBWvNHSrPeA/XQoaDz_LPNc.jpg?size=704x700&quality=96&sign=edce5f60a13128fc5b0d31410e24e28b&type=album" width=60%/>

Рассмотрим плоскость $x=0.1$:

<img width=60% src="https://sun9-10.userapi.com/impg/vM3osyqnvvNeyEicVzQoI_DEVxpnMxMCxGvJ9Q/bSUO8BrP9Sg.jpg?size=890x698&quality=96&sign=7d30352a15c0c941799b1283ecd49db7&type=album" />

Построим график зависимости $y$ от $z$. График отображает убывание $y$ с ростом $z$, собственно так и происходит, зависимость сохраняется, если посмотреть на траекторию всей системы.

<img width=60% src="https://sun9-85.userapi.com/impg/m3HvwMH274i2c_dD0BrHBfRCgA4fUuz88znvHQ/gFezjb6LJSM.jpg?size=736x514&quality=96&sign=a8e03cc778120485a325e37b5f4c8a0c&type=album" />

Конкретно с такой разделяющей плоскостью получается бесконечное число точек в отображении Пуанкаре, однако при изменении параметра $$c$$ количество точек может меняться, например при $c = 4$ будет всего 6 точек, так как траектория циклична:

<img width=80% src="https://sun9-3.userapi.com/impg/Qdhl7CWaXfV9jsER_EsWY5IaunZCbDVG8RtiCA/FFjpJrZcfc4.jpg?size=968x644&quality=96&sign=4f99dbcc5066ba01732e116111bc6517&type=album" />

### Диаграммы бифуркации

Диаграммы бифуркации используются для оценки влияния изменения параметров на систему. Для построения, изменяется одна переменная, а остальные фиксируются, затем строится график предела траектории (то есть последние несколько точек при $t \to \infty$). В этой статье рассматривалось влияние каждого параметра на каждое измерение системы. \
*Правильность метода не гарантируется


 
<table>
<tr>
<img width="33%" src="https://sun9-87.userapi.com/impg/MB5-aX318SCX0S8-wkjJGqL-bVePZYqXeoHPaQ/zBsOApFDltU.jpg?size=1522x2160&quality=96&sign=53f5764122ed8400a5cf52704bd5aa11&type=album" />
</tr> <tr>
<img width="33%" src="https://sun9-4.userapi.com/impg/mzZZEzbDKLyu_TNFnH7yUh6KYA1jWf8cXH2lUg/YdWJ9C-b0-s.jpg?size=1506x2160&quality=96&sign=9679c33a8a37e887fb7cb643536126f8&type=album" />
</tr> <tr>
<img width="33%" src="https://sun9-73.userapi.com/impg/oV3-oCMc4LnF-issG_xBc7XsCro0ItKrCUfa0Q/KlhFxfTJWTs.jpg?size=1490x2160&quality=96&sign=7ad1af630534778ae409b9adc9279aec&type=album" />
</tr>
</table>

В любом случае, можно сделать вывод, что система ведет неподвижно, периодично, квазипериодично и хаотично в зависимости от параметров.

## Применение в науке

В основном аттрактор Рёсслера используется в качестве простой модели для обоснования хаоса в непрерывном времени, а также служит прототипом для большинства систем с хаотическим характером, особенно в химии.

Так например, аттрактор Рёсслера применялся в исследовании хаоса в далекой от равновесия химической кинетике  (Ruelle 1973, Rössler 1976b, 1977b, Rössler & Wegmann 1978). Рёсслер и Вегманн предложили следующую схему химических реакций:

<img width=40% src="https://sun9-59.userapi.com/impg/_VqS6A5L_0_Ai536HwdXYOVELUDXJQxSESw-fQ/B3Wi09hV0ug.jpg?size=500x604&quality=96&sign=b5119fde08c23683aea0caad326fa503&type=album" />

в которой шаги 1 и 5 являются каталитическими, шаг 2 автокаталитический. Виды $A_1 - A_5$ находились фиксированными в больших резервуарах, в результате чего система не была в термодинамическом равновесии. Временная зависимость для видов $X, Y, Z$ была получена взятием производной закона действующих масс, эти уравнения имели квадратичные нелинейности. Соответственно схема на графике (b) приводит к аттрактору некоторой системы на графике (a):

<img src="https://sun9-43.userapi.com/impg/Hhz9B7Efmx3rj_0FO1Ns7wuJsbVZJBKJ6lJWgQ/Lsyq_QtyXcY.jpg?size=1736x676&quality=96&sign=8dca457a6f409d06eb02364c65a73314&type=album" />

Поведение системы на графике схоже с поведением аттрактора Рёсслера, это позволяет привести физическое, механическое обоснование процесса.

## Бонус

[Анимация траектории аттрактора Рёсслера с примером хаотичности](https://youtu.be/1iPklhy-HsE)

[Визуализатор построения траектории](https://colab.research.google.com/drive/1hV3DiLLKc0W959NSDGjyKpdgTQC6gA_r?usp=sharing)

