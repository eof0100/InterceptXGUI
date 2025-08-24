<h1 style="margin-bottom:0">InterceptX GUI <span style="font-weight:400;">v1.0.0</span></h1>
<p style="margin-top:4px;color:#666;">Release date: 2025-08-24</p>

<hr/>

<h2>Overview</h2>
<p>
  <strong>InterceptX GUI</strong> is a Java-based HTTP proxy with a Swing GUI. It intercepts, displays, and forwards HTTP (HTTPS support coming) traffic between your browser and target servers, showing request/response headers and readable bodies in real time.
</p>

<div style="background:#f6f8fa;border:1px solid #d0d7de;border-radius:6px;padding:12px;">
  <p style="margin:0;"><strong>Heads up:</strong> The GitHub-generated “Source code (zip/tar.gz)” asset
  <em>does not contain Java source code</em>. It only includes the files present in this public repository (e.g., <code>InterceptX.jar</code> and <code>README.md</code>). The source code is private.</p>
</div>

<h2>What’s Included (Assets)</h2>
<ul>
  <li><strong>InterceptX.jar</strong> — runnable application</li>
  <li><strong>Source code (zip/tar.gz)</strong> — auto-generated archive of this repo contents (no Java sources)</li>
</ul>

<h2>Highlights</h2>
<ul>
  <li>Intercepts browser HTTP requests/responses (multiple concurrent connections)</li>
  <li>Displays all request/response headers</li>
  <li>Shows text bodies (HTML/JSON/XML); summarizes binary content only (MIME type &amp; size)</li>
  <li>Automatic <code>gzip</code> response decoding</li>
  <li>Start/Stop proxy from the GUI; configurable port (default <code>8080</code>)</li>
</ul>

<h2>Requirements</h2>
<ul>
  <li>Java 8 or newer (<code>java -version</code>)</li>
  <li>Network access to target servers</li>
  <li>Ability to set browser proxy to <code>localhost:&lt;port&gt;</code></li>
</ul>

<h2>How to Run</h2>

<h3>Windows</h3>
<ol>
  <li>Download <code>InterceptX.jar</code> from the Assets below.</li>
  <li>Open <strong>Command Prompt</strong> and change to the download folder:
    <pre><code>cd C:\Path\To\InterceptXGUI</code></pre>
  </li>
  <li>Run:
    <pre><code>java -jar InterceptX.jar</code></pre>
  </li>
</ol>

<h3>Linux</h3>
<ol>
  <li>Download <code>InterceptX.jar</code> from the Assets below.</li>
  <li>Open a <strong>Terminal</strong> and change to the download folder:
    <pre><code>cd /path/to/InterceptXGUI</code></pre>
  </li>
  <li>Run:
    <pre><code>java -jar InterceptX.jar</code></pre>
  </li>
</ol>

<h3>Configure Your Browser</h3>
<ol>
  <li>Set HTTP proxy to <code>localhost</code> and the port you entered in the app (default <code>8080</code>).</li>
  <li>Browse any site; traffic will appear in the InterceptX GUI window.</li>
</ol>

<h2>Notes &amp; Limitations</h2>
<ul>
  <li><strong>HTTP only</strong> — HTTPS interception is not yet supported.</li>
  <li>Large/binary bodies are not dumped into the GUI; they’re summarized (size + MIME).</li>
  <li>If the chosen port is in use, the app will show an error; pick a different port.</li>
</ul>

<h2>Changelog</h2>
<ul>
  <li><strong>v1.0.0</strong>
    <ul>
      <li>Initial public release of InterceptX GUI</li>
      <li>Request/response interception with header display</li>
      <li>Text body rendering + gzip decoding</li>
      <li>Binary content summary and basic logging</li>
    </ul>
  </li>
</ul>

<h2>Verification</h2>
<p>Checksum Verification:</p>
<pre><code>SHA256 (InterceptX.jar): 666E03B45CEC69561F2F90F3AF75A9FD7B40E3E7F60DF0F64ED3CC4C3FE6FE01</code></pre>

<h2>About the Developer</h2>
<p>
I am currently a Bachelor’s student in Computer Science at Eastern Washington University (EWU). 
I created <strong>InterceptX GUI</strong> out of my personal interest in computer security and networking, 
and as a hands-on project to deepen my understanding of Java, HTTP protocols, and proxy servers. 
This project is part of my journey to learn practical cybersecurity concepts and improve my programming skills.
</p>


<h2>Feedback</h2>
<p>This is my basic first release of InterceptX. Next goal is to support HTTPS and be able to intercept and edit request/response on the fly. Report issues or suggestions via the repository’s Issues tab. Thank you. </p>
