## COOKIES

<body> 
  <div class="row">
  	<input id="username" type="text" class="form-control " placeholder="username" aria-label="username">
  </div>
<br>
   <button class="btn" type="button" id="addUsernameCookie" onclick="setUsernameCookie()">Salveaza</button>
  <br>
  Nume utilizator:<span id="usernameCookie"> </span>
  <br>
 Versiune browser: <span id="browserVersionCookie"> </span>
  
  <br>
  <a title="Analiza DPIA" href="https://didatec-my.sharepoint.com/personal/cristian_is_diana_utcluj_didatec_ro/_layouts/15/doc.aspx?sourcedoc={8cb11dbf-1ff3-4dbf-97f9-72e446aab3e6}&action=edit">
	</a>
  
</body>
              
<script> 
  document.cookie = "session=test GDPR"; 
  document.cookie = "favorite_task=collect Data"; 
  document.cookie = "username=Diana C";
  document.cookie = "browser=chrome";
  document.cookie = "browser=chrome";
  document.cookie = "expires=Fri, 11 Dec 2030 14:00:00 UTC";
  function alertCookie() { alert(document.cookie); } 
  
 

  function setUsernameCookie(){
		let element = document.getElementById('username');
		document.cookie = "numeStudent="+element.value;
		let btn1 = document.getElementById('addUsernameCookie');
		btn1.style="display:none";
		document.getElementById('usernameCookie').innerHTML=element.value;
	}
  
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


  </script>


