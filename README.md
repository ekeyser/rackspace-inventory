rackspace-inventory
========

#### Rackspace Infrastructure Inventory ####

This module provides an abstraction layer to inventory your cloud resources.

Supported services (and APIs):

Supported Regions

### Installation ###
```bash
npm install rackspace-inventory
```

### Usage ###

```javascript
import RackspaceInventory from 'rackspace-inventory'

const config = {
  credentials: {
    accessKeyId: 'your_access_key',
    secretAccessKey: 'your_secret_key'
  },
  services: ['ec2', 'rds'],
  regions: ['us-west-2, us-east-1']
};

const oInventory = new RackspaceInventory(config);
const oResources = oInventory.inventory();
```
