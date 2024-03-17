<h1>DOM XSS in document.write sink using source location.search</h1>

The search functionality accepts uses input, and fails to validate and encode user input before incorporating it into the document.write function. This vulnerability allows malicious codes to be injected and executed. 

<h2>Vulnerability Details:</h2><br>
<b>Vulnerability Type:</b> DOM XSS<br>
<b>Affected Endpoint:</b> Search Functionality<br>
<b>Vulnerable Parameter:</b> <b><i>`search`</i></b> paramater in the URL query string<br><br>
<img src="https://github.com/cybermonkgirl/cyber-labs/blob/main/portswigger-labs/cross-site%20scripting/DOM%20XSS%3A%20document.write%20sink/screenshot-search-functionality.png" alt="Screenshot of Search Function">
<br>

<h2>Proof of Concept(POC)</h2><br>
<h3>XSS Payload</h3>
<img src="https://github.com/cybermonkgirl/cyber-labs/blob/74b6fc820a9d2dfd5c93b9688056244890f2f77f/portswigger-labs/cross-site%20scripting/DOM%20XSS%3A%20document.write%20sink/document.write-payload.png" alt="XSS Payload">
<br>
<h3>Exploitation</h3>
<img src="https://github.com/cybermonkgirl/cyber-labs/blob/950d311791e480a8041aa8a80c7b7436fffe547e/portswigger-labs/cross-site%20scripting/DOM%20XSS%3A%20document.write%20sink/documen-write-result.png" alt="results - XSS alert pop-up">
