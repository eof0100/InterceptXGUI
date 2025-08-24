# InterceptX GUI

<p align="center">
  <img src="logo.png" alt="InterceptX Logo" width="150"/>
</p>

<h2 align="center">Java-Based HTTP Proxy with GUI</h2>

<p align="center">
  <b>InterceptX GUI</b> is a Java-based HTTP proxy application with a graphical interface.<br/>
  It allows users to intercept, view, and analyze HTTP requests and responses between a browser and web servers in real-time.
</p>

---

## ✨ Features

<ul>
  <li>Intercepts HTTP traffic from your browser to any web server (<b>HTTPS not yet supported</b>).</li>
  <li>Displays full HTTP request and response headers in a GUI.</li>
  <li>Captures response body:
    <ul>
      <li>Text content (HTML, JSON, XML) is displayed directly.</li>
      <li>Binary content (images, PDF, ZIP, etc.) is summarized with size and MIME type.</li>
    </ul>
  </li>
  <li>Automatically decodes gzip-compressed responses.</li>
  <li>Start and stop the proxy server directly from the GUI.</li>
  <li>Logs all activity in a scrollable <code>JTextArea</code> window.</li>
  <li>Simple port configuration for the proxy (default: <code>8080</code>).</li>
</ul>

---

## ⚙️ How It Works

<ol>
  <li><b>Start the Proxy:</b> Click the <code>Start Proxy</code> button and specify a port.</li>
  <li><b>Browser Traffic Interception:</b>
    <ul>
      <li>The proxy listens on the specified port.</li>
      <li>When a browser sends an HTTP request, the proxy receives it.</li>
    </ul>
  </li>
  <li><b>Forwarding Requests:</b>
    <ul>
      <li>The proxy sends the request to the real server.</li>
      <li>Headers and body are forwarded correctly, including POST/PUT data.</li>
    </ul>
  </li>
  <li><b>Handling Responses:</b>
    <ul>
      <li>The proxy receives the response from the server.</li>
      <li>Text-based content is displayed in the GUI.</li>
      <li>Binary content is logged with size and MIME type.</li>
      <li>The response is forwarded back to the browser.</li>
    </ul>
  </li>
  <li><b>Stop the Proxy:</b> Click the <code>Stop Proxy</code> button to safely terminate the server thread.</li>
</ol>

---

## ▶️ How to Run

1. Download <code>InterceptX.jar</code> from this repository.  
2. Open a terminal or command prompt.  
3. Navigate to the folder containing the JAR file:  

   ```bash
   cd /path/to/InterceptXGUI
