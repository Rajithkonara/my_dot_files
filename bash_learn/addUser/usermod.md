# can edit 

## expiary date to a account

$ usermod --expiredate 2017-10-30 rajith

## adding the user to supplementary group

$ usermod --append --groups root,users rajith

## changing default location of the home directory

$ usermod --home /tmp rajith

## changing the shell the user will by default

$ usermod --shell /bin/sh rajith
