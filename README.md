# DoS
<b>DoS</b>--A Simple Program to Test DoS Protection System</br>
<b>THIS PROGRAM IS FOR EDUCATIONAL PURPOSES ONLY</b><br>

## Usage
```$./ddos (HOST) (PORT) [options...] ``` <br>
HOST -- host to ddos<br>
PORT -- port to connect,if set to 0 will try random ports<br>
<b>Options:</b><br>
<p>
-r -- generate random packet<br>
-u -- Use UDP<br>
-p -- Use TCP<br>
-t (THREAD COUNT) -- describes thread count,by default set to 5<br>
-s (PACKET SIZE) -- set packet size<br>
--http -- Make http request<br>
--no-warnings -- ignore all warnings<br>
--no-errors -- ignore errors<br>
--no-wait -- Do not wait server to respond<br>
--no-check -- Do not check server before starting ddos<br>
--packetfile (FILENAME) -- load packet conents from file(Could be overrided with --http option)<br>
--sleep (TIME) -- sleep between packets sendings (in milliseconds)<br>
</p><br>
## Examples
``` $ ./ddos some.boring.long.domain.net 80 -t 70 --no-wait --http ```
  <br>
  This will send packets  some.boring.long.domain.net:80 without waiting for response using http request syntax in 70 threads.<br>
``` $ ./ddos example.com 88 --no-check --no-wait -u ```
  <br>
  With this options program will send  packets to example.com:88 without pre-start host check and without waiting for response.Program will use 5 threads. Program will use UDP protocol.<br>

## Updating
``` $ ./build.sh update ```
