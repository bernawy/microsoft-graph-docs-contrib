---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = AllowedValue(
	id = "Alpine",
	is_active = True,
)

result = await graph_client.directory.custom_security_attribute_definitions.by_custom_security_attribute_definition_id('customSecurityAttributeDefinition-id').allowed_values.post(request_body)


```