# DNS-Resolver-Test
This project is intended to test the speed of different DNS resolvers, specifically the default CDE lightband DNS resolver and Cloudflares 1.1.1.1 with WARP. Currently there are no records of CDE Lightbands resolver speed times, but currently Cloudflares product is #3 on the authoritative side of the house. 

DNS Speed Check Checklist
- [ ] Flush DNS Cache `ipconfig /flushdns`
- [ ] Test query time using CDE Resolver
- [ ] Test query time using Cloudflares Resolver
- [ ] Test query times with DNS cache now filled
- [ ] Record results
