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



</script>

<body> 
  COOKIES: <button onclick="alertCookie()">Show cookies</button> 
<br>
 Get a sample cookie named test2: <button onclick="alertCookieValue()">Show cookie value</button>
<br>
 Do something only once: <button onclick="doOnce()">Only do something once</button>
<br>
  
</body>
