## Цель работы

1. Зекрепить практические навыки использования языка программирования R для обработки данных
2. Закрепить знания основных функций обработки данных экосистемы tidyverse языка R
3. Закрепить навыки исследования метаданных DNS трафика

###  Задание 1-3 
Подготовленные данные:

```{r}
library(dplyr)
data<-read.csv("dns.csv")
print(data)
```

### Задание 4
Сколько участников информационного обмена в сети Доброй Организации?

```{r}
print(length(unique(union((unique(data$is)),(unique(data$id))))))
```

### Задание 5
Какое соотношение участников обмена внутри сети и участников обращений к внешним ресурсам?

```{r}
vnr<- select()
vns
```

### Задание 6
Найдите топ-10 участников сети, проявляющих наибольшую сетевую активность.

```{r}
library(dplyr)
slice(as.data.frame(rev(sort(table(data$is)))),1:10)
```

### Задание 7
Найдите топ-10 доменов, к которым обращаются пользователи сети и соответственное количество обра-
щений

```{r}

```
### Задание 8
Опеределите базовые статистические характеристики (функция summary()) интервала времени между
последовательным обращениями к топ-10 доменам.

```{r}

```
### Задание 9
Часто вредоносное программное обеспечение использует DNS канал в качестве канала управления, пе-
риодически отправляя запросы на подконтрольный злоумышленникам DNS сервер. По периодическим
запросам на один и тот же домен можно выявить скрытый DNS канал. Есть ли такие IP адреса в исследу-
емом датасете?
```{r}

```
