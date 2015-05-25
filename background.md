# Language-theoretic security: A Literature Primer

prepared by Michael E. Locasto for the EDURange project.

LangSec (https://langsec.org) is a set of principles and ideas that attempt to provide a structured, coherent, and meaningful 
explanation for the existence of many of the most proliferate classes of software bugs and errors.

Like most ideas, LangSec itself is not entirely new, and has roots in many different parts of the traditional academic
and hacker literature.  In this file, I will list some papers that helped influence my own thinking on LangSec-related 
concepts before I even knew there was a "LangSec."  This list is by no means complete or exhaustive: it is a record of 
my own personal journey toward LangSec's formulation and exposure by L.S., M.P., and S.B.  Papers that I list here
have some element of weird machines or LangSec.  In many cases, I suspect that the authors of each paper were conciously
attempting to express some rigorous basis for their system or security model or mechanism; while the focus of the paper
may have been on some specific security problem (e.g., stopping the spread of Internet worms), the general nature of 
the problem of reliably recognizing input languages so permeates the discipline that most good systems security work
necessarily encounters LangSec in one form or another.

Why do things break?

Perhaps because they are attempting to do something fundamentally impossible.
The problem is that we have not spent sufficient effort in defining the boundary between “useful computation with limited 
computational power” (as a way of minimizing the vuln. surface) and “arbitrarily powerful computation subject to exploit.”

#Weird Machines

What is a "weird" "machine", and why should you care?

    weird : unexpected, latent functionality arising from the hidden or composed artifacts in your actual computing environment
    machine : actually quite structured and principled; may be "strange" but not ad hoc


Jedidiah R. Crandall, Zhendong Su, S. Felix Wu, and Frederic T. Chong. 
On Deriving Unknown Vulnerabilities from Zero-Day Polymorphic and Metamorphic Worm Exploits. 
In the proceedings of the 12th ACM Conference on Computer and Communications Security (CCS 2005). 
Alexandria, Virginia. November 2005.



Vigilante "Vigilante: End-to-End Containment of Internet Worms"
VSEF


    traditional return-to-libc: "Getting around non-executable stack (and fix)" Solar Designer http://www.clip.dia.fi.upm.es/~alopez/bugs/bugtraq2/0287.html
    return-to-libc: Nergal, "Advanced return-into-lib(c) Exploits: PaX Case Study," Phrack 58:4
    Return-oriented programming: The Geometry of Innocent Flesh on the Bone: Return-into-libc without Function Calls (on the x86) Hovav Shacham. In Proceedings of CCS 2007, pages 552–561. ACM Press, Oct. 2007. http://cseweb.ucsd.edu/~hovav/papers/s07.html


    Thomas Dullien and Halvar Flake "Exploitation and State Machines" PDF
    F. B. Schneider. Enforceable Security Policies. ACM Transactions on Information and System Security, 2(4), Mar. 2000.
    A Language-Based Approach to Security. Fred B. Schneider, Greg Morrisett, and Robert Harper2


    Insertion, Evasion, and Denial of Service: Eluding Network Intrusion Detection by Thomas H Ptacek and Timothy M. Newsham
    Network Intrusion Detection: Evasion, Traffic Normalization, and End-to-End Protocol Semantics. Mark Handley and Vern Paxson and Christian Kreibich USENIX paperhtml


packet-in-packet


    http://travisgoodspeed.blogspot.ca/2011/09/remotely-exploiting-phy-layer.html
    WOOT 2011 paper: http://www.usenix.org/events/woot11/tech/final_files/Goodspeed.pdf


# Misc. Links


    http://www.darkreading.com/vulnerability/taming-bad-inputs-means-taking-aim-at-we/240152171
    http://programmingisterrible.com/post/42215715657/postels-principle-is-a-bad-idea
    Programming with Nothing: http://experthuman.com/programming-with-nothing
    Learning to classify vulns: http://dl.acm.org/citation.cfm?doid=1835804.1835821
    PHY layer hacking: http://2012.hackitoergosum.org/blog/schedule/talks#Strangeand
    Catastrophic backtracking in regular expressions http://t.co/KWVDhLyI
    From Buffer Overflows to Weird Machines
    Cyberpatterns
    The Halting Problems of Network Stack Insecurity
    Security Applications of Formal Language Theory
    Packets in Packets (Goodspeed)
    Vulnerable Compliance (Geer)
    IDS Evasion Attacks (Ptacek and Newsham)
    Traffic Normalization (Handley)
    Crandall CCS 2005
    http://www.isg.rhul.ac.uk/tls/
    travis goodspeed: "Remotely Exploiting the PHY Layer"
        http://travisgoodspeed.blogspot.ca/2011/09/remotely-exploiting-phy-layer.html
        WOOT 2011 paper: http://www.usenix.org/events/woot11/tech/final_files/Goodspeed.pdf
    https://www.usenix.org/conference/woot11/packets-packets-orson-welles-band-signaling-attacks-modern-radios
        http://www.phrack.org/issues.html?issue=68&id=4&mode=txt (see 0x06, "How I misunderstood digital radio; or, "Weird machines" are in radio, too!" by M.Laphroaig pastor@phrack )

    http://www.microsoft.com/typography/otspec/featuretags.htm
    evading AV: http://blog.endpoint.com/2013/01/evading-anti-virus-metasploit.html
    http://programmingisterrible.com/post/42432568185/how-to-parse-ruby
    packet of death: http://appliance.cloudshark.org/news/cloudshark-in-the-wild/intel-packet-of-death-capture/
    blocking content based on executable env: http://arstechnica.com/security/2013/01/firefox-to-block-content-based-on-java-reader-and-silverlight/
    recognize a dialup? i.imgur.com/Q3lKIr1.jpg
    http://www.johndcook.com/blog/2013/02/21/can-regular-expressions-parse-html-or-not/
    "evil" code: http://erratasec.blogspot.ca/2013/03/the-debate-over-evil-code.html
