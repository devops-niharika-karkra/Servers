# Forward Proxy
Apache can act as forward proxy. In this setup, clients in an internal network route their outgoing internet traffic through Apache to enforce
security policies, filter content, or cache external resources.

<img width="686" height="461" alt="forward-proxy" src="https://github.com/user-attachments/assets/c08c0330-bbb5-4c16-9371-2d48333936af" />

As represented in this diagram, the proxy server resides in between system and the internet. 
**_For Example:_** if you are opening the www.example.com then the servers of example will only know that request is coming from proxy server 
so that way it hides your identity.
