**How to update your loop**

*******************
1. Delete your exsiting cron (this helps prevent those annoying rebooting to fix radio error messages after a rebuild)

`cd`

`crontab -r`

`rm -rf myopenaps`

`rm -rf src`

********************
2.  Then let's grab updated oref0 code

  `mkdir -p ~/src; cd ~/src && git clone -b myversion git://github.com/hilarykoch/oref0.git || (cd oref0 && git checkout myversion && git pull)`
  
  `npm run global-install`

********************
3.  Edit your runagain file to change anything that you'd like by using either of these commands

`cd && ~/src/oref0/bin/oref0-setup.sh`

********************
5. Once everything gets installed and you answer YES to both of the cron questions, then we will edit your preferences.json

`edit-pref`

********************
Congrats, your loop is updated and your runagain has saved the information for all those.
