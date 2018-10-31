# Overview

To interact with your Timesketch system, an API is available.

## Permissions

If you do n ot have the right permissions, the following error message will be posted

````
````

# Login / Authorisation

Login / Authorisation is done with JWT (JSON Web Token).

## URL

```
POST https://timesketch/login/
```

## Response

## Sampe data

Cannot post that because don't want to disclose my data. But it will look like the following:



## Sample GET

```
curl -X GET -k -H 'Accept: application/json'  -H "Content-type: application/json" -H "Accept: application/json" -i 'https://demo.timesketch.org/login/' --data '{"username": "admin", "password": "PASSWORD"}'
```

That csrf token can then be used for authentitcate other API endpoints.



# Sketches

## Get sketches

```
curl -X GET -k -H 'Accept: application/json'  -H "Content-type: application/json" -H "X-CSRF-Token: ImQ1ODFhMDkxNThhYzMwZWEwODljNDBmZDk0OWMxNDFhODAwZmRhY2Ui.Drm5XA.Klf6tifElERZPM72ddiEh9svvl8" -H "Accept: application/json" -i 'https://demo.timesketch.org/sketches/' --data '{"name": "", "description": "description"}'
```

# Create sketch

```
curl -X POST -k -H 'Accept: application/json'  -H "Cookie: eyJfZnJlc2giOmZhbHNlLCJjc3JmX3Rva2VuIjp7IiBiIjoiWkRVNE1XRXdPVEUxT0dGak16QmxZVEE0T1dNME1HWmtPVFE1WXpFME1XRTRNREJtWkdGalpRPT0ifX0.Drm5XA.65HdWH-WI_SkseMXzHIYgeYFf50"-H "Content-type: application/json" -H "X-CSRF-Token: ImQ1ODFhMDkxNThhYzMwZWEwODljNDBmZDk0OWMxNDFhODAwZmRhY2Ui.Drm5XA.Klf6tifElERZPM72ddiEh9svvl8" -H "Accept: application/json" -i 'https://demo.timesketch.org/sketches/' --data '{"name": "", "description": "description"}'
```

# Jupyter

There is also a Jupyter Notebook in that project, where I hope it will help.