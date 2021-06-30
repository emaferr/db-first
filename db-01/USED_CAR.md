# Dealer Database

## (table) Used_Cars

- id                       BINGINT          PRIMARY KEY UNIQUE NOTNULL INDEX    
- brand                    VARCHAR(50)      NOTNULL
- model                    VARCHAR(50)      NOTNULL           
- model_year               YEAR             NULL      <!-- es: 2010 -->           
- release_year             YEAR             NOTNULL
- body_type                VARCHAR(50)      NOTNULL   <!-- es: Hatchback, SUV, wagon etc. -->
- color                    VARCHAR(30)      NOTNULL
- mileage_km               MEDIUMINT        NULL      <!-- es: 180.000 -->
- engine_cc                SMALLINT         NOTNULL   <!-- es: 7000 -->

