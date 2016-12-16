# easy-http
Simple http requests using ES5 and XMLHttpRequest


## Usage
```js

 http({
      method: 'GET',
      url: 'https://dragons-api.herokuapp.com/api/dragons'
    })
    .then(function(response) {
      console.log('get response', response)
    })
    .catch(function(err) {
      console.log('err', err)
    })

```
```js

 http({
      method: 'POST',
      url: 'https://app.com/api/user',
      data: {
        name: 'Olar',
        email: 'email@gmail.com'
      }
    })
    .then(function(response) {
      console.log('post response', response)
    })
    .catch(function(err) {
      console.log('err', err)
    })

```

### Add headers

```js

 http({
      method: 'POST',
      url: 'https://app.com/api/user',
      data: {
        name: 'Olar',
        email: 'email@gmail.com'
      },
      headers: {
       'Content-Type': 'application/json;charset=UTF-8'
      }
    })
    .then(function(response) {
      console.log('post response', response)
    })
    .catch(function(err) {
      console.log('err', err)
    })

```
