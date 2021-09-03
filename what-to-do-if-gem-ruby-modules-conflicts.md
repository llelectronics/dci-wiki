# Fix Ruby Gem plugin conflict

* move ~/.gem on the jenkins user out of the way 
* machinectl shell jenkins@ -> cd ~/jobs/mgmt_tooling/workspace -> bundle update
