# Telegraf System Setup Process

The procedure for setting up the telegraf to parse log files.  Currently a configuration file has been written to parse QE logs.

## Telegraf Windows Service Setup

References:
  - [Running Telegraf as a Windows service](https://github.com/influxdata/docs.influxdata.com/blob/master/content/telegraf/v1.7/administration/windows_service.md) - Official Documentation

1. Download the [telegraf distribution for windows.](https://dl.influxdata.com/telegraf/releases/telegraf-1.10.4_windows_amd64.zip)

2. Either download the telegraf.conf configuration file from the github repo for the lab system you wish to setup or grab the telegraf.conf file you created in the Config File Setup.

3. Create the directory `C:\Program Files\Telegraf`

4. Place both the telegraf.exe that was downloaded in step 1 and the config file downloaded in step 2 into `C:\Program Files\Telegraf`

5. As administrator run powershell and run the command `C:\"Program Files"\Telegraf\telegraf.exe --service install`

6. To start telegraf run the command `net start telegraf`
