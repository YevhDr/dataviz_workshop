# Тренінг з візуалізації даних (18 березня 2021 року)

Джерело даних: https://github.com/CSSEGISandData/COVID-19 (Інститут Джона Хопкінса)





**Як отримати ISO коди країн (шпаркалка для R-studio)**

*#встановити бібліотеку "countrycode"*

install.packages("countrycode")

*#підʼєднати її*

library(countrycode)

*#також потрібна бібліотека "dplyr"*

library(dplyr)


*Ось так додаємо в наші дані колонку*

**df %>% mutate(ISO = countrycode(countryNameColumn, origin = 'country.name', destination = 'genc3c'),
         countryNameColumn = as.character(countryNameColumn))**
         
countryNameColumn - колонка у даних, де зазначені назви країн



