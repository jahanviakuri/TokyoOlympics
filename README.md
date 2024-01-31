# TokyoOlympics


Data source     --ingestion----------> Data Factory (source from http) ---> Data lake Gen 2
(http //github --> raw csv file)                                         ( Data sink in raw-data folder)

Raw-data folder in DL ----connect DL to DBricks using app --------> Azure databricks ---------->Data lake gen 2
                                                       (Transform data using spark session)    ( store data in transform data-folder)

Transform-data folder in DL ----------> Synapse Analystics  --------------> analytic tools( POWERBI , Tableau)
                                   ( use SQL to draw patterns)
