## ACTIVITATE PRACTICA: CRISTIAN DIANA MARIA, TSAeA, sem. II, 2020-2021

<body> 
  <div class="row">
	<b>Introduceti numele de utilizator:</b>
  	<input id="username" type="text" class="form-control " placeholder="username" aria-label="username">
  </div>
	
  <button class="btn" type="button" id="addUsernameCookie" onclick="setCookies();parseAndDisplayCookies()">Seteaza username COOKIE</button>
  <br>
  <b>Nume utilizator: </b><span id="usernameCookie"> </span>
  <b>Versiune browser : </b><span id="browserVersionCookie"> </span>
	<hr>
	<div>
  <b><a href="https://didatec-my.sharepoint.com/:w:/r/personal/cristian_is_diana_utcluj_didatec_ro/_layouts/15/Doc.aspx?sourcedoc=%7B06670782-017A-443A-B220-CFC0D0005D1C%7D&file=DPIA_CristianDianaMaria.docx&action=default&mobileredirect=true">Analiza DPIA</a></b>
	</div>
	<hr>
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

</body>
              
<script>
 	   function setCookies(){
		var usernameElement = document.getElementById('username');
		document.cookie = "usernameCookie=" + usernameElement.value +'; ';
		document.cookie = "browserCookie=" + navigator.userAgent ; //detectBrowser();
		}
		
	   function parseAndDisplayCookies(){
			var username = getCookie("usernameCookie");
			var browser = getCookie("browserCookie");
			document.getElementById("usernameCookie").innerHTML = username;
			document.getElementById("browserVersionCookie").innerHTML = browser;
	   }

		
	   function retrieveUsernameFromCookie(){
		 var cookies = document.cookie.split("; ");
		 var usernameCookie = cookies[0]; 
		 var browsewrCookie = cookies[1];
		 console.log(cookies);
		 console.log(usernameCookie);
		 console.log(browsewrCookie);
		 }
	
		//gets the type of browser (stackoverflow)
		function detectBrowser() { 
			if((navigator.userAgent.indexOf("Opera") || navigator.userAgent.indexOf('OPR')) != -1 ) {
				return 'Opera';
			} else if(navigator.userAgent.indexOf("Chrome") != -1 ) {
				return 'Chrome';
			} else if(navigator.userAgent.indexOf("Safari") != -1) {
				return 'Safari';
			} else if(navigator.userAgent.indexOf("Firefox") != -1 ){
				return 'Firefox';
			} else if((navigator.userAgent.indexOf("MSIE") != -1 ) || (!!document.documentMode == true )) {
				return 'IE';
			} else {
				return 'Unknown';
			}
		} 
	
		//w3schools
		function getCookie(cname) {
		  var name = cname + "=";
		  var decodedCookie = decodeURIComponent(document.cookie);
		  var ca = decodedCookie.split(';');
		  for(var i = 0; i <ca.length; i++) {
			var c = ca[i];
			while (c.charAt(0) == ' ') {
			  c = c.substring(1);
			}
			if (c.indexOf(name) == 0) {
			  return c.substring(name.length, c.length);
			}
		  }
		  return "";
	}
	
  </script>


