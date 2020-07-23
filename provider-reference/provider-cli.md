---
description: Golem Provider command line interface
---

# Provider CLI reference

## CLI response

{% hint style="info" %}
Please check for feedback while interacting with all the commands below. For example when user types

```text
golem settings set node_name
```

 CLI should respond either:

1. Node name changed to or
2. Prompt info what went wrong
{% endhint %}

##  CLI commands

* `golem status` Display general status, state, latest jobs and wallet info
* `golem settings` Manage settings
  * _subcommands:_
    * `show` Show current settings
    * `set` Change settings
    * `help` Prints this message or the help of the given subcommand\(s\)
      * `golem settings show` Show current settings
      * `golem settings node name` Set name of your node
      * `golem settings set` Change settings
        * `golem settings set --cores` Set number of shared CPU cores \[≥1\]
        * `golem settings set --memory` Set number of shared RAM \[GB\]
        * `golem settings set --disk` Set number of disk space \[GB\]
        * `golem settings set --starting_fee` \(_default 0_\) Set a price for starting a task
        * `golem settings set --env_per_hour` \(_default X_\) Set a price for working environment per hour
        * `golem settings set --cpu_per_hour` \(_default X_\) Set a price for CPU per hour
      * `golem settigs env` Manage environments
        * `golem settings env show` Show environments
        * `golem settings env enable` Enable environment \(WASM, VM enabled by default\)
        * `golem settings env disable` Disable environment
      * `golem settings cache clear` Clear Provider cache files
      * `golem settings set --payout_address` Set your Ethereum address
* `golem backup` Backup your Golem private keys
  * `golem backup key export` Export your Golem private key
  * `golem backup key import` Import your Golem private key
* `golem stop` Stop Golem
* `golem pause/resume` Pause or resume the node
* `golem help` Prints this message or the help of the given subcommand\(s\)

