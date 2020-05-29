# Driver license datasets
It contains datasets related to Italian drive licenses, a dataset for each region.

These datasets were published as Open Data by the Italian Ministry of Infrastructure and Transport.
They have been downloaded in October, 2019 from http://dati.mit.gov.it/catalog/dataset/patenti.
However, in January, 2020 the Italian Ministry modified the actual available version by limiting the exposed data.

## Dataset content

| *Original column name*      | *English column name*       | *Format*                                                                                               | *Description*                                                                                                 |
|-----------------------------|-----------------------------|--------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| ID                          | ID                          | number                                                                                                 | Progressive row ID                                                                                            |
| anno_nascita                | year of birth               | date (AAAA)                                                                                            | Year of birth of the license holder                                                                           |
| comune_residenza            | municipality of residence   | string                                                                                                 | Italian municipality that is the residence of the license holder                                              |
| provincia_residenza         | province of residence       | string                                                                                                 | Italian province that is the residence of the license holder                                                  |
| regione_residenza           | region of residence         | string                                                                                                 | Italian region that is the residence of the license holder                                                    |
| stato_estero_nascita        | foreign birth state         | string                                                                                                 | Foreign state of birth of the license holder (if any)                                                         |
| sesso                       | gender                      | string (M\|F)                                                                                          | Gender of the license holder                                                                                  |
| categoria_patente           | license category            | string (AMS \| CS \| AM \| C \| BS \| AS \| D \| BE \| B \| CE \| F \| DS \| CATEGORIA NON CODIFICATA) | Maximum category obtained by the license holder at the dataset creation/update                                |
| data_rilascio               | release date                | date (AAAA-MM-DD HH:MM:SS)                                                                             | Date of the license release **_NOTE_**: the time is empty                                                     |
| abilitato_a                 | qualification               | string (S\|N)                                                                                          | It indicates whether regardless of the maximum category, the license has one of the A2, A3, A4 qualifications |
| data_abilitazione           | qualification date          | date (AAAA-MM-DD HH:MM:SS)                                                                             | Date of the qualification release **_NOTE_**: the time is empty                                               |
| data_scadenza               | expiry date                 | date (AAAA-MM-DD HH:MM:SS)                                                                             | Date of the license expiry **_NOTE_**: the time is empty                                                      |
| stato_estero_primo_rilascio | foreign state first release | string                                                                                                 | Foreing state first license release (if any)                                                                  |
| punti_patente               | License points              | Number                                                                                                 | Number of license points                                                                                      |

## Dataset format

Each dataset is released as a ZIP file containing the original CSV file.
