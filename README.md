# firewhat-delorme
DeLorme inReach ping simulation

Step 1:<br>
Create online form that will allow user to fill out all possible Delorme values.<br>
User typed input of Lat/Long, heading, speed? Random generated Lat/Long data? <br> 
User typed input of endpoint, i.e. http://www.firewhat.com/delorme/incomingMessage<br>
<br>
Step 2: <br> 
 Using Ajax, send filled out form to user supplied endpoint.
 
 <b>Example DeLorme inReach Json</b><br>
  ```javascript
  {
 "Version": "2.0",
 "Events": [
	 {
	 "imei": "100000000000001",
	 "messageCode": 3,
	 "freeText": "On my way.",
	 "timeStamp": 1323784607376,
	 "addresses": [
	 	{ "address": "2075752244" },
	 	{ "address": "support@delorme.com" }
 	 ],
	 "point": {
	 	"latitude": 43.8078653812408,
	 	"longitude": -70.1636695861816,
	 	"altitude": 45,
	 	"gpsFix": 2,
	 	"course": 45,
	 	"speed": 50
	 },
	 "status": {
	 	"autonomous": 0,
	 	"lowBattery": 1,
	 	"intervalChange": 0,
	 	"resetDetected": 0
	 }
	 }
 ]
}
```
