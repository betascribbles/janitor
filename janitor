#!/bin/env bash

echo -e "\e[1;32m Step 1: Updating|Upgrading packages\n=====================================\e[0m"
sudo apt-get update -y && sudo apt-get upgrade -y

echo

echo -e "\e[1;32m Step 3: Repair broken packages/dependencies\n=============================================\e[0m"
sudo apt --fix-missing update -y
sudo apt-get update -y
sudo apt-get install -f -y

echo

echo -e "\e[1;32m Step 4: Removing all the junk files\n=====================================\e[0m"
sudo apt-get clean -y
sudo apt-get autoclean -y
sudo apt-get autoremove -y

echo

echo -e "\e[1;32m Last step: Updating packages\n==============================\e[0m"
sudo apt-get update -y && sudo apt-get upgrade -y

echo

echo -e "\e[1;32m \tCONGRATULATIONS $USER!!\n \tYour system is clean and up-to-date\e[0m"

echo
