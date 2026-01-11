# Setting Up Runcloud Server | Best Practices | Part 1

[![Watch on YouTube](https://img.youtube.com/vi/ZAn8_YalJSM/maxresdefault.jpg)](https://www.youtube.com/watch?v=ZAn8_YalJSM)

**Published:** September 11, 2022

[Watch on YouTube](https://www.youtube.com/watch?v=ZAn8_YalJSM)

---

## Description

This is a part 1 of series, how to work with Runcloud.

This video will walk you through setting up your Runcloud server.  I tried to keep everything simple and it only cover basics and not advanced hardening techniques. 

Before installing agent, update your server and set your timezone with following commands:

apt update && apt upgrade -y
timedatectl set-timezone Europe/London

1. Make sure to properly configure your hardware-level firewall inside of an administration panel from your VPS provider (some VPS providers do not provide HW-level firewalls).  

2. Open only the necessary ports that you need (80, 443) and harden your port 22 with dedicated IP, if you have one. If not, keep port 22 open.  

3. Open port 34210/TCP (RunCloud agent) and whitelist the following IP addresses: 52.52.156.27 54.215.67.177  

4. Perform manual installation and backup MySQL credentials from a terminal, after installation finishes.  

5. In your RunCloud dashboard, create a system user and create a strong and complicated password.  

6. Disable root login and if you have your own SSH key, upload it and disable password authentification.  

7. Add your integrations of choice. I highly recommend using Cloudflare for managing all your domains for easy integration.   

8. Set up your preferred notification channel (email, Slack, or Telegram).

If you want, you can limit ports 80 and 443 to only communicate with Cloudflare. You will need to add Rich Rules for each port in Security settings.

Here are all Cloudflare IPs
https://www.cloudflare.com/ips/

About Webnestify
Imagine a world where you can focus on your business and less time maintaining your cloud infrastrucure. With Webnestify cloud based solutions, we provide customized solutions for all types of companies to meet their needs; no matter how big or small they may be!

https://webnestify.cloud
https://www.trustpilot.com/review/webnestify.cloud
