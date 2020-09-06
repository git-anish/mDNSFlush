# mDNSrestart for Odysseyra1n!

mDNSrestart relaunches mDNSResponder and mDNSResponderHelper on boot. It does this through a LaunchDaemon thats set to run a script on boot (only in the jailbroken environment). The LaunchDaemon will run once per boot and never again. You can look at the log in /tmp/mDNSrestart.log to see when it was last run.

mDNSrestart was made possible by [nathanaccidentally's mDNSFlush](https://github.com/nathanaccidentally/mDNSFlush)

mDNSrestart should fix issues [15](https://github.com/PoomSmart/LetMeBlock/issues/15) & [17](https://github.com/PoomSmart/LetMeBlock/issues/17) on Odysseyra1n.

You should reboot after install to test whether its working. If the script has run, it will concatonate the current date & time after boot to /tmp/mDNSrestart.log

You should be able to compile this quite easily and run it on your device.

**Changelog v1.2:**

1.3 Fixed depictions and added dependencies

1.2 Fixed postinst

1.1 Fixed permissions on files to execute correctly on install and boot

1.0 Initial release
