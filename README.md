# NH Applet Scaffolding Template
This repository contains a webhapp template for the [holochain scaffolding tool](https://github.com/holochain/scaffolding).

## Getting Started
This guide assumes you have the [holochain nix environment](https://developer.holochain.org/quick-start/) set up.

Then, start by running:
```bash
nix run github:holochain/holochain#hc-scaffold -- web-app --templates-url https://github.com/neighbour-hoods/nh-applet-template
```

Follow the steps provided in the terminal. Once your applet repository has been created, you can continue to use the scaffolding tool to create a working applet.

Scaffold your DNA:
```bash
hc scaffold dna {dna_name}
```

Scaffold your zome:
```bash
hc scaffold zome {zome_name}
```

Scaffold your entry type:
```bash
hc scaffold entry-type {entry_type_name}
```

Build your applet:
```bash
npm run package:applet
```

Which will bundle a `.webhapp` file that can be loaded into the [NH-launcher](https://github.com/neighbour-hoods/nh-launcher).