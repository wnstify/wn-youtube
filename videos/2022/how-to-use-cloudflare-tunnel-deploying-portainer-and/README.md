# How to use Cloudflare Tunnel | Deploying Portainer and WordPress stack

[![Watch on YouTube](https://img.youtube.com/vi/G_PqTyeZCWk/maxresdefault.jpg)](https://www.youtube.com/watch?v=G_PqTyeZCWk)

**Published:** September 21, 2022

[Watch on YouTube](https://www.youtube.com/watch?v=G_PqTyeZCWk)

---

## Description

In this demonstration, I am about to show you the power of Cloudflare Tunnel Service.  
We will be creating a fresh VPS server, and installing Cloudflared, Portainer, and our WordPress stack.  

Cloudflare Tunnel (Cloudflared) is a part of Cloudflare Zero Trust product/service, which is completely free for up to 50 users. 
https://www.cloudflare.com/products/tunnel/ 
https://www.cloudflare.com/products/zero-trust/ 

All applications proxyfied in tunnels are running on a separate enterprise network. They are separated from basic CDN service networks while offering the same benefits like DDOS Protection, IP Filtering, Blocking common threats, and more.

Please watch my previous video, where I set up a brand new account for Zero Trust platform:
https://www.youtube.com/watch?v=5uq3NPpswek&t=

The most beneficial thing about Cloudflared, is that you don't need your server to be open for public. That means port 80, 443, or any other ports except port 22 can be closed without issues. 

All inbound and outbound connection is between Cloudflare and your origin server and no one else can connect to your server.  

My terminal of choice is Termius.
It has many great benefits, that make my life much easier.  It can sync all of your servers with SSH keys, snippets, and more. 
https://termius.com/

About Webnestify
Imagine a world where you can focus on your business and less time maintaining your cloud infrastructure. With Webnestify cloud-based solutions, we provide customized solutions for all types of companies to meet their needs; no matter how big or small they may be!

https://webnestify.cloud https://www.trustpilot.com/review/webnestify.cloud
