# GDash

A unified GPU statistics dashboard for multiple servers.

## Usage

Given SSH hosts `g1`, `g2` and `g3`
already defined in `~/.ssh/config`,
execute locally:
```bash
./gdash g1 g2 g3
```
Example result:
```
Server    GPU    Usage    Memory             Users
--------  -----  -------  -----------------  --------------------------
g1.0      v100   15%      19.24GB / 31.75GB  lxx(19.23GB), root(4.00MB)
g1.1      v100   0%       19.24GB / 31.75GB  lxx(19.23GB), root(4.00MB)
g1.2      v100   0%       19.24GB / 31.75GB  lxx(19.23GB), root(4.00MB)
g1.3      v100   17%      19.24GB / 31.75GB  lxx(19.23GB), root(4.00MB)
g2.0      v100   16%      19.37GB / 31.75GB  lxx(19.36GB)
g2.1      v100   16%      19.37GB / 31.75GB  lxx(19.36GB)
g2.2      v100   15%      19.37GB / 31.75GB  lxx(19.36GB)
g2.3      v100   83%      24.21GB / 31.75GB  lxx(19.36GB), root(4.84GB)
g3.0      v100   91%      29.90GB / 31.75GB  wxx(29.89GB)
g3.1      v100   0%        4.00MB / 31.75GB
g3.2      v100   0%        4.00MB / 31.75GB
g3.3      v100   0%        4.00MB / 31.75GB
```
