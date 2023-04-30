Setup
=====

General
-------

Pull the latest version of the project Install node.js v18

Install pnpm with (npm install -g pnpm)

To Run Frontend:
----------------

In frontend_react
~~~~~~~~~~~~~~~~~

run: pnpm i

In /src/contracts_hardhat
~~~~~~~~~~~~~~~~~~~~~~~~~

run:

pnpm add -D hardhat

pnpm hardhat compile

.. _in-frontend_react-1:

In frontend_react
~~~~~~~~~~~~~~~~~

run: pnpm start

To Run Backend:
---------------

In backend_dotnet
~~~~~~~~~~~~~~~~~

run: dotnet run

To set up metamask
------------------

Create a wallet Go to settings -> networks -> Add a network

Network Name: Avalanche FUJI C-Chain (You can edit this if you want) New
RPC URL:
https://nd-363-962-610.p2pify.com/e561a44aeaec63c0ab48af257d3352fe/ext/bc/C/rpc
Chain Id : 43113 Currency symbol : AVAX Block explorer URL :
https://testnet.snowtrace.io/

Press save and use this network while entering the website

Docker Setup
------------

Docker Commands
~~~~~~~~~~~~~~~

run:

docker compose build

docker compose -f docker-compose.yml up -d

Important:

-d flag is not required if the containers will run on a screen

REACT_APP_BACKEND_URL and REACT_APP_FRONTEND_URL need to be set
accordingly inside the docker-compose.yml file

Shutting down the containers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

run: docker compose down

if it does not work,

run:

docker stop $(docker ps -aq)

docker rm $(docker ps -aq)

For Linux Enviroments
~~~~~~~~~~~~~~~~~~~~~

podman-compose can be used instead of docker compose and podman instead
of docker if root access is not available

To keep the containers running in the background when the terminal is
closed, create a new screen and run the commands inside of it

Screen controls
~~~~~~~~~~~~~~~

To create a new screen
~~~~~~~~~~~~~~~~~~~~~~

run: screen -S

Deattach the current screen
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Press CTRL+A and then D

Reattach a screen
~~~~~~~~~~~~~~~~~

run: screen -x

To terminate the current screen
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Press CTRL+A and then Y and then Enter

