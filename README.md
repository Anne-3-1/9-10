# 9-10
Анна

1-когда сопротивлением среды можно пренебречь (оно ничтожно мало)

2-Дискретизация - важный процесс, используемый для преобразования аналоговой информации в цифровой формат

3-сопротивление не учитывается

4-Для определения информационно-оптимального шага дискретизации можно использовать правило максимума детерминанта, оценив собственные числа автокорреляционной матрицы обрабатываемых сигналов

5-Для компьютерного моделирования в рассмотренной задаче можно использовать различные средства, например:

- OpenSim. Программная система с открытым исходным кодом для биомеханического моделирования. 

- Physics Abstraction Layer. Пакет физического моделирования с открытым исходным кодом. 

- Project Chrono. Платформа мультифизического моделирования с открытым исходным кодом. 

- Repast. Платформа для моделирования на основе агентов с версиями для отдельных рабочих станций и высокопроизводительных компьютерных кластеров. 

- SageMath. Система для экспериментов с алгеброй и геометрией с помощью Python. 

- Scilab. Бесплатное программное обеспечение с открытым исходным кодом для численных вычислений и моделирования. 

- ADINA. Программное обеспечение для инженерного моделирования конструкций, жидкостей, теплопередачи и мультифизических задач. 

- AnyLogic. Многофункциональный инструмент имитационного моделирования для бизнеса и науки.

6-// Инициализация начальных данных

t := 0;

v := v0; 

y := 0; 

h := 0; 

 repeat

 F := ro abs(v)*v*C*S/2;

 a := -g + F / m;

y:= y + v delta + a* delta delta / 2; 

 if y > h then h := y;
 
v :v + a* delta;

7-45 метров.

m*v^2/2=m*g*h

h=v^2/(2*g)=30^2/(2*10)=900/20=45 м

#10

1-Дискретные модели, по определению - это модели с величинами, принимающими конечное или счётное число значений в заданный (фиксированный) промежуток времени. На практике такие модели наиболее соответствуют действительности. Например, в биологии, численность популяции далеко не всегда зависит только от мгновенных значений ее в данный момент, а еще от численностей в некоторые предшествующие моменты времени, что как раз и может учитываться в дискретных моделях

2-Достоинства модели неограниченного роста:

является классической математической моделью динамики численности популяции; 

позволяет проводить расчёты в электронных таблицах. 

Недостатки модели неограниченного роста:

не учитывает, что рост численности популяции может сильно опережать рост ресурсов для её питания. 

Модель неограниченного роста адекватна, пока масса живых организмов достаточно мала по сравнению с предельно допустимой массой этих организмов в данных природных условиях. Например, модель считается адекватной, если разница в массе живых организмов через n лет составляет не более 10% от начальной массы

3-В основе модели ограниченного роста лежат следующие идеи:

Постоянный неограниченный рост популяции невозможен из-за конкуренции внутри популяции за ресурсы питания. 

Любая популяция, развиваясь, достигает своей максимальной численности, зависящей от факторов внешней среды. 

Достоинства модели ограниченного роста:

позволяет учитывать, что чем ближе масса живых организмов к предельно допустимой, тем меньшим становится коэффициент прироста; 

помогает проследить за изменением массы растений в разных климатических зонах, например, в тундре и тайге.

4-Согласно модели ограниченного роста, если в начальный момент численность популяции больше критической численности L, то популяция будет неограниченно расти. 

С точки зрения биологии это объясняется тем, что рано или поздно популяция сталкивается с ограничениями, не позволяющими ей наращивать далее своё обилие. Ресурсы, за счёт которых существуют виды — пища, убежища, подходящие места для размножения и т.п., на любой территории имеют пределы. 

Величина L получила название нижней критической численности (плотности) и индивидуальна для каждого вида. Например, по наблюдениям биологов, для ондатр критическая численность равна всего лишь одной паре особей на тысячу квадратных километров, а вот для американского странствующего голубя наименьшая критическая численность равна сотням тысяч особей

5-Для определения допустимого отлова с помощью моделирования используют модель ограниченного роста. В ней вводят максимальную численность популяции L и строят модель так, чтобы численность животных не превышала эту величину. Как только численность приближается к L, коэффициент прироста уменьшается и рост замедляется

6-Сущность отнощений хищник-жертва,заключается в том,что число хищников,напрямую зависит от числа жертв

7-Система «хищник — жертва» — сложная экосистема, для которой реализованы долговременные отношения между видами хищника и жертвы, типичный пример коэволюции. Отношения между хищниками и их жертвами развиваются циклически, являясь иллюстрацией нейтрального равновесия

8-Да, возможны и другие модели взаимного влияния видов, вот некоторые из них:

Аллелопатия. Подавление одного вида организмов другим вследствие выделения токсичных веществ. Пример: выделение антибиотиков двумя близкорасположенными бактериями, в этом случае антибиотик каждой бактерии будет замедлять рост и развитие другой, может приводить к гибели. 

Сожительство. Один организм использует другого (или его жилище) в качестве места проживания, не причиняя последнему вреда. Пример: взаимоотношения между растениями и дуплогнёздниками, те из птиц и зверей, которые заселяют уже существующие дупла, тем самым не наносят деревьям вреда, но и не приносят пользы. 

Сотрудничество. Объединение животных в группы для более успешного и эффективного выживания и развития. 

9-Обратная связь — в самом широком понимании ответная реакция человека или группы людей на получаемую информацию или совершаемое действие

10-Обратная связь в модели ограниченного роста работает следующим образом: коэффициент прироста KL не фиксирован, а меняется в зависимости от ситуации. На него влияют две величины — максимальная численность популяции L и текущая численность N

11-Поддержание постоянной температуры тела человека

12-Да, в модели ограниченного роста присутствует обратная связь. Это зависимость коэффициента прироста KL от численности N, с помощью которой регулируется численность. 

Саморегуляция в этой модели заключается в том, что если в какой-то момент популяция резко сокращается, после устранения проблемы численность снова восстанавливается и достигает максимального уровня L

13-В модели «хищник-жертва» существуют прямая и обратная связи между популяциями, причём эти связи в общем случае несимметричны.  

Асимметричность и несогласованность действия прямой и обратной связей служат источниками неустойчивости и колебаний в системе. 
