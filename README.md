# Enhanced Easy HMC Command Line Interface (eezh)

Enhanced EZH script is a fork of [EZH](http://ezh.sourceforge.net/) by [Brian Smith](https://sourceforge.net/u/ixbrian/profile/) for the IBM HMC console to provide an alternate, simpler command structure which makes the HMC command line interface easier to use for day to day administration tasks.  The vision for this project is to enhance and bring EZH commands forward and inline with technologies provided in the newer HMC code base.

**Brian, Thank you and anyone who has contributed to EZH!**

Enhanced EZH provides an interactive menu to make it even easier to use ("eezh" command).


## Installation
To install, download the "eezh" script.

Then use scp to copy the script to your home directory on the HMC (i.e. scp eezh hscroot@hmc_hostname:~)

SSH to the HMC and login as your account.   Then type "source eezh".   You will need to run this command each time you login to the HMC for the EZH commands to be available. 


## Change Log
### Version 2.0 (2020-09-29)
- Changed name from ezh to eezh; Enhanced EZH.
- Enhancements:
  - Most commands now sort output by frame name then LPAR name.  Input listings for frame and LPAR names are sorted as well.
  - LPAR power on, shutdown, restart commands to list only running or powered off LPARs depending on selected operations.
  - framelsfirm now displays the Update Access Key (UAK) expiration date for POWER8 or later hardware.
  - lparlscpu no longer returns "null" for dedicated CPU LPARs.
- New commands:
  - sriovlsfirm - list SRIOV firmware, driver and frame update availability.
- Commands in the works:
  - sriovlsadapter
  - sriovlsphysport
  - sriovlslogport


## About the author / Contacting the author
This script is ehanced by Matthew Opoka and originally authored by Brian Smith.

You can contact me at:  m a t t h e w at o p o k a dot n a m e

## License / Disclaimer
**This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.**

**This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.**

**You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.**
