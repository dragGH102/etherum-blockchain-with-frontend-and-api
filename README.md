App developed for Hackzurich 2017 composed of:
- Backend (Node + python for data fetching from Tomson Reuters API)
- Frontend (jQuery + D3JS)
- Private blockchain with Etherum smart concract ("Charitycoin")

The idea was to offer a blockchain solution to the lack of transparency in online donations.

Developer with the awesome help of my team mates (Klemen, Viton and Nina)

# RUN private Blockchain

## Install etherum 

https://ethereum.gitbooks.io/frontier-guide/content/installing_linux.html

## Run etherum

./Blockchain/start.sh

# RUN frontend (Linux)

npm install -g serve

serve Frontend/

# RUN DB in Docker
 
docker run \
  --detach \
  --publish 27017:27017 \
  --restart unless-stopped \
  --name MongoDB \
  --volume /home/manuel/TMP/MIX_CAN_DELETE/hackzurich2017:/data/db \
  mongo:3.4
