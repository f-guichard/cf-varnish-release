# cf-varnish-release
Initial varnish release with broker for CFY marketplace

##Steps details :
A. bosh init release o-varnish
B. bosh generate package varnish
C. Make the release (get tarball, get minimal config file and make all necessary bosh config files -- see bosh.io)
D. bosh create release --force --name varnish --version 1 --with-tarball
E. bosh upload release /dev_releases/varnish
F. bosh releases :
+---------+----------+-------------+
| Name    | Versions | Commit Hash |
+---------+----------+-------------+
| varnish | 1*       | 00000000    |
+---------+----------+-------------+
(*) Currently deployed

#Next step : 
A. make this release a real tutorial for community
B. push broker source code
C. Explain register into marketplace
