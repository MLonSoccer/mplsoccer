# mplsoccer
mplsoccer is a Python plotting library for drawing soccer / football pitches quickly in Matplotlib.

mplsoccer currently supports several data formats:
- Statsbomb
- Stats Perform
- Tracab (ChyronHego) tracking data
- Opta
- STATS (formerly Prozone)
- Wyscout (the pitch dimensions are taken from ggsoccer: https://github.com/Torvaney/ggsoccer)

The following example draws a Statsbomb pitch (the default) with stripes.
``` python
from mplsoccer.pitch import Pitch
pitch = Pitch(orientation='horizontal',figsize=(10,10),stripe=True)
fig, ax = pitch.draw()
fig.savefig('statsbomb.png',pad_inches=0,bbox_inches='tight')
```
![alt text](https://github.com/andrewRowlinson/mplsoccer/blob/master/docs/figures/README_example_statsbomb_pitch.png?raw=true "statsbomb pitch")

For fun you can also plot the same pitch in xkcd mode.
``` python
from mplsoccer.pitch import Pitch
import matplotlib.pyplot as plt
plt.xkcd()
pitch = Pitch(orientation='horizontal',figsize=(10,10),stripe=True)
fig, ax = pitch.draw()
fig.savefig('statsbomb_xkcd.png',pad_inches=0,bbox_inches='tight')
```
![alt text](https://github.com/andrewRowlinson/mplsoccer/blob/master/docs/figures/README_example_xkcd_pitch.png?raw=true "pitch xkcd style")

# This library is under development
The following developments are planned
- create pass map methods
- add examples (team line-up / pass maps/ pressure maps/ subplots)
- add method for plotting Voronoi diagrams
- create documentation using Sphinx
