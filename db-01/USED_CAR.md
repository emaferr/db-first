# Dealer Database

## Used_Cars

- id                       BINGINT          PRIMARY KEY UNIQUE NOTNULL INDEX   
- chassis_number           CHAR(17)         UNIQUE NOTNULL
- plate                    VARCHAR(8)       UNIQUE NOTNULL
- brand                    VARCHAR(50)      NOTNULL
- model                    VARCHAR(50)      NOTNULL           
- model_year               YEAR             NULL       <!-- es: 2010 -->           
- release_year             YEAR             NOTNULL
- body_type                VARCHAR(50)      NOTNULL    <!-- es: Hatchback, SUV, Wagon etc. -->
- color                    VARCHAR(30)      NOTNULL
- mileage_km               MEDIUMINT        NULL       <!-- es: 180.000 -->
- engine_cc                SMALLINT         NOTNULL    <!-- es: 7000 -->
- hp                       SMALLINT         NOTNULL    <!-- es: 7000 --> 
- kw                       SMALLINT         NULL       <!-- es: 1000 --> 
- fuel_type                VARCHAR(30)      NOTNULL    <!-- es: eletric, gpl, gasoline --> 
- fuel_capacity_liters     FLOAT(4,2)       NULL       <!-- es: 35.50 --> 
- consumption_liter        FLOAT(4,2)       NULL       <!-- es: 18.12 --> 
- co2_emissions_gram       FLOAT(5,2)       NULL       <!-- es: 200,80 -->
- drive_type               CHAR(3)          NOTNULL    <!-- es: AWD, FWD, RWD, 4WD -->
- passenger_capacity       TINYINT          NULL
- doors                    TINYINT          NOTNULL    <!-- es: 3/4, 4/5 -->
- driver_side              VARCHAR(5)       NULL       <!-- es: left or right -->
- average_weight_kg        SMALLINT         NULL       <!-- es: 2700 -->
- average_length_meters    FLOAT(3,2)       NULL       <!-- es: 1,97 -->
- transmission             VARCHAR(3)       NOTNULL    <!-- es: AT, MT, CVT -->
- top_speed                FLOAT(5,2)       NULL       <!-- es: 190,80 -->
- gps                      TINYINT(1)       NULL       <!-- boolean -->
- alarm                    TINYINT(1)       NULL       <!-- boolean -->
- air_conditioning         TINYINT(1)       NULL       <!-- boolean -->
- path                     VARCHAR(255)     NULL       <!-- /img/car.jpg -->
- price                    FLOAT(9,2)       NULL       <!-- es: 1.500.000,99 -->
- first_insert             DATETIME         NOTNULL    
- time                     TIMESTAMP        CURRENT_TIMESTAMP