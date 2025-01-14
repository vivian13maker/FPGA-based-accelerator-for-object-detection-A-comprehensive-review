# Pseudorandom number generator based on a 5D hyperchaotic four-wing memristive system and its FPGA implementation

## ABSTRACT

Pseudorandom numbers are widely used in information encryption, spread spectrum communication and other science and technology and engineering fields. Because chaos is very sensitive to the initial conditions and has good inherent pseudo-random characteristics, the research of pseudorandom number generator (PRNG) based on a chaotic system becomes a new beneficial exploration. This paper presents a FPGA PRNG based on a 5D hyperchaotic four-wing memristive system (HFWMS). The 5D HFWMS has multiline equilibrium and three positive Lyapunov exponents, which indicates that the system has very complex dynamic behavior. On this basis, a FPGA PRNG based on the 5D HFWMS is proposed. The proposed PRNG is implemented in VHDL language, modeled and simulated on Vivado 2018.3 platform, and synthesized by FPGA device ZYNQ-XC7Z020 on Xilinx. The post-processing module consists of 16 linear shift registers and 15 levels XOR chain. The maximum operating frequency is 138.331 MHz and the speed is 15.37 Mbit/s. The random bit sets generated by PRNG are further verified by NIST 800.22 statistical standard. The security is analyzed by dynamic degradation, keyspace, key sensitivity and correlation. Experiments show that the design can be applied to various embedded password applications.

## Contribution

This paper presents a PRNG-HFWMS based on FPGA. The 5D HFWMS has very complex dynamic behavior, which has multi-line equilibrium and three positive Lyapunov exponents, so it is very suitable for the design of PRNG. On this basis, a new PRNG based on the 5D HFWMS is proposed. The post-processing module consists of 16 shift registers and 15 levels of XOR chains. Finally, the PRNG test of the designed chaotic oscillator shows that the maximum operating frequency is 138.331 MHz and the speed is 15.37 Mbit/s. The random bit sets generated by PRNG has been further verified
by NIST 800.22 statistical standard, which proves that the proposed design scheme can be applied to various embedded cryptography applications.

## Main experimental analysis

When the system parameters are set as a = 1, b = 1, c = 0.7,m = 1, d = 0.2, e = 0.1, n = 0.01, and the initial conditions are (1,−1, 1, 1, 1), system behaves as a four-wing hyperchaotic attractor, and its phase portrait is shown in Fig. 1a. Figures 2 and 3 are the LE spectrum and bifurcation diagram of system with respect to parameter a respectively. From Fig. 2, it can be seen that the system has three positive LEs, especially when a = 0.78, the five LEs are LE1 = 0.1712, LE2 = 0.0907, LE3 = 0.0107, LE4 = 0, LE5 = −2.3243. From the bifurcation diagram in Fig. 3, it can be seen that the system has periodic, chaotic and hyperchaotic phenomena. When the system parameters of system (1) are selected as a = 11, b = 1, c = 0.7,m = 1, d = 0.2, e = 0.1, n = 0.01, and the initial conditions are selected as (0, 1, 0, 0, 0), the system presents a two-wing hyperchaotic attractor, as shown in Fig. 1b.

![image-20210913231927824](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913231927.png)

## Performance

![image-20210913232005577](https://gitee.com/feiyipengfei/pic-md1/raw/master/20210913232005.png)

