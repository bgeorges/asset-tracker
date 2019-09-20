# asset-tracker

Email notification from SigFox
```json
{
"device":"2C37D2", 
"time":1560987871, 
"duplicate":false, 
"snr":18.15, 
"station":"4FD2", 
"data":"720209081140888107821410", 
"avgSnr":23.40, 
"lat":-39.0, 
"lng":176.0, 
"rssi":-101.00, 
"seqNumber":2852 
}
Parse payload using URL endpoint:
http://viper-oyster.4b63.pro-ap-southeast-2.openshiftapps.com/parse/720209081140888107821410
```

Parser should produce the following output extracting data from the payload, i.e "720209081140888107821410"

```json
{"MessageType":2,"UptimeWeeks":39,"TxCount":2304,"RxCount":256,"TripCount":17,"GpsSuccessCount":2112,"GpsFailureCount":96,"AverageFixTimeSeconds":15,"AverageFailTimeSeconds":130,"AverageFreshenTimeSeconds":10,"WakeUpsPerTrip":8}
```

other example with different payload
```json
{
"device":"2C37D2", 
"time":1560987823, 
"duplicate":false, 
"snr":22.15, 
"station":"4FD2", 
"data":"0063bcf0e82ee9e8680000d0", 
"avgSnr":23.38, 
"lat":-39.0, 
"lng":176.0, 
"rssi":-101.00, 
"seqNumber":2851 
}
```

Parse payload using URL endpoint:
http://viper-oyster.4b63.pro-ap-southeast-2.openshiftapps.com/parse/0063bcf0e82ee9e8680000d0

```json
{"MessageType":0,"InTrip":false,"LastFixFailed":false,"Latitude":-38.6876317,"Longitude":176.00945099999998,"Heading":0,"SpeedKmH":0,"BatteryVoltage":5.2}
```


