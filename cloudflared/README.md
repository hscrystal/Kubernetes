Ref. https://developers.cloudflare.com/cloudflare-one/tutorials/many-cfd-one-tunnel/
Associate your Tunnel with a DNS record
Go to the Cloudflare dashboard.
Go to the DNS tab.
Now create a CNAME targeting .cfargotunnel.com. In this example, the tunnel ID is ef824aef-7557-4b41-a398-4684585177ad, so create a CNAME record specifically targeting ef824aef-7557-4b41-a398-4684585177ad.cfargotunnel.com.
You can also create multiple CNAME records targeting the same Tunnel, if desired.

Alternatively, you can perform this step from the command line by running 
cloudflared tunnel route dns <tunnel> <hostname>. 
For example, cloudflared tunnel route dns example-tunnel tunnel.example.coms

Ref. https://nicwortel.nl/blog/2022/continuous-deployment-to-kubernetes-with-github-actions
    https://www.robert-jensen.dk/posts/2024-external-dns-with-cloudflare/