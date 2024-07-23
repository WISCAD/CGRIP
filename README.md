# CGRIP: Global Routing Congestion Analysis for Modern VLSI Design

Supported by **NSF award [1608040](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1608040&ActiveAwards=true&ExpiredAwards=true)**

CGRIP is a fast routing congestion analysis tool. It captures a number of factors that contribute to congestion in modern designs such as varying wire size and spacing at different metal layers, routing blockages, and virtual pins at different metal layers. It works with a flexible model of global routing which is an extension of the mathematical model given in GRIP. The model is based on regional minimization of overflow, as an objective introduced to quickly identify the locations of the congested regions which are specified by an input resolution parameter. A further extension (LCGRIP in ISPD'13) introduces vertex capacity and non-uniform gcell generation to reduce mismatch with detailed routing caused by local nets.

A simple variation of CGRIP, called coalesCgrip, was used to judge the [ISPD 2011 contest](http://www.ispd.cc/contests/11/ispd2011_contest.html) and was mentioned in this [EETimes article](https://www.eetimes.com/ISPD-reveals-3-D--maskless-lithography-trends-/). Information about the procedures of CGRIP and coalesCgrip and their comparison are given in the paper and presentation slides included.

**Related Publications:**

H. Shojaei, A. Davoodi, and J. Linderoth, "Congestion analysis for global routing via integer programming", in Int'l Conf. on Computer-Aided Design (ICCAD'11), pp. 256-262, November 2011. 

H. Shojaei, A. Davoodi, and J. Linderoth, "Planning for local net congestion in global routing", in Int'l Symp. on Physical Design (ISPD'13), pp. 85-92, March 2013. 

**CGRIP Variations included:**

CGRIP V2.0 binary (has additional features to specify individual bounding-box constraint to control how scenic each net is routed, along with bounds on the number of rip-up and reroute iterations and on the execution runtime)

CGRIP-noCPLEX V2.0 binary (does not require CPLEX installation but has less improvements since integer programming-based optimizations are disabled)

coalesCgrip V1.3 binary (CGRIP_300_900_1.exe)

coalesCgrip V1.3 library: (available compilations are gcc 4.1.2 and gcc 4.4.3)

All the above variations (except CGRIP-noCPLEX) evoke the IBM ILOG CPLEX optimization tool. A free license for CPLEX can be obtained from the IBM ILOG CPLEX Optimization Studio for Academics. Please download the following two files from the IBM website to install and use CPLEX: (a) cplex_studio122.acad.linux-x86.bin (b) access.ilm.
