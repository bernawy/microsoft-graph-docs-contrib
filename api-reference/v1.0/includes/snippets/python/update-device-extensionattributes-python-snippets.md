---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = Device(
	additional_data = {
			"extension_attributes" : {
					"extension_attribute1" : "BYOD-Device",
			},
	}
)

result = await graph_client.devices.by_device_id('device-id').patch(request_body)


```