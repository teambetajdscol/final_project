# final_project
Ini adalah respository sementara untuk Team Beta

## Business Problem Understanding
#### Context
Washington, D.C. adalah ibu kota dari Amerika Serikat yang berkembang pesat dengan populasi mendekati 700000 orang. Kota ini sangat terpisah dan memiliki biaya hidup yang tinggi. Pada tahun 2017, harga rata-rata rumah keluarga tunggal di kawasan tersebut dapat mencapai $649000. 

Melansir dari web [Redfin,](https://www.redfin.com/city/12839/DC/Washington-DC/housing-market) pemasaran perumahan Washington, D.C. cukup kompetitif dimana rumah di Washington, D.C. rata-rata menerima dua penawaran dan terjual dalam waktu sekitar 39 hari. 

#### Problem Statement
Dalam pasar perumahan, prediksi harga rumah yang akurat akan sangat membantu penjual dan agen properti dalam membuat keputusan yang informatif. Prediksi harga rumah merupakan salah satu tugas yang cukup rumit dilakukan karena banyak faktor yang dapat mempengaruhi keakuratan prediksi baik secara langsung ataupun tidak langsung. Prediksi harga rumah harus memberikan hasil yang cukup akurat sehingga pembeli bisa mendapatkan harga yang sesuai dengan rumah yang akan dijual. Selain itu, tingginya minat pembelian rumah di Washington, D.C., maka sangat penting juga untuk dapat menentukan harga rumah yang kompetitif dengan harga jual rumah lainnya.

#### Goals
Berdasarkan permasalahan tersebut, tujuan dari proyek ini adalah memprediksi harga rumah di Washington, D.C. untuk membantu pembeli dan penjual rumah dalam menentukan harga terbaik dimana agen properti bertindak sebagai pihak ketiga, sehingga nantinya dapat meminimalisir terjadinya *underprice* dan *overprice*.

Prediksi harga rumah akan dilakukan dengan menggunakan data aktual properti perumahan Washington,D.C. dan *machine learning*.

#### Analytic Approach
Jadi, yang perlu dilakukan dalam hal ini adalah:
* menganalisis data untuk dapat menemukan pola dari fitur-fitur yang ada, yang membedakan satu rumah dengan yang lainnya. 
* membangun suatu model regresi yang akan membantu dalam melakukan prediksi harga rumah yang akan berguna  dalam menentukan harga jual rumah.

#### Metric Evaluation


#### Attribute Information
|     No    |     Feature               |     Data Type    |     Description                                                                                                                         |
|-----------|---------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
|     1     |     Unnamed: 0            |     Int64        |     Number of Index                                                                                                                     |
|     2     |     BATHRM                |     int64        |     Number of bathrooms                                                                                                                 |
|     3     |     HF_BATHRM             |     int64        |     Number of half   bathroom     (No bathtub or shower)                                                                                |
|     4     |     HEAT                  |     object       |     Heating type                                                                                                                        |
|     5     |     AC                    |     Object       |     Air Conditioner   availability (Y/N)                                                                                                |
|     6     |     NUM_UNITS             |     float64      |     Number of units                                                                                                                     |
|     7     |     ROOMS                 |     int64        |     Number of rooms                                                                                                                     |
|     8     |     BEDRM                 |     int64        |     Number of bedrooms                                                                                                                  |
|     9     |     AYB                   |     float64      |     The earliest time the   main portion of the building was built                                                                      |
|     10    |     YR_RMDL               |     float64      |     The year structure was   remodeled                                                                                                  |
|     11    |     EYB                   |     int64        |     The year an   improvement was built more recent than actual year built                                                              |
|     12    |     STORIES               |     float64      |     Number of stories in   primary dwelling                                                                                             |
|     13    |     SALEDATE              |     object       |     Date of most recent   sale                                                                                                          |
|     14    |     PRICE                 |     float64      |     Price of most recent   sale                                                                                                         |
|     15    |     QUALIFIED             |     object       |     Internally used   indicator to reflect if a sale is representative of market value according to   the office's internal criteria    |
|     16    |     SALE_NUM              |     int64        |     Number of times it's   been sold since May 2014                                                                                     |
|     17    |     GBA                   |     float64      |     Gross building area in   square feet                                                                                                |
|     18    |     BLDG_NUM              |     int64        |     Building number on the   property                                                                                                   |
|     19    |     STYLE                 |     object       |     Type of story                                                                                                                       |
|     20    |     STRUCT                |     object       |     Building structure                                                                                                                  |
|     21    |     GRADE                 |     object       |     Property Grade                                                                                                                      |
|     22    |     CNDTN                 |     object       |     Property Condition                                                                                                                  |
|     23    |     EXTWALL               |     object       |     Exterior wall type                                                                                                                  |
|     24    |     ROOF                  |     object       |     Roof type                                                                                                                           |
|     25    |     INTWALL               |     object       |     Interior wall type                                                                                                                  |
|     26    |     KITCHENS              |     float64      |     Number of kitchens                                                                                                                  |
|     27    |     FIREPLACES            |     int64        |     Number of fireplaces                                                                                                                |
|     28    |     USECODE               |     int64        |     Property use code type                                                                                                              |
|     29    |     LANDAREA              |     int64        |     Land area of property   in square feet                                                                                              |
|     30    |     GIS_LAST_MOD_DTTM     |     object       |     Last modified data                                                                                                                  |
|     31    |     SOURCE                |     object       |     Raw data source                                                                                                                     |
|     32    |     CMPLX_NUM             |     float64      |     Complex number                                                                                                                      |
|     33    |     LIVING_GBA            |     float64      |     Gross building area in   square feet                                                                                                |
|     34    |     FULLADDRESS           |     object       |     Full street address                                                                                                                 |
|     35    |     CITY                  |     object       |     City                                                                                                                                |
|     36    |     STATE                 |     object       |     State                                                                                                                               |
|     37    |     ZIPCODE               |     float64      |     Zipcode                                                                                                                             |
|     38    |     NATIONALGRID          |     object       |     Address location   national grid coordinate spatial address                                                                         |
|     39    |     LATITUDE              |     float64      |     Latitude                                                                                                                            |
|     40    |     LONGITUDE             |     float64      |     Longitude                                                                                                                           |
|     41    |     ASSESSMENT_NBHD       |     object       |     Neighborhood ID                                                                                                                     |
|     42    |     ASSESSMENT_SUBNBHD    |     object       |     Subneighborhood ID                                                                                                                  |
|     43    |     CENSUS_TRACT          |     float64      |     Census tract                                                                                                                        |
|     44    |     CENSUS_BLOCK          |     object       |     Census block                                                                                                                        |
|     45    |     WARD                  |     object       |     Ward (district is   divided into eight wards, each with approximately 75,000 residents)                                             |
|     46    |     SQUARE                |     object       |     Square (Part of Square   Suffix Lot (SSL) an address identifier in DC)                                                              |
|     47    |     X                     |     float64      |     Longitude                                                                                                                           |
|     48    |     Y                     |     float64      |     Latitude                                                                                                                            |
|     49    |     QUADRANT              |     object       |     City quadrant (NE, SE,   SW, NW)                                                                                                    |
|     50    |     P0010001              |     Int64        |     Total population                                                                                                                    |
|     51    |     H0010001              |     int64        |     Total housing units                                                                                                                 |
|     52    |     H0010002              |     int64        |     Occupied housing units                                                                                                              |
|     53    |     H0010003              |     int64        |     Vacant housing units                                                                                                                |
|     54    |     ACRES                 |     float64      |     Acres                                                                                                                               |
|     55    |     SQ_MILES              |     float64      |     Square miles                                                                                                                        |
|     56    |     Shape_Length          |     float64      |     SHAPE length                                                                                                                        |
|     57    |     Shape_Area            |     float64      |     SHAPE area                                                                                                                          |
|     58    |     FAGI_TOTAL_2010       |     float64      |     The earliest time the   main portion of the building was built                                                                      |
|     59    |     FAGI_MEDIAN_2010      |     float64      |     The year structure was   remodeled                                                                                                  |
|     60    |     FAGI_TOTAL_2013       |     float64      |     The year an   improvement was built more recent than actual year built                                                              |
|     61    |     FAGI_MEDIAN_2013      |     float64      |     Number of stories in   primary dwelling                                                                                             |
|     62    |     FAGI_TOTAL_2011       |     float64      |     Date of most recent   sale                                                                                                          |
|     63    |     FAGI_MEDIAN_2011      |     float64      |     Price of most recent   sale                                                                                                         |
|     64    |     FAGI_TOTAL_2012       |     float64      |     Internally used   indicator to reflect if a sale is representative of market value according to   the office's internal criteria    |
|     65    |     FAGI_MEDIAN_2012      |     float64      |     Number of times it's   been sold since May 2014                                                                                     |
|     66    |     FAGI_TOTAL_2014       |     float64      |     Gross building area in   square feet                                                                                                |
|     67    |     FAGI_MEDIAN_2014      |     float64      |     Building number on the   property                                                                                                   |
|     68    |     FAGI_TOTAL_2015       |     float64      |     Type of story                                                                                                                       |
|     69    |     FAGI_MEDIAN_2015      |     float64      |     Building structure                                                                                                                  |
