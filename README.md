# dataviz_workshop
Тренінг з візуалізації даних


Джерело даних: https://github.com/CSSEGISandData/COVID-19


**Найпростіший спосіб отримати ISO коди країн у R:

Потрібен пакет "countrycode"

#встановити бібліотеку
install.packages("countrycode")

#завантажити
library(countrycode)

#також потрібна бібліотека dplyr

df %>% mutate(ISO = countrycode(countryColumn, origin = 'country.name', destination = 'genc3c'),
         countryColumn = as.character(countryColumn))
         
де countryColumn - колонка у даних, де зазначені назви країн англійською



