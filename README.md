# Lightweight PHP curl class
Lightweight class for simple curl requests.
Current version support only GET and POST requests.

## Usage:
Put file some where. In next example file shoulde be in same folder as main file.
```
require 'curl.class.php';

$curl = new Curl();

$response = $curl->get('http://example.com');

echo "Response: $response";
```

```
$curl = new Culr();
//Request paramertes
$params = array(
  'test' => 'test'
);
$headers = array(
  'User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36'
);
$response = $curl->post('http://api.example.com',$params,$headers);
```
##Methods

```
Curl::get($url, $params = array(), $headers = array(), $userOptions = array())
Curl::post($url, $params = array(), $headers = array(), $userOptions = array())
```
