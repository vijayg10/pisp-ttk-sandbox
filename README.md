# PISP TTK Sandbox

## Introduction
![Diagram](/assets/images/diagram-pisp-sandbox-ttk.jpg)

## Quick Start
1. Clone the repository
```
git clone https://github.com/vijayg10/pisp-ttk-sandbox.git
cd pisp-ttk-sandbox
```
2. Run simulators
```
docker-compose up
```
3. Open TTK Sender UI on http://localhost:16060
4. Goto `Test Runner` and open `Collection Managaer`
5. Click on `Import File` and load the TTK test case `thirdparty.json` from the folder `test-cases`
6. Select the imported file in the collection manager
7. Click on the button `Run`
8. Observe the requests and responses in each test case


## Sending Third-party http requests from your solution
1. Run the docker-compose as per the previous section.
2. Send the http requests from your implementation to `localhost:4040`.
3. Observe the inbound requests and simulated responses in TTK receiver monitoring page http://localhost:6060/monitoring
