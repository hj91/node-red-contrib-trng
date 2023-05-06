# node-red-contrib-trng

A Node-RED module that attempts to be a True Random Number Generator (TRNG) for generating highly random data when triggered.

## Features

- Generates random data by combining multiple sources of entropy
- Output is provided as a hexadecimal string
- Configurable output length

## Installation

### Using the Node-RED editor:

1. Click the hamburger menu in the top right corner.
2. Select "Manage Palette".
3. In the "User Settings" window, switch to the "Install" tab.
4. Search for `node-red-contrib-trng` and click "Install".

### Using npm:

Run the following command in your Node-RED user directory (typically `~/.node-red`):

```bash
npm install node-red-contrib-trng
```

## Usage

1. Drag the "TRNG" node from the palette into the workspace.
2. Double-click the node to configure its properties, such as output length.
3. Wire the "TRNG" node to other nodes as needed (e.g., a debug node to display the output).
4. Deploy the flow and trigger the "TRNG" node to generate random data.


## Example

Here's a simple example of how to use the TRNG node in a flow:

1. Add an inject node and set its payload to a number, representing the desired length of the random data.
2. Connect the inject node to the input of the TRNG node.
3. Add a debug node and connect it to the output of the TRNG node.
4. Deploy the flow and trigger the inject node. The debug node should display the generated random data as a hexadecimal string of the specified length.
5. Check examples/ for the readymade sample flow.

## Author

Harshad Joshi

## License

This Node-RED module is released under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
```

## Use Cases

The TRNG (True Random Number Generator) Node-RED module can prove useful in various scenarios where you need high-quality random data. Some potential use cases include:

1. Cryptography: Generating encryption keys, initialization vectors, or salts to ensure strong security in encryption and cryptographic operations.
2. Unique Identifiers: Creating unique IDs for resources, transactions, or other entities that require a high degree of uniqueness and unpredictability.
3. Random Sampling: Selecting random samples from large datasets for statistical analysis, simulations, or testing purposes.
4. Randomization in Testing: Generating random inputs for testing and validation of software or hardware systems, ensuring a wide range of test cases.
5. Gaming and Gambling: Producing random outcomes for games, lotteries, or gambling applications to ensure fairness and unpredictability.
6. Authentication: Generating one-time passwords (OTP) or temporary tokens for secure authentication processes.
7. Simulation and Modeling: Generating random initial conditions, parameters, or events in simulations and modeling systems to study various scenarios or to perform Monte Carlo simulations.
8. Load balancing and Distribution: Randomly distributing tasks, requests, or resources across multiple servers, processes, or workers to balance the load and optimize system performance.

The TRNG Node-RED module is designed to generate high-quality random data by combining multiple sources of entropy, making it suitable for applications where the quality of randomness is crucial.


## Disclaimer 

This module is created for generation of random numbers and does not intend to replace existing security solutions and algorithms. Do not complain to me or anyone in case things break by using this module. 
