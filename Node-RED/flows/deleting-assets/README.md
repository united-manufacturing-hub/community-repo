# deleteAsset

This flow allows you to delete assets from your database tables using Node-RED. With a little bit of adjustment, you can remove any item that you do not want to keep in your database. This flow is a community contribution from DanielH.

## Prerequisites

Before using this template, make sure that you have installed the `digitaloak/node-red-contrib-digitaloak-postgresql` package. If you need help installing new nodes/plugins in Node-RED, you can follow [this tutorial](https://learn.umh.app/course/how-to-install-new-nodes-plugins-in-node-red/).

## Usage
1. Install the `digitaloak/node-red-contrib-digitaloak-postgresql` package if not already installed.
2. Import the `deleteAsset` flow into your Node-RED instance.
3. Adjust the postgresql query node to connect to your database by entering the database credentials and details.
4. Change the value in the second node to represent the asset you want to delete. You can also customize the SQL query in the postgresql node to suit your requirements.
5. Deploy the flow to your Node-RED instance.
6. Press the inject button to delete the asset.

![deleteAssetFlow](./Untitled%203.png)

You can copy the template from [here](./deleting-asset-node-red.json).
