This folder contains the following challenge

Challenge #2

We need to write code that will query the meta data of an instance within AWS and provide a json formatted output. The choice of language and implementation is up to you.
Bonus Points
The code allows for a particular data key to be retrieved individually
Hints
·         Aws Documentation (https://docs.aws.amazon.com/)
·         Azure Documentation (https://docs.microsoft.com/en-us/azure/?product=featured)
·         Google Documentation (https://cloud.google.com/docs)
 
Link Referred - https://docs.microsoft.com/en-us/rest/api/compute/virtual-machines/get

To do challenge 2 i have created a virutal machine on azure using the rest api querying VMs metadata in jason format

1.  API get request would look like following 

GET https://management.azure.com/subscriptions/[subscriptionId]/resourceGroups/chethanEX/providers/Microsoft.Compute/virtualMachines/samplevm1?api-version=2021-07-01
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6ImpTMVhvMU9XRGpfNTJ2YndHTmd2UU8yVnpNYyIsImtpZCI6ImpTMVhvMU9XRGpfNTJ2YndHTmd2UU8yVnpNYyJ9.eyJhdWQiOiJodHRwOi8vY2JwZzAzbG9hZGRldnJlZ3Vpd2ViLmF6dXJld2Vic2l0ZXMubmV0IiwiaXNzIjoiaHR0cHM6Ly9zdHMud2luZG93cy5uZXQvZGMwYzZiMDgtYWZkMi00MTcxLWJiYTQtNjFjNzg2MWNlZmEzLyIsImlhdCI6MTY1MTIxNDE3NCwibmJmIjoxNjUxMjE0MTc0LCJleHAiOjE2NTEyMTgwNzQsImFpbyI6IkUyWmdZSEJYamVpN1ZLbXh4SHpuN2hJak1kWUxBQT09IiwiYXBwaWQiOiI3YWUxNTNkMS1mMmFkLTQ5ODEtYmE5Zi1jNDNiOWM2ZDJhZDYiLCJhcHBpZGFjciI6IjEiLCJncm91cHMiOlsiZWI1OGUyYjktMzdhOC00OWNkLWI2Y2MtNGI2MTYyMzliZTJmIiwiODNmYTg4MmEtZWIwYy00MmQzLTlkNjctOWU1ZDhiYmRhNTAwIiwiMDY2ZWJmOGYtYjQzZC00ZGFiLWFmNWUtZjIzYzU3YjAwNTljIl0sImlkcCI6Imh0dHBzOi8vc3RzLndpbmRvd3MubmV0L2RjMGM2YjA4LWFmZDItNDE3MS1iYmE0LTYxYzc4NjFjZWZhMy8iLCJvaWQiOiIyOTFiNGYzNy1iODk3LTQ4NGYtODc1ZS02ZGM2OGM5ZDhhNmYiLCJyaCI6IjAuQVMwQUNHc00zTkt2Y1VHN3BHSEhoaHp2b3p6RVkybUxKYzFGcERJZWR3OUJONFF0QUFBLiIsInN1YiI6IjI5MWI0ZjM3LWI4OTctNDg0Zi04NzVlLTZkYzY4YzlkOGE2ZiIsInRpZCI6ImRjMGM2YjA4LWFmZDItNDE3MS1iYmE0LTYxYzc4NjFjZWZhMyIsInV0aSI6InVtbUJkb1ZtMzAtc3NTVHI4cnBZQUEiLCJ2ZXIiOiIxLjAifQ.lG3LWuCt2vJ2M_iUX1hIdoYBYXhj7Hs-kvN4YfT-88jYCzyW1B2Ak9tqqeX6S_PZTUFjapKYrF9dAHM7MFa6F8tGJAY6p1KOtmB48WG48NxA_8kItwwE2E08OrBkx7XZCWjaSlSQ0CAO73dBraSQa5BA4vvzQhQrn4K2VejSuOYqMAc5bG5c4e6tq61-x1ed_dgjdcUYi3hH5bvCO9ZVDh5_ZqVACLm-BQhoYJA48NRzQ85K7ENG5o7zGXzbrSMOiKqbegoTw0tba0KrGTlWz8pGuDUzQAZLCVEyySEcnDP1ZvpJYsfx2dj6dyhQsfCGUzmdM1m9yCKtpzHHfnXOjw




