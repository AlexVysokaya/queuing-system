# queuing-system

Представленная в данной работе программа моделирует работу СМО с ограниченным буфером (или без буфера), 
обрабатывающую входной поток в виде задач, заданных определенным законом распределения. Также рассчитываются характеристики данной модели.

Для описания потока заявок необходимо:
1. Задать интервалы времени между соседними моментами поступления заявок (Tzmin и Tzmax) и интервал времени для вычисления времени обработки (Tsmin и Tsmax),
если будет использован линейный закон распределения.
2. Задать интенсивность потока λ и интенсивность обслуживания µ, если будет использоваться экспоненциальный закон распределения. 

Инструкция:

1. Перейдите по ссылке: https://alexvysokaya.github.io/queuing-system/

2. По умолчанию все поля заполнены данными из задания. Если хотите изменить данные, нажмите на поле ввода,
удалите предыдущее значение и введите с клавиатуры новое. Все данные необходимо ввести, пустой строки быть не должно.
Кол-во серверов (N) и мест в буфере (M) должно быть целым числом. При этом, кол-во серверов должно быть больше 0,
а кол-во мест в буфере больше или равно 0.
Все остальные параметры ВС могут быть записаны как целыми числами, так и дробными. При этом дробь может быть, как
десятичная (!!!обязательно через точку), так и обычной (через дробную черту /), но никаких отступов перед числом или
пробелов внутри числа.
Правильный способ ввода:
Tzmin = 0.8333
Tzmin = 1.0
Tzmin = 1/2
Неправильный:
Tzmin = 1,5
Tzmin = 1 . 3
Tzmin =    1.3

При некорректном способе ввода программа может неправильно понять введенные значения, что может привести к некорректной работе.
В случае возникновения критической ошибки лучшим решением будет закрыть текущую вкладку и заново перейти по ссылки из пункта 1.

3. Обратите внимание, что Тsmin должно быть меньше Tsmax. Аналогично с Tzmin и Tzmax.

4. В случае, если выбрано экспоненциальное распределение, то Tsmin и Tzmax должны в сумме давать желаемое среднее значение.
Таким образом, если среднее время обработки = 2, то могут быть следующие комбинации: Tsmin = 2, Tsmax = 2; Tsmin = 1, Tsmax = 3;
и так далее, чтобы выполнялось условие:
(Tsmin + Tsmax) / 2 = tобр
От этого зависит какой будет частота обработки заявок µ.

5. Выбрать желаемый тип распределения: линейны или экспоненциальный.

6. После ввода всех значений нужно нажать кнопку «Смоделировать ВС и рассчитать ее параметры»

7. Если какие-то данные, необходимые для вычислений, не введены, программа сообщит вам об этом.

8. Дождаться расчета результатов.
9. Данная программа может моделировать разные виды СМО (одноканальную или многоканальную, с буфером или без него).
