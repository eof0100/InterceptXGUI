\# InterceptX GUI



\*\*InterceptX GUI\*\* is a Java-based HTTP proxy application with a graphical interface. It allows users to intercept, view, and analyze HTTP requests and responses between a browser and web servers in real-time.



---



\## Features



\- Intercepts HTTP (HTTPS not yet supported) traffic from your browser to any web server.

\- Displays full HTTP request and response headers in a GUI.

\- Captures response body:

&nbsp; - Text content (HTML, JSON, XML) is displayed directly.

&nbsp; - Binary content (images, PDF, ZIP, etc.) is summarized with size and MIME type.

\- Automatically decodes gzip-compressed responses.

\- Start and stop the proxy server directly from the GUI.

\- Logs all activity in a scrollable `JTextArea` window.

\- Simple port configuration for the proxy (default: 8080).



---



\## How It Works



1\. \*\*Start the Proxy\*\*: Click the "Start Proxy" button and specify a port.

2\. \*\*Browser Traffic Interception\*\*:

&nbsp;  - The proxy listens on the specified port.

&nbsp;  - When a browser sends an HTTP request, the proxy receives it.

3\. \*\*Forwarding Requests\*\*:

&nbsp;  - The proxy sends the request to the real server.

&nbsp;  - Headers and body are forwarded correctly, including POST/PUT data.

4\. \*\*Handling Responses\*\*:

&nbsp;  - The proxy receives the response from the server.

&nbsp;  - Text-based content is displayed in the GUI.

&nbsp;  - Binary content is logged with size and MIME type.

&nbsp;  - The response is forwarded back to the browser.

5\. \*\*Stop the Proxy\*\*: Click the "Stop Proxy" button to safely terminate the server thread.



---



\## How to Run



1\. Download `InterceptX.jar` from this repository.

2\. Open a terminal/command prompt.

3\. cd /path/to/InterceptXGUI

4\. Run the following command:



Linux or Windows:

java -jar InterceptX.jar

5. Configure your browser to use the proxy at the specified port number

6\. Intercepted traffic will appear live in GUI 




