# dataviz_workshop
Тренінг з візуалізації даних (18 березня 2021 року)

Джерело даних: https://github.com/CSSEGISandData/COVID-19 (Інститут Джона Хопкінса)





**Як отримати ISO коди країн

Для R - потрібен пакет "countrycode"

*#встановити бібліотеку
install.packages("countrycode")

*#завантажити
library(countrycode)

*#також потрібна бібліотека "dplyr"


*Ось так додаємо в наші дані колонку
df %>% mutate(ISO = countrycode(countryColumn, origin = 'country.name', destination = 'genc3c'),
         countryColumn = as.character(countryColumn))
         
де countryColumn - колонка у даних, де зазначені назви країн англійською



