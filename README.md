# read_gadget_MBII
This is a python code to read the binary output (snapshot) of Massive Black II simulation of Khandai et al <br />
<br />
MBII Blocks:<br />
1.position (type 0, 1, 4, 5)<br />
2.velocity (type 0, 1, 4, 5)<br />
3.id       (type 0, 1, 4, 5)<br />
4.masses   (type 0, 4, 5)<br />
5.internal energy (type 0)<br />
6.density (type 0)<br />
7.electron abundance (type 0)<br />
8.HI abundance (type 0)<br />
9.smoothing length (type 0)<br />
10.star formation rate (type 0)<br />
11.stellar formation time (type 4)<br />
12.metallicity (type 0, 4)<br />
13.bh_mass (type 5)<br />
14. bh_modot (type 5)<br />
15.bh_nprogs (type 5)<br />
<br />
<br />
1.position (type 0, 1, 4, 5)<br />
2.velocity (type 0, 1, 4, 5)<br />
3.id       (type 0, 1, 4, 5)<br />
4.masses   (type 0, 4, 5)<br />
5.internal energy (type 0)<br />
6.electron abundance (type 0)<br />
7.HI abundance (type 0)<br />
8.smoothing length (type 0)<br />
9.star formation rate (type 0)<br />
10.stellar formation time (type 4)<br />
11.metallicity (type 0, 4)<br />
12.bh_mass (type 5)<br />
13. bh_modot (type 5)<br />
14.bh_nprogs (type 5)<br />
<br />
So take bh_mass (as blackhole mass and it wont be discrete as you see in the mass field)
and bh_modot for accretion rate.<br />
<br />
UnitMass_in_g = 1.989e+43            -->10^10 solar mass<br />
UnitLength_in_cm = 3.085678e+21      -->1 kpc<br />
UnitTime_in_s = 3.08568e16           -->this is derived from velocity and length<br />
UnitVelocity_in_cm_per_s = 100000    --> km/sec<br />
<br />
Accretion rate is in mass/time unit in the above units. you will need to multiply by 
c^2 to get the bolometric luminosity.<br />
