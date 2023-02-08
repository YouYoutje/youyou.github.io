---
sidebar_position: 1
---

# Common Issues

## UI has not been built

Because the UI for inventory is written in React it can't run natively under FiveM so it must first be bundled into html/css/js.

We provide an easy way for you to do this by downloading a pre-bundled release, which you can get from [here](https://github.com/overextended/ox_inventory/releases/latest).  
Make sure you download the `ox_inventory.zip` file as that one contains the bundled files and others are raw source code.

If in case you wanted to edit the inventory UI you would have to build these files yourself.  
To do so please read our [_Building inventory UI_](../Guides/inventory_ui.md) guide.

## Stashes / trunks are not saved at server restart

The only supported way of doing a restart is **txAdmin scheduled restart**.  
txAdmin scheduled restart should be your only way of restarting a server in production.

If you need to do a manual restart, you must use `/saveinv` before restarting the server.  
If you don't do this, all inventory except players inventory will not be saved.
