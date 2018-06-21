<h1>This is the Cheetsheet for url rewriting</h1>

<h2>Regex Characters</h2>
<ul>
<li>. (any character)</li>
<li>* (zero of more of the preceding)</li>
<li>+ (one or more of the preceding)</li>
<li>{} (minimum to maximum quantifier)</li>
<li>? (ungreedy modifier)</li>
<li>! (at start of string means "negative pattern")</li>
<li>^ (start of string, or "negative" if at the start of a range)</li>
<li>$ (end of string)</li>
<li>[] (match any of contents)</li>
<li>- (range if used between square brackets)</li>
<li>() (group, backreferenced group)</li>
<li>| (alternative, or)</li>
<li>\ (the escape character itself)</li>

</ul>




<h2>Flags</h2>
<ul>
<li>C (chained with next rule)</li>
<li>CO=cookie (set specified cookie)</li>
<li>E=var:value (set environment variable var to value)</li>
<li>F (forbidden - sends a 403 header to the user)</li>
<li>G (gone - no longer exists)</li>
<li>H=handler (set handler)</li>
<li>L (last - stop processing rules)</li>
<li>N (next - continue processing rules)</li>
<li>NC (case insensitive)</li>
<li>NE (do not escape special URL characters in output)</li>
<li>NS (ignore this rule if the request is a subrequest)</li>
<li>P (proxy - i.e., apache should grab the remote content specified in the substitution section and return it)</li>
<li>
PT (pass through - use when processing URLs with additional handlers, e.g., mod_alias)</li>
<li>R (temporary redirect to new URL)</li>
<li>R=301 (permanent redirect to new URL)</li>
<li>QSA (append query string from request to substituted URL)</li>
<li>S=x (skip next x rules)</li>
<li>T=mime-type (force specified mime type)</li>


</ul>


<h2>VARIABLE_NAME</h2>

<ul>
<li>
  HTTP Headers
  <ul>
    <li>HTTP_USER_AGENT</li>
    <li>HTTP_REFERER</li>
    <li>HTTP_COOKIE</li>
    <li>HTTP_FORWARDED</li>
    <li>HTTP_HOST</li>
    <li>HTTP_PROXY_CONNECTION</li>
    <li>HTTP_ACCEPT</li>
  </ul>
</li>
<li>
  Connection Variables
  <ul>
        <li>REMOTE_ADDR</li>
        <li>REMOTE_HOST</li>
        <li>REMOTE_USER</li>
        <li>REMOTE_IDENT</li>
        <li>REQUEST_METHOD</li>
        <li>SCRIPT_FILENAME</li>
        <li>PATH_INFO</li>
        <li>QUERY_STRING</li>
        <li>AUTH_TYPE</li>
  </ul>
</li>
<li>
    Server Variables
    <ul>
       <li>DOCUMENT_ROOT</li>
       <li>SERVER_ADMIN</li>
       <li>SERVER_NAME</li>
       <li>SERVER_ADDR</li>
       <li>SERVER_PORT</li>
       <li>SERVER_PROTOCOL</li>
       <li>SERVER_SOFTWARE</li>
    </ul>
</li>
<li>
    Dates and Times
    <ul>
        <li>TIME_YEAR</li>
        <li>TIME_MON</li>
        <li>TIME_DAY</li>
        <li>TIME_HOUR</li>
        <li>TIME_MIN</li>
        <li>TIME_SEC</li>
        <li>TIME_WDAY</li>
        <li>TIME</li>
    </ul>
</li>
<li>
    Special Items
    <ul>
        <li>API_VERSION</li>
        <li>THE_REQUEST</li>
        <li>REQUEST_URI</li>
        <li>REQUEST_FILENAME</li>
        <li>IS_SUBREQ</li>
    </ul>
</li>
</ul>

PS. taken from https://www.addedbytes.com/blog/url-rewriting-for-beginners
