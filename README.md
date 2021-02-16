# mac80211_hwsim

This is a modified version of mac80211_hwsim to work with
[YAWMD](https://github.com/mjmoreira/yawmd).

Mac80211_hwsim normally comes with the Linux kernel.
The original is available in the
[Linux kernel source](https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/tree/)
at `drivers/net/wireless/mac80211_hwsim.h` and
`drivers/net/wireless/mac80211_hwsim.c`.

# Building
You need the Linux kernel headers (from a package named linux-headers or similar),
to build mac80211_hwsim.

```
make
```

# Running
```
sudo modprobe mac80211
sudo insmod mac80211_hwsim.ko [radios=10] # default is 2
```

