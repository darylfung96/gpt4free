### Example: `forefront` (use like openai pypi package) <a name="example-forefront"></a>

```python
from gpt4free import forefront
# create an account
acount_data = forefront.Account.create(logging=False)
print(token)
# get a response
for response in forefront.StreamingCompletion.create(
	account_data=account_data,
	prompt='hello world',
	model='gpt-4'
):
    print(response.choices[0].text, end='')
print("")
```
