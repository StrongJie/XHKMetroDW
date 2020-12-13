# XHKMetroDW
Development and construction of digital warehouse in Metro data.
The data set comes from the open source data of Shenzhen municipal government, and the data does not involve any sensitive information. It can be used for big data processing, such as offline computing.

## Big data technology ecology involved
1.Hadoop：HDFS MR Yarn  
2.Hive  
3.Redis  
4.Flink

## Key points of the project
1. The data contains 1.33 million Metro information data, in the file folder.
2. Using Flink Scala for ETL to produce data information in CSV format. You need to use local redis because redis is used to remove duplication.
   According to the current code logic, it may take more time to parse all the data.
   At present, the project does not involve data collection. After extracting the CSV data, the data needs to be manually transferred to the relevant directory of HDFS
3. The data warehouse part is divided into ODS DWD DWS ADS, in which ADS involves several indexes, which are basically calculated offline based on one day's indicators.

## Future development plan
1.Add real-time calculation and processing part  
2.Add data display part

## Thanks
The whole project refers to the open source project of youth geek. If you want to know more about the ecological use of big data based on this dataset, please see this link:
https://gitee.com/geekyouth/SZT-bigdata?_from=gitee_search
