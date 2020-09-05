# mDNSrestart for Odysseyra1n!


MDNSFlush was [originally created by nathanaccidentally](https://github.com/nathanaccidentally/mDNSFlush) for flushing the ```mDNSResponder``` and ```discoverd``` cache so that you shouldn't run into any issues with network dropping/disconnecting.

I've modified it as a fix [for this LetMeBlock issue](https://github.com/PoomSmart/LetMeBlock/issues/15) on Odysseyra1n.

mDNSrestart should fix issues related to mDNSResponder & mDNSResponderHelper on boot. mDNSrestart uses a LaunchDaemon to run a bash script on boot, and stops running immidiately after the script has finished running. The daemon will only launch once every boot.

You should reboot after install to test whether its working. If the script has run it'll concatonate the current date after boot to /tmp/flush.log

You should be able to compile this quite easily and run it on your device.

**Changelog v1.1:**

1.1 Fixed permissions on files to execute correctly on install and boot

1.0 Initial release
