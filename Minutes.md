IETF 120 HP-WAN side-meeting

Meeting host:
Sandy Zhang (zhang.zheng@zte.com.cn)
Peng Liu (liupengyjy@chinamobile.com)

Contact:
Quan Xiong (xiong.quan@zte.com.cn)
Kehan Yao (yaokehan@chinamobile.com)

notes:
https://notes.ietf.org/s/notes-ietf-120-HP-WAN-side-meeting

Minutes:

[Post Presentations there was a Open Discussion]

Joel M. Halpern (Ericsson)
The use case requirements listed are not exactly the same, and it is impossible to cover all usecases with one solution.
Problems cannot be analyzed based on a preset solution.
The current requirements are mixed together, and each requirement needs to be analyzed in layers to further clarify the problems that need to be solved.
This is not a problem related to routing area, it has more relationship with transport layer. The first thing is that the key point of routing area should be pointed out and focus on.

Jeffrey Zhang (Juniper)
The original MPLS network RSVP-TE has the concept of resource reservation. If SR is needed to meet these requirements, does it mean that resource reservation is brought back again?
Is it necessary to introduce multicast for communications between more than two sites?

Tim Chown (JISC)
There are many related scientific data transmission technology research works in academia and they are open. There are also related discussions in WLCG, which can be further checked.
Nick’s colleagues at ES-net wrote up the Science DMZ network - https://fasterdata.es.net/science-dmz/ - this is the same as the WLCG has evolved.
Detnet is not a consideration for solution now.

Daniel Huang (ZTE):
Agree with Joe’s point of view on demand Narrow Down. The sensitivity of HP-WAN services to delay, jitter, and packet loss is different from that of DetNet services. DetNet is a solution option, but it is not suitable for all scenarios from a cost perspective.
Other discussion: (Sorry the Name is missed, appreciated if the question provider will claim)
Why must the network be (almost) lossless, and what impact does packet loss have on these use cases?
Why can’t existing congestion control/QOS solutions, such as cube, BBR, etc., meet the needs?

Q&A
Q: Dirk Trossen (Huawei Technologies Duesseldorf GmbH): Telecom Supercomputing Express Line uses slicing technology and also mentions the need for statistical multiplexing. How do these two solutions coexist?

A: Huang Cancan (China Telecom): Supercomputing Express Line does not use dedicated lines. The access side adjusts the speed of specific user services at the OLT.

Q: Huang Guangping (ZTE): How sensitive is the DDM service to the transmission delay of the WAN segment? What is the incremental demand relative to the existing network capacity?

A: Richard YANG (Yale): DDM services are sensitive to end-to-end delay, but there is no clear delay threshold requirement.

Daniel King (Lancaster University)

Clearly something to continue to discuss here. I would like to see a dedicated mailing-list for following up after this meeting.
