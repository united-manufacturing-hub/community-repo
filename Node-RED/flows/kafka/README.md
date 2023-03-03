# Exporting Kafka data with a Node-RED flow

This Node-RED flow exports Kafka data by importing Kafka messages, converting them to Base64, and exporting them. This tutorial demonstrates how to use the flow with simulated temperature data. 
![Untitled](/images/knowledge-base/node-red-flows-repo/Untitled%202.png)

## Prerequisites

Before using this flow, make sure that you have installed the `node-red-contrib-kafkajs` and `node-red-contrib-base64` packages.

## Usage

1. Copy the template `kafkaexportTemplate-node-red.json` to your clipboard.

2. Open your Node-RED instance and import the template by selecting `Import` from the main menu, then `Clipboard` and paste the contents of the clipboard. 

3. Double-click on the `Kafka Message Consumer` node and configure it to consume the appropriate Kafka messages.

4. Deploy the flow to your Node-RED instance.

5. The flow will import Kafka messages and convert them to Base64. The `Base64 Encoder` node will encode the message in Base64 format, and the `File` node will write the message to the specified file path.

## Note

If you encounter any issues exporting binary data, this flow may be a more reliable solution than using Kowl.

