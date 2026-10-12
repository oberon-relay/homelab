# Cisco 2821 Password Recovery / Wipe

## Steps

1. Power-cycle the router. As soon as System Bootstrap starts, send the control break of `Ctrl-A` & `\`.
2. `confreg 0x2142` to indicate a skip of the normal processes.
3. `reset` to complete the router.
4. Answer `no` to the setup dialogue, then `enable` to move to admin mode (`#`).
5. `configure terminal`, then `config-register 0x2102`, and then `end` to write in the new normal.
6. `write erase` to delete the old configuration in the NVRAM.
7. `reload` to get the router to re-read the register.
8. Check `show version` to ensure that all is properly completed.

## Register values

* `0x2102` = Normal value.
* `0x2142` = Skipping the router's existing "notebook" of information.

## Traps

* Trap 1: Errors with interrupting the boot.
* Trap 2: Accidentally forgetting to set the changes to ensure they stick for future reboots.
