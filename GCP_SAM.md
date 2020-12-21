Create Google Cloud Platform Function (HTTP trigger) which will list buckets (storages),
get objects and find param.json. If file exist, function should parse it and start\stop
instances described in file.

Feel free to create 3 vm's before.

#### Note:
	- only 2 vm's can be running. if all of them have "start" action 
	  start 2 of them and modify param.json in bucket

#### Param.json example:
```sh
{
	"vm-first": {
		"name": "[INSTANCE_NAME]",
		"zone": "[INSTANCE_ZONE]",
		"action": "stop"
		},
	"vm-second": {
		"name": "[INSTANCE_NAME]",
		"zone": "[INSTANCE_ZONE]",
		"action": "start"
		},
	"vm-third": {
		"name": "[INSTANCE_NAME]",
		"zone": "[INSTANCE_ZONE]",
		"action": "start"
		}
}
```
