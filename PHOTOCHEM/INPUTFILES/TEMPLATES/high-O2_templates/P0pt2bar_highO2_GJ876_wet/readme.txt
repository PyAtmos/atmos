Running the photochemical model for a high-O2 (95% O2) Earth with GJ 876 as the host star.

The surface pressure is P0=0.2 bars. Assumptions is the steady-state atmosphere described in Wordsworth & Pierrehumbert 2014,
where a low abundances of a non-condensible gas has removed the cold trap and allowed O2 to build up (after H2O photolysis and escape of H)
until the cold trap is restablished. Meanwhile the planet's surface is irrevesibly oxidized over time. No reduced gases should be present. 

Updated "species.dat" for oxidized mantle case:

H2 --> LBound 1--> 0 (Vdep = 2.4E-02)
CO --> Lbound 1--> 0 (Vdep = 1.2E-02)
CH4 --> Lbound still 1; mixing ratio fixed at 0.0 (Vdep changed to 1.e00)
N2O --> Mixing ratio goes from 3.7e-07 --> 0.0
N2 --> Rmix 0.78 --> 0.02

Other reduced species have a large deposition velocity because they would be consumed by an oxidized surface. 
Oxidized species have a 0 deposition velocity. 

in.dist close to convergence.

-EWS - updated 09/18/2015 (eschwiet@uw.edu)

03/04/2016: Updated in.dist to correct for earlier code error - EWS (eschwiet@uw.edu)
NOTE: The o2 mixing ratio had to be changed to 92% in species.dat to allow model convergence at P0=0.2bar.
03/14/2016: Updated species.dat, parameters.inc, and in.dist to correct for NR (no significant effect),
            and redox calc error from Tri-diag species. 
