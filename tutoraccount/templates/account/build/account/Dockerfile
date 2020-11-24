FROM debian

LABEL MAINTAINER=MP
RUN apt-get update && apt-get -y upgrade

# Installing python packages with nano, vim and telnet
RUN apt-get -y install python3-dev default-libmysqlclient-dev build-essential nano vim telnet

RUN apt-get -y install python3-pip  git curl 
RUN pip3 install mysqlclient

# Installing node and React dependencies
RUN apt-get -y install node-gyp nodejs npm && npm install npm@latest -g

# Making directory
RUN  mkdir /openedx /openedx/data

# Cloning  your custom app to the working directory ##
RUN git clone -b murat https://github.com/murat-polat/frontend-app-account/ /openedx/account

WORKDIR /openedx/account/

RUN cd /openedx/account

## Installing and building app
RUN npm install 

EXPOSE 1997 


CMD ["npm", "start" ]