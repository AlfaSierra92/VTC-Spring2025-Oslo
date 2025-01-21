# VTC-Spring2025-Oslo

Official repository of all of the codes mentioned into VTC-Spring2025-Oslo paper.

## iPerf w/ AC
An iPerf patch (*001-iperf-MAC_AC-patch.patch*) to enable Access Categories (BK, BE, VI, VO).

## Raspberry Pi 5 tweaking
### ath9k debug mode

Edit kernel config file by adding:

```bash
CONFIG_ATH9K_HTC_DEBUGFS=y
CONFIG_ATH9K_HWRNG=y
CONFIG_ATH9K_DEBUGFS=y
```

and build it as usual.

### Enable queues

Apply *00550-ac.patch* and build Kernel as usual.