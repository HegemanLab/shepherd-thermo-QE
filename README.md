# Shepherd-thermo-QE
Log parsing and forwarding to an InfluxDB database for logs from [Q Exactive Mass Spectrometer](https://www.thermofisher.com/order/catalog/product/IQLAAEGAAPFALGMAZR) using Telegraf.

## Motivation
The goal is to have real-time and historical monitoring of the QE's logbook and temperature logs so that machine performance and status can be evaluated.

## Screenshots

## Tech used
[Telegraf](https://github.com/influxdata/telegraf)

## Installation
1. Download the [telegraf distribution for windows.](https://dl.influxdata.com/telegraf/releases/telegraf-1.10.4_windows_amd64.zip)

2. Either download the telegraf.conf configuration file from the github repo for the lab system you wish to setup or grab the telegraf.conf file you created in the Config File Setup.

3. Create the directory `C:\Program Files\Telegraf`

4. Place both the telegraf.exe that was downloaded in step 1 and the config file downloaded in step 2 into `C:\Program Files\Telegraf`

5. As administrator run powershell and run the command `C:\"Program Files"\Telegraf\telegraf.exe --service install`

6. To start telegraf run the command `net start telegraf`
## References
- [Running Telegraf as a Windows service](https://github.com/influxdata/docs.influxdata.com/blob/master/content/telegraf/v1.7/administration/windows_service.md) - Official Documentation
