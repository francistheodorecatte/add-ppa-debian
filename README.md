# add-ppa-debian for Debian 11+
For when you want newer mesa-vulkan-drivers builds than Debian packages!

Now including support for per-repository keyrings, bypassing the deprecated /etc/apt/trusted.gpg. Note that makes this script useless for Debian versions 10 or older, but older versions of this script using the ``apt-key add`` method will still work.

**Install**  
Make the script executable and copy it to a PATH binary directory like /usr/local/bin.

**Usage**  
Run with root privileges or sudo, passing the PPA as the only argument, e.g.:  
``sudo add-ppa-debian ppa:kisak/kisak-mesa``

**Updating expired keys**  
Simply rerun add-ppa-debian passing the affected PPA.

**PPA Removal**  
Delete the PPA sources file from ``/etc/apt/sources.list.d/``, optionally removing the PPA key file from ``/usr/share/keyrings/``.
