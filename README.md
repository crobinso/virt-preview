Helper script for maintaining the [fedora virt preview repo](http://fedoraproject.org/wiki/Virtualization_Preview_Repository), a [Fedora copr repo](https://copr.fedorainfracloud.org/coprs/g/virtmaint-sig/virt-preview/) hosting builds of latest virt packages for stable Fedora releases.

When invoked, the script will:

* Check koji for latest virt package version strings
* Find which versions aren't in the copr repo yet
* Kick off copr commands to build them

I run it daily in a cron script.
