---
title: "In-Band Network Telemetry as a Service"
collection: publications
permalink: /publication/hp4_int
excerpt: 'A research project on adding profiling feature on HyPer4, a portable virtualization tool for P4 language.'
date: 2017-12-09
---
A research project on adding profiling feature on HyPer4, a portable virtualization tool for P4 language. Code: [Github](https://github.com/cwkenwaysun/hp4_INT)

Parter: [Mazhar Naqvi](https://github.com/mazhar-naqvi)

![p4int](https://chien-wei.github.io/files/hp4_int/p4int.png)  
Current solution for building INT-capable network on P4 programs.  

![hp4int](https://chien-wei.github.io/files/hp4_int/hp4int.png)  
Our solution that use HyPer4+INT.


## Abstract
Large and complex network environments consist of complex configurations. In-band network telemetry (INT) provides useful information that helps in network diagnostics. However, adding support for INT in network requires modifications in switch configurations. We extend HyPer4 to support INT such that network administrators are able to run unmodified P4 programs on HyPer4. At the same time, they can enjoy INT features from HyPer4 layer.

## Reference
[1] Barefoot Networks. P4 source routing. [https://github.com/p4lang/tutorials/tree/master/SIGCOMM_2015](https://github.com/p4lang/tutorials/tree/master/SIGCOMM_2015).  
[2] Barefoot Networks. p4factory. [https://github.com/p4lang/p4factory/tree/master/apps/int](https://github.com/p4lang/p4factory/tree/master/apps/int).  
[3] Bob Lantz Mininet Core Team. mininet. [https://github.com/p4lang/mininet](https://github.com/p4lang/mininet).  
[4] Bosshart, P., Daly, D., Gibb, G., Izzard, M., McKeown, N., Rexford, J., Schlesinger, C., Talayco, D., Vahdat, A., Varghese, G., and Walker, D. P4: Programming protocol-independent packet processors. SIGCOMM Comput. Commun. Rev. 44, 3 (July 2014), 87–95.  
[5] Kim, Changhoon et al. “In-band Network Telemetry via Programmable Dataplanes.” (2015).  
[6] Barefoot Networks. Changhoon Kim, Parag Bhide, Ed Doe, Hugh Holbrook, Anoop Ghanwani, Dan Daly, Mukesh Hira, Bruce Davie. In-band Network Telemetry (INT). [https://p4.org/assets/INT-current-spec.pdf](https://p4.org/assets/INT-current-spec.pdf).  
[7] Flux Research Group, University of Utah. Controller pro ject for HyPer4. [https://gitlab. flux.utah.edu/hp4/hp4-ctrl](https://gitlab.flux.utah.edu/hp4/hp4-ctrl).  
[8] Hancock, D., and van der Merwe, J. Hyper4: Using p4 to virtualize the programmable data plane. In Proceedings of the 12th International on Conference on Emerging Networking EXperiments and Technologies (New York, NY, USA, 2016), CoNEXT ’16, ACM, pp. 35–49.  
[9] McKeown, N., Anderson, T., Balakrishnan, H., Parulkar, G., Peterson, L., Rexford, J., Shenker, S., and Turner, J. Openflow: Enabling innovation in campus networks. SIGCOMM Comput. Commun. Rev. 38, 2 (Mar. 2008).  
