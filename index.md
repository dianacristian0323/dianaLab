## COOKIES

<body> 
  <div class='row">
  	<input id="username" type="text" class="form-control " placeholder="username" aria-label="username">
  </div>

  Nume utilizator: <button class="btn btn-success custom" type="button" id="addUsernameCookie" onclick="setUsernameCookie()">Salveaza</button>
  
 Versiune browser: 

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


  function getCookie(cname) {
    var name = cname + "=";
    var ca = document.cookie.split(';');
    for(var i=0; i<ca.length; i++) {
        var c = ca[i];
        while (c.charAt(0)==' ') c = c.substring(1);
        if (c.indexOf(name) == 0) return c.substring(name.length,c.length);
    }
    return "";
}

function GetCookies() {
    document.getElementById('txtFirstName').value = getCookie('CTFirstName');
}

</script>
  
// Opera 8.0+
var isOpera = (!!window.opr && !!opr.addons) || !!window.opera || navigator.userAgent.indexOf(' OPR/') >= 0;

// Firefox 1.0+
var isFirefox = typeof InstallTrigger !== 'undefined';

// Safari 3.0+ "[object HTMLElementConstructor]" 
var isSafari = /constructor/i.test(window.HTMLElement) || (function (p) { return p.toString() === "[object SafariRemoteNotification]"; })(!window['safari'] || (typeof safari !== 'undefined' && window['safari'].pushNotification));

// Internet Explorer 6-11
var isIE = /*@cc_on!@*/false || !!document.documentMode;

// Edge 20+
var isEdge = !isIE && !!window.StyleMedia;

// Chrome 1 - 79
var isChrome = !!window.chrome && (!!window.chrome.webstore || !!window.chrome.runtime);

// Edge (based on chromium) detection
var isEdgeChromium = isChrome && (navigator.userAgent.indexOf("Edg") != -1);

// Blink engine detection
var isBlink = (isChrome || isOpera) && !!window.CSS;


  
  <body onunload="WriteCookies()" onload="GetCookies()">

</body>
