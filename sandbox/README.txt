WEB TESTING SANDBOX – README
-----------------------------------------

This project is a complete Web Testing Sandbox built using Docker.
It provides a safe, isolated environment for testing websites, monitoring traffic, and running a browser without affecting the host machine.

-----------------------------------------
PROJECT FEATURES
-----------------------------------------

1. Browser Container (Chrome UI)
   - A full Chrome browser runs inside a Docker container.
   - Access it at: https://localhost:3001

2. Logged Network Traffic
   - All browser traffic is captured using tcpdump.
   - Logs are saved into logs/traffic.pcap

3. Private, Isolated Network
   - Containers run in a dedicated isolated network called "websandbox".

4. Controlled DNS
   - Browser container DNS is forced to 1.1.1.1

5. Full Auto Reset on Close
   - Run docker compose down -v to fully reset.

-----------------------------------------
HOW TO RUN THE SANDBOX
-----------------------------------------

1. Open terminal inside the sandbox folder.
2. Run: docker compose up
3. Open: https://localhost:3001
4. Click Advanced → Proceed to localhost (unsafe)

-----------------------------------------
USING THE SANDBOX
-----------------------------------------

- Launch Chrome inside the Selkies desktop UI.
- Browse any site.
- Traffic logs saved to logs/traffic.pcap

-----------------------------------------
RESETTING
-----------------------------------------

CTRL + C to stop
docker compose down -v

-----------------------------------------
