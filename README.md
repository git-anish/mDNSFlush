# mDNSrestart for Odysseyra1n!

You can install this from [my repo](https://repo.anishs.xyz/), it is also available on [Packix](https://repo.packix.com/package/com.git-anish.mDNSrestart/)!

mDNSrestart relaunches mDNSResponder and mDNSResponderHelper after a successful boot. It does this through a LaunchDaemon thats set to run a script on boot (only within a jailbroken environment). The LaunchDaemon will run once per boot and never again. You can look at the log in /tmp/mDNSrestart.log to see when it was last run.

mDNSrestart was made possible by [nathanaccidentally's mDNSFlush](https://github.com/nathanaccidentally/mDNSFlush).

mDNSrestart should fix issues related to LetMeBlock & other ad-block related tweaks [15](https://github.com/PoomSmart/LetMeBlock/issues/15) & [17](https://github.com/PoomSmart/LetMeBlock/issues/17) on Odysseyra1n.

You should reboot after install to test whether its working. If the script has run, it will concatenate the current date & time after boot to /tmp/mDNSrestart.log

You should be able to compile this quite easily and run it on your device.

**Changelog:**

1.4 Fixed Packages file and changed repo domain

1.3 Fixed depictions and added dependencies

1.2 Fixed postinst

1.1 Fixed permissions on files to execute correctly on install and boot

1.0 Initial release
