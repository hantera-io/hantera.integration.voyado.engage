# Hantera Voyado Engage Integration

This repository contains a basic integration for syncing orders and invoices to [Voyado Engage](https://voyado.com/products/customer-loyalty-platform/) to enable automations and targeting.

The code provides a starting point that can be further enhanced with additional fields as needed for each project.

## Overview

The files in the repository is explained below:

- `/h_manifest.yaml`

  This manifest installs the integration.
  
- `/components/voyado.engage.onOrderCommands.hreactor`

  This rule component captures events in Hantera and schedules the appropriate jobs.

- `/components/voyado.engage.orders.hreactor`

  The reactor component is responsible for export orders used for automations. Refer to source code comments for more information.

- `/components/voyado.engage.receipts.hreactor`

  The reactor component is responsible for exporting invoices for commerce-based targeting

## Getting started

The code contains mapping for standard features and should work out-of-the-box. To quickly get started, simply apply the `h_manifest.yaml` file to your installation using [Hantera CLI](https://developer.hantera.io/learn/hantera-cli/):

```bash
h_ manage apply h_manifest.yaml
```

## Support

This integration is provided as-is, but if you have any question, you are welcome to join us on [Discord](https://discord.gg/pKUjk952U6).