## COOKIES

<script> 
  document.cookie = "session=test GDPR"; 
  document.cookie = "favorite_task=collect Data"; 
  document.cookie = "username=Diana C";
  document.cookie = "browser=chrome";
  document.cookie = "browser=chrome";
  document.cookie = "expires=Fri, 11 Dec 2030 14:00:00 UTC";
  function alertCookie() { alert(document.cookie); } 
  
  
  
  document.cookie = "test1=Hello";
  document.cookie = "test2=World";

  const cookieValue = document.cookie
    .split('; ')
    .find(row => row.startsWith('test2='))
    .split('=')[1];

  function alertCookieValue() {
    alert(cookieValue);
  }


function doOnce() {
  if (!document.cookie.split('; ').find(row => row.startsWith('doSomethingOnlyOnce'))) {
    alert("Do something here!");
    document.cookie = "doSomethingOnlyOnce=true; expires=Fri, 31 Dec 2021 23:59:59 GMT";
  }
}


function resetOnce() {
  document.cookie = "doSomethingOnlyOnce=; expires=Thu, 01 Jan 1970 00:00:00 GMT";
}


//ES5

if (document.cookie.split(';').some(function(item) {
    return item.trim().indexOf('reader=') == 0
})) {
    console.log('The cookie "reader" exists (ES5)')
}

//ES2016

if (document.cookie.split(';').some((item) => item.trim().startsWith('reader='))) {
    console.log('The cookie "reader" exists (ES6)')
}



//ES5

if (document.cookie.split(';').some(function(item) {
    return item.indexOf('reader=1') >= 0
})) {
    console.log('The cookie "reader" has "1" for value')
}

//ES2016

if (document.cookie.split(';').some((item) => item.includes('reader=1'))) {
    console.log('The cookie "reader" has "1" for value')
}


</script>

<body> 
  COOKIES: <button class="btn btn-info" onclick="alertCookie()">Show cookies</button> 
<br>
  Get a sample cookie named test2: <button onclick="alertCookieValue()">Show cookie value</button>
<br>
  Do something only once: <button class="btn btn-info" onclick="doOnce()">Only do something once</button>
<br>
  Reset the previous cookie: <button class="btn btn-info" onclick="resetOnce()">Reset only once cookie</button>
<br>
   Check a cookie existence
 <br>
  Check that a cookie has a specific value
</body>
