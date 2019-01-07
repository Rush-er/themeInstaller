#! /bin/bash

if [ $EUID != 0 ]; then
    sudo "$0" "$@"
    exit $?
fi

ROOT_UID=0
DEST_DIR=

# Destination directory
if [ "$UID" -eq "$ROOT_UID" ]; then
  DEST_DIR="/usr/share/DestinationFolderName"
else
  DEST_DIR="$HOME/.DestinationFolderName"
fi

  rm -rf $DEST_DIR/NAME*
  echo -e "\nInstalling Theme/Icons_Name..."
# Copying files
  cp -a Theme/Icons_Name* $DEST_DIR
  echo -e "\nInstallation complete!"
  notify-send "All done!" "Enjoy Theme/Icons_Name!" -i face-smile

