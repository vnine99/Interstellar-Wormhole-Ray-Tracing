# Interstellar-Wormhole-Ray-Tracing
As part of a computational methods in physics class, my two team members and I created this Mathematica notebook which implements a ray tracing map for the light from a wormhole. Our approach was based on the paper by Kip Thorne et al. (http://arxiv.org/abs/1502.03809)

We have implemented parallelized and nonparallelized versions of the raytracing computation. The parallelized version leverages Mathematica's ParallelTable. 

To run the notebook, place files named "GargantuaSide.jpg" and "SaturnSide.jpg" in the same directory as the notebook file. These images will represent the two sides of the wormhole. To increase the accuracy of the algorithm at the cost of increased computation time, make the division size smaller in the ray-trace computation. For example, change the two instances of 512 in CreateMap to 1024. One can adjust the location of the camera by adjusting theta_c, phi_c, and l_c. One can also adjust the wormhole's lensing width, mass, diameter, and length. These parameters are more fully described in the aforementioned paper. 

One can use the images provided by Double Negative VFX (http://www.dneg.com/dneg_vfx/wormhole/) to render images which resemble the wormhole from Interstellar.

We used the following star field image and Saturn image:

![](https://github.com/lrudolph1/Interstellar-Wormhole-Ray-Tracing/blob/master/Images/InterstellarWormhole_Fig10.jpg)


![](https://github.com/lrudolph1/Interstellar-Wormhole-Ray-Tracing/blob/master/Images/InterstellarWormhole_Fig6a.jpg)

With these images and our ray tracing implementation (with 1024 divisions), we obtained the following image:

![](https://github.com/lrudolph1/Interstellar-Wormhole-Ray-Tracing/blob/master/Images/1024%20division%20render.jpg)

This rendering simulates the perspective of a camera at the star field location looking into a wormhole which leads to Saturn.

