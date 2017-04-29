## Lost atom
---
    Lost atoms: original %ld current %ld

每次输出therom会检查lost atom，表示原子离开box太远，或者在reneiboring之前，移动距离超过一个处理器的子区域。

Lost atoms are checked for each time thermo output is done. See the thermo_modify lost command for options. Lost atoms usually indicate bad dynamics, e.g. atoms have been blown far out of the simulation box, or moved further than one processor’s sub-domain away before reneighboring.

\[dd\]
