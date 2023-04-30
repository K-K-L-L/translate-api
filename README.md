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
# PHP
```
<?php
$text_here = "السلام عليكم";
$lang_here = "en";

$url = 'https://API.englishboy.repl.co/translate?text='.urlencode($text_here).'&to='.urlencode($lang_here);

$response = file_get_contents($url);
$result = json_decode($response, true);

if ($result !== false) {
    echo $result['text'];
} else {
    echo 'Request failed';
}
?>
```
**If you have any questions contact me on Discord: KKLL#9777**
