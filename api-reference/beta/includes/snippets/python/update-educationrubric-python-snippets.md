---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = EducationRubric(
	display_name = "Example Credit Rubric after display name patch",
)

result = await graph_client.education.me.rubrics.by_education_rubric_id('educationRubric-id').patch(request_body)


```