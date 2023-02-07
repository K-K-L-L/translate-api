# translate-api
### A fast, accurate translate API supporting multiple languages. Real-time text translation. Wide range of language support. Try it now!

# Python
```
import requests

text_here = "مرحبا"
lang_here = "en"

url = f'https://API.englishboy.repl.co/translate?text={text_here}&to={lang_here}'

response = requests.get(url)

if response.status_code == 200:
    result = response.json()
    print(result['text'])
else:
    print('Request failed with status code:', response.status_code) # Output: Welcome
```

# JavaScript
```
const axios = require('axios');

let text_here = "مرحبا";
let lang_here = "en";

let url = `https://API.englishboy.repl.co/translate?text=${text_here}&to=${lang_here}`;

axios.get(url)
  .then(response => {
    if (response.status === 200) {
      let result = response.data;
      console.log(result['text']);
    } else {
      console.log(`Request failed with status code: ${response.status}`);
    }
  })
  .catch(error => {
    console.error(error);
  });
```

**If you have any questions contact me on Discord: Rian1545#0371**
