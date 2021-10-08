# vaccinations
A small project which aim is to present an interactive map of COVID vaccination percentage in Poland (broken down by municipality) compared with election results for Poland's leading party Law and Justice (PiS) in 2019.

## Interctive map
http://covid-vaccinations.herokuapp.com/

## Data sources
1. [Official COVID vaccination data from "Open data" portal](https://dane.gov.pl/pl/dataset/2476,odsetek-osob-zaszczepionych-przeciwko-covid19-w-gm?fbclid=IwAR059OLAARQT9Umr02jVnfn9abacBD0ZF12fNyHH7m1hHXUswt-tufdMDsA)
2. [Official 2019 election data from National Electoral Commission](https://sejmsenat2019.pkw.gov.pl/sejmsenat2019/data/csv/wyniki_gl_na_listy_po_powiatach_sejm_xlsx.zip)
3. [The Main Office of Geodesy and Cartography regional division of the country into municipalities (shapefile)](http://www.gugik.gov.pl/pzgik/dane-bez-oplat/dane-z-panstwowego-rejestru-granic-i-powierzchni-jednostek-podzialow-terytorialnych-kraju-prg)

## Inspiration articles:

## Authors
Sebastian Konicz - sebastian.konicz@gmail.com

## Project Organization

------------

    ├── data                            <- place whre the data is stored
    │   │
    │   ├── final                           <- final files
	│   │
    │   ├── geo                             <- geospatial data
    │   │
    │   ├── interim                         <- interim data that has been transformed
    │   │
    │   └── raw                             <- the original, immutable data dump
    │
    ├── src                                 <- source code for use in this project
    │   │
    │   ├── 101_vac_cou_data_load.py            <- transforms oficial vaccination data to dataframe
    │   │
    │   ├── 102_vac_cou_map.py                  <- crates map besed on vaccination and geospacial data
    │   │
    │   ├── 201_elec_data_load.py               <- transforms oficial election data to dataframe
    │   │
    │   ├── 202_elec_cou_map.py                 <- crates map besed on election and geospacial data
    │   │
    │   └── 203_elec_correlation.py             <- calculation of Pearson's coefficient
	│
    ├── templates                       <- folder with template sites for flask
	│
    ├── app.py                          <- app for running flask and Dash application
	│
    ├── LICENSE                         <- MIT license.
	│
    ├── Procfile                        <- file for flask
	│
    ├── README.md                       <- the top-level README for developers using this project.
	│
    └── requirements.txt                <- requirements for the project

------------
