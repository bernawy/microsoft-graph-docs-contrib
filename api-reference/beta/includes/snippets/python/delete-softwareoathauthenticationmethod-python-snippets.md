---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)


await graph_client.users.by_user_id('user-id').authentication.software_oath_methods.by_software_oath_authentication_method_id('softwareOathAuthenticationMethod-id').delete()


```