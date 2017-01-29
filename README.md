TMDBApi
=======
Node.JS library wrapping themoviedb.org v3 API.

### Installation

```
npm install tmdbapi
```

### Usage

```js
const tmdb = new (require('tmdb'))({
    apiv3: <YOUR_API_KEY>
    endpoint: //optional
    language: //optional
});
```

### Simple login

```js
tmdb.login('myusername', 'mypassword')
  .then(session => console.log('connected', session))
  .catch(console.error);
```

### Calls

A complete list of calls can be found on [the wiki](/wiki/Supported-methods)

## License 

The MIT License - Copyright (c) 2017 Jean van Kasteel <vankasteelj@gmail.com>

>Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

>The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

>THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.