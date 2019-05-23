DWeb Camp 2019 // Open Dialogue Call // May 16
==============================================

**These notes will be published publicly**

DWeb Camp [Open Dialogue calls](https://github.com/dweb-camp-2019/organizing#open-dialogue-calls) are a space for you to ask us logistical questions, bounce your project ideas off of us (and each other!), and maybe even find other collaborators to work on a project.

## Helpful Links

- [Website](https://dwebcamp.org)
- [GitHub](https://github.com/dweb-camp-2019)
- [Chat](https://riot.im/app/#/room/#decentralizedweb-general:matrix.org)

## Participants

- Mai
    - people's open
- Wendy
    - director of Partnerships; IA-- Executive Producer of DWeb Camp
- Mark Nadal
    - GUN protocol which is used by IA
    - live scheduling software at Camp
- Ben
    - toronto mesh / coordinating mesh net at dweb 
- Jay Carpenter
    - desert blockchain in arizona & desert blockchain camp
    - build a blockchain with newspapers
- Talbert
- dcrocker
- Dylan Reibling
    - documentary film maker; interested in decentralization & blockchain
    - Interested in decentralized video
- Riley

## Notes

- Projects
    - scheduling software (mark) to enable spontaneous events to emerge
    - solar cooking
    - wellness: mushroom innoculation, yoga, breathwork, etc.
    - conservation: discussions re: offgrid power and networks
    - Secure Scuttle Butt
    - Focus on projects based on what is possible under circumstances in which power/connectivity access is difficult
- Spaces
    - 3 zones: hacking (indoor), wellness (dome), forum (outdoor space)
- Video Projects
    - Internet Archive, DTube, Alexandria, work on projects that are examples of blockchain-based video services
- Distinction
    - Mark
        - Values of blockchain as being Randian => greed
        - Values of cryptocurrency => privacy
        - Values of decentralization => openness/freedom
    - Ben
        - Decentralization: are we talking about application layer or network layer?
        - Are we talking about decentralized protocols? governance? knowledge?
        - >> We want DWeb Camp to be a space where we hold these conversations
    - Wendy
        - The projects will run the gambit: This event will bring people from all kinds of philosophies around decentralization
        - It can be technical, creative, etc.
- Protocols
    - IP and not IP-based protocols and devices
        - Disaster Radio, LoRa protocol
    - Libp2p
    - Also DAM: https://gun.eco/docs/DAM
    - It is possible to operate without IP, but most of them do
    - Mainstream p2p protocols still rely on IP, even IPFS
    - Some support multicast, but often they cannot cross that boundary if connected to other servers (?)
- Internet access
    - We currently only have 40 Mbps, but may have a few 100 Mbps available but not yet guaranteed. We will definitely have a local mesh
    - Ben
        - Mdns allows peering through multicast (like Apple TV discoverable across a home)
            - Network Address Translation (NAT): Networks being in their own NATs, with private IP addresses. 
            - NAT broadcasts don't cross over the Layer 3 boundaries
            - It's easy to do p2p applications at home (like SSB or IPFS nodes) and have them find themselves without much bootstrapping
            - Client isolation: If people want to isolate devices for security reasons
    - Mark
        - How do we traverse the network if we don't have Internet?
        - I'd like to be able to daisy-chain connection across Wi-Fi towers, and emit multicast messages across these Wi-Fi routers
    - Ben
        - 1) We could run the entire camp as a home network
            - As if we were patching a whole network of ethernet cables together
            - It's a bit cheating because it's doesn't resemble the real internet
        - 2) Layer 3 network protocol: Babel
            - Two towers become boundaries where multicast packets don't cross
            - Addresses problems
                - 1. NATting problem - colliding IP addresses between public + private IP
                    - We can assign a pan-public IP address to all the devices, they would be globally unique among the campers
                - 2. Automatic discovery won't happen
    - Mark: Who assigns the IP address for that network?
    - Ben: There would have to be a DHCP server
        - Each tower would have a DHCP server, and that would assign IP addresses for those devices
        - There will be opportunities to test it, during the build
    --Mark: Can we have a captive portal (like at a starbucks) where you can see which IP addresses are in the area?
