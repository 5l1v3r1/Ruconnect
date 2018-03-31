# ruconnect.rb
A handy tool made to control multiple devices one at the time using the terminal. The tool is using tcp socket and letting each device act like a client by letting them connect to you and wait for your command, you only have to type the command once and the script itself will send it to every device and you will then after get their response.

## Usage

Start client: `ruby client.rb`

Start host: `ruby host.rb`

**NOTE**: You need to start the host before you can start clients.

## Usage (daemon)

![Starting client as background worker](start-client.gif)

Start client as background worker: `ruby daemon.rb start`

![Stopping client background worker](stop-client.gif)

Stop client background worker: `ruby daemon.rb stop`

Start host: `ruby host.rb`

**NOTE**: Client(s) will continue searching for a host until one is found.