#!/bin/bash
# To run, type 'bash 2.EDITH.sh' OR './2.EDITH.sh'

echo "Hello! My name is EDITH.  "
#  EDITH = Even Dead... I Am The Hero.  :)
sleep 1.5
echo ' '
echo '  ^    ^' 
echo "    ..  "
echo "  \____/ "
echo '   '
sleep 2
echo "This script has 2 parts..."
sleep 1  
echo "Part 1 will stop and restart all  Security Onion (SO) services"
sleep 1
echo "Part 2 will start up additional services (Moloch, MISP, and the Hive)."
sleep 1
read -p "Press [c] to continue, or press anything else to quit: " continue 
if [[ $continue = c ]] ; then

	sleep .5
	read -p "Does SO need to be updated? Please enter [y/n]" answer
		if [[ $answer = y ]] ; then

			echo sudo so-stop
			sudo so-stop
			sleep 3
			echo sudo soup
			sudo soup
			sleep 3
			echo sudo so-start
			sudo sudo so-start

		fi
#############################################################################
# 				just for fun                                #
#############################################################################
#
clear
echo 'now its time for some fun...'
sleep 2
clear
bash /home/jrizzie/fun/chloe.sh
#
#############################################################################
#                               just for fun                                #
#############################################################################
clear
	read -p "Start Moloch/Hive/Misp? Enter [y/n]: " last
	if [[ $last = y ]] ; then
		echo Starting Moloch...
		sleep 1 
		echo sudo systemctl start molochcapture
		sudo systemctl start molochcapture
		sleep 1
		echo .
		sleep .5	
		echo ..
		sleep .5
		echo ...
		sleep 3
		echo sudo systemctl start molochviewer
		sudo systemctl start molochviewer
		sleep 1
		echo .
		sleep .5
		echo ..
		sleep .5
		echo ...
		sleep 3
		clear
		echo 'starting The Hive - (in Docker)...'
		cd /docker/thehive && docker-compose up -d
		cd ~
		echo .
		sleep 1
		echo ..
		sleep 1
		echo ...
		fi
fi
