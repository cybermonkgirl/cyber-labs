<h1>Reflected XSS into HTML context with nothing encoded</h1>

<h3><b>Step #1: Code Analysis</b></h3>
There is no encoding, the search element simply accepts the users input and reflects it on the result page. 
<img src= "https://github.com/cybermonkgirl/cyber-labs/blob/main/portswigger-labs/cross-site%20scripting/nothing-encoded/html.png" alt="Screenshot of HTML class 'search'">
<br>
<h3><b>Step #2: Exploit Vulnerability</b></h3>
Since there is no encoding, a basic xss input wil be used to test how inputs are processed. 
<img src="https://github.com/cybermonkgirl/cyber-labs/blob/main/portswigger-labs/cross-site%20scripting/nothing-encoded/basic-xss-script-tag.png" alt="<script>alert('xss');</script>">
<br>
</li><img src="https://github.com/cybermonkgirl/cyber-labs/blob/main/portswigger-labs/cross-site%20scripting/nothing-encoded/results_nothing-enoded.png" alt="xss alert pop up result[successful]">
