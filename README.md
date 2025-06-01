# Cybersecurity game "Red Team"

Linear game for [KYPO CRP](https://docs.crp.kypo.muni.cz/).

Follow the [general instructions](https://gitlab.ics.muni.cz/muni-kypo-trainings/games/all-games-index) to set up the game.

This game uses `kali` and `debian-10` images from [MUNI-KYPO-IMAGES](https://gitlab.ics.muni.cz/muni-kypo-images), which need to be available in OpenStack for use with KYPO CRP. To get and upload the images, see [this guide](https://gitlab.ics.muni.cz/muni-kypo-images/muni-kypo-images-wiki/-/wikis/How-to-get-image-for-OpenStack).

## Game Levels Summary
* Connect to sandbox and access the attacker machine
* Host scan with nmap to find open services
* Attempt FTP login and explore stored files
* Transfer files and extract credentials
* Log in via SSH using discovered credentials
* Change user's password to restrict access

## Topology summary
|Host|Image|Flavor|
|-|-|-|
|attacker|kali|m1.medium|
|server|debian-10|csirtmu.tiny1x2|
|client|debian-10|csirtmu.tiny1x2|
|router|debian-10|csirtmu.tiny1x2|

