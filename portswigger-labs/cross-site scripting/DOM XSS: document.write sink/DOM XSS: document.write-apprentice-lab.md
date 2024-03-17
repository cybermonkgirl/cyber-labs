<h1>DOM XSS in document.write sink using source location.search</h1>

<h3>Step #1: Code Analysis</h3>
The vulnerability in the provided code stems from its failure to validate and encode user input before incorporating it into the document.write function. This oversight exposes the application to cross-site scripting (XSS) attacks, as malicious users can inject arbitrary code into the HTML document by manipulating the query parameter.
<br>
<img src="https://github.com/cybermonkgirl/cyber-labs/blob/main/portswigger-labs/cross-site%20scripting/DOM%20XSS%3A%20document.write%20sink/image.png" alt="Screenshot of Search Function">
<br>
<h3>Step #2: Exploit Identified Vulnerability</h3>
