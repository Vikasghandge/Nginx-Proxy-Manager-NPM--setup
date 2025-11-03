# Nginx-Proxy-Manager-NPM--setup

## Configure Your Domain in Nginx Proxy Manager
Once you have NPM running (http://<server-ip>:81), do this:   access with your serverIP:81 

## 1️⃣ Log in to NPM dashboard
URL: http://<your-server-ip>:81
Default login:

```
Email: admin@example.com
Password: changeme

```

## 2️⃣ Add a New Proxy Host
Go to: Hosts → Proxy Hosts → Add Proxy Host
Now fill in:

Domain Names:                               [your domain name]  example.                      skilllab.duckdns.org 
Scheme            http
Forward Hostname / IP                        127.0.0.1     or container_name
Forward Port                                    80

## 3️⃣ SSL Configuration (Optional but Recommended)
If your DuckDNS domain is public and reachable:

Go to the SSL tab

Choose Request a new SSL Certificate

Enable:

✅ “Force SSL”

✅ “HTTP/2 Support”

Click Save

NPM will automatically get a free Let’s Encrypt SSL certificate.









