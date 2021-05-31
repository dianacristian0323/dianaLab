## COOKIES

<body onload="insertText();"> 
  <div class="row">
  	<input id="username" type="text" class="form-control " placeholder="username" aria-label="username">
  </div>
	<table>
        <tr>
            <td id="td1"></td>
        </tr>
    </table>
<br>
   <button class="btn" type="button" id="addUsernameCookie" onclick="setUsernameCookie()">Salveaza</button>
  <br>
  <b>Nume utilizator:</b><span id="usernameCookie"> </span>
  <br>
 <b>Versiune browser:</b><span id="browserVersionCookie"> </span>
  <br>
	  <p><b>Nota de informare:</b></p>
	<p><b>NOTĂ DE INFORMARE PRIVIND PROTECŢIA DATELOR PERSONALE</b></p>
<p>Conform cerinţelor Legii nr. 677/2001 pentru protecţia persoanelor cu privire la prelucrarea datelor cu caracter personal şi libera circulaţie a acestor date, modificată şi completată şi ale Legii nr. 506/2004 privind prelucrarea datelor cu caracter personal şi protecţia vieţii private în sectorul comunicaţiilor electronice, Universitatea Tehnică din Cluj Napoca are obligaţia de a administra în condiţii de siguranţă şi numai pentru scopurile specificate, datele personale pe care ni le furnizaţi despre dumneavoastră, un membru al familiei dumneavoastră ori o altă persoană.</p>
<p>Scopul colectării datelor este: gestionarea calității de student în cadrul UTCN și gestionarea comunicării între UTCN si Universitatea din UK pentru transferul studentului spre UK și înapoi dar și pentru revendicarea rezultatelor obținute de acesta după parcurgerea stagiului acolo. 
Sunteţi obligat(ă) să furnizaţi datele, acestea fiind necesare pentru identificarea dumneavoastră ca student al Universității Tehnice din Cluj Napoca. 
Refuzul dvs. determină imposibilitatea efectuării stagiului (sfârșitul stagiului /anularea stagiului). Implicit, dacă în timpul stagiului nu veți mai fi de acord cu prelucrarea datelor cu caracter personal, nu vom mai putea colecta rezultatele dumneavoastră obținute în urma efectuării stagiului ceea ce va conduce la nerecunoașterea acestuia ca activitate educațională. </p>
<p>Informaţiile înregistrate sunt destinate utilizării de către operator şi sunt comunicate numai următorilor destinatari: Universitatea Tehnică din Cluj Napoca (Facultatea de Electronică, Telecomunicații și tehnologia informației, Master eActivități), Departamentul Erasmus  din UTCN, ambasada UK în Romania (pentru formalitățile necesare survenite în urma faptului că UK nu mai face parte din UE). 
Conform Legii nr. 677/2001, beneficiaţi de dreptul de acces, de intervenţie asupra datelor, dreptul de a nu fi supus unei decizii individuale şi dreptul de a vă adresa justiţiei. Totodată, aveţi dreptul să vă opuneţi prelucrării datelor personale care vă privesc şi să solicitaţi ştergerea datelor. Pentru exercitarea acestor drepturi, vă puteţi adresa cu o cerere scrisă, datată şi semnată la Biroul pentru Protectia Datelor cu Caracter Personal. De asemenea, vă este recunoscut dreptul de a vă adresa justiţiei. 
Datele dumneavoastră vor fi transferate în UK, în vederea stabilirii detaliilor legate de stagiul de mobilitate pe care îl veți avea. </p>
<p>Dacă unele din datele despre dumneavoastră sunt incorecte, vă rugăm să ne informaţi cât mai curând posibil.</p>

  <br>
	<div>
  <b><a href="https://didatec-my.sharepoint.com/personal/cristian_is_diana_utcluj_didatec_ro/_layouts/15/doc.aspx?sourcedoc={8cb11dbf-1ff3-4dbf-97f9-72e446aab3e6}&action=edit">Analiza DPIA</a></b>
	</div>

	
  
</body>
              
<script type="text/javascript"> 
	function insertText () {
    document.getElementById('td1').innerHTML = "Some text to enter";
}
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


