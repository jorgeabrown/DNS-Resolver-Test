# Information Gathering

### Control DNS Query Times (Averages)
Querying `google.com`

- **Flushed DNS:** 43 milliseconds
- **Filled DNS:** 31 milliseconds

### CloudFlare WARP DNS Query Times (Averages)
Querying `google.com`

- **Flushed DNS:** 25 milliseconds
- **Filled DNS:** 23 milliseconds

### Outcome / Lessons Learned: 
- CloudFlares WARP app significantly increased DNS query speed times compared to the control.
- It almost seems as if flushing the DNS had no effect, so I am wondering how that is possible.
- Installation of WARP added a net adapter with a description of "CloudFlare WARP Interface Tunnel"
- I am unsure how this adapter works, going to dig deeper and see what I can find out.
  - According to Copilot, the virtual network adapter added essentially acts as a bridge between
    the system and the WARP client software. It captures network traffic, encrypts it, and sends it
    to Cloudflares servers for processing. After, it routes the traffic back to its destination securely.
