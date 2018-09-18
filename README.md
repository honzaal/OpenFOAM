# OpenFOAM cases

.

# VIV_cylinder (not ready yet)

Vortex induced vibrations tutorial case, the starting point for the first "discord-project". Dynamic mesh with SDOF & transient BC, setup suitable for OpenFOAM 5.0. The case is based on wingMotion tutorial (transient part) but still has some flaws.. check for later updates.

Please visit https://discord.gg/P9p9eHn for more information and progress in this project. You'll find here an open and helpful community & plenty room for your ideas and questions too :)

.

# VIV_cylinder_v2

The same case with different settings, much quicker run. Steady-state simulation (simpleFoam) is done to skip the long period of vortex formation, followed by field mapping to other case for transient solver (pimpleDyMFoam). This way the show starts quickly (good for testing) but for real results I'd do only the unsteady part with transient BC. Turbulent KE and dissipation rate were lowered on inlet.
