# OpenFOAM cases

.

# VIV_cylinder (not ready yet)

Vortex induced vibrations tutorial case; the starting point for the first "discord-project". Dynamic mesh with SDOF & transient BC, setup for OpenFOAM 5.0. The case is based on wingMotion tutorial (transient part) but has some flaws.. check for later updates.

Please visit https://discord.gg/P9p9eHn for more information and progress in this project. You'll find here an open and helpful community & plenty room for your ideas and questions too :)

.

# VIV_cylinder_v2

The same case but different settings, much quicker results. Steady-state simulation (simpleFoam) is done first to skip the long period of vortex formation, followed by field mapping to other case for transient solver (pimpleDyMFoam). This way the show starts quickly (good for testing) but for real results I'd only do the unsteady part with transient BCs (at least some ramp functions - the initial 'kick' from steady solution is a bit unphysical). Turbulent KE and dissipation rate lowered on inlet.

edit: Due to some changes in newer commits of OpenFOAM v6, the case was updated (tested on commit 6-d3fd147e6c65).
