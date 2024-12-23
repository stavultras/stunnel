# Additional changes to the original stunnel
Added "direct" protocol. It's very similar to socks5, but doesn't have excess socks5's handshakes which decreases latency. "direct" protocol doesn't use "auth" handshake. In my case I was able to reduce latency from 450 ms to 250 ms. However, if you still need socks5 client on stunnel client's side, you can use "direct:socks5" protocol.


# stunnel overview


### Short description

The stunnel program is designed to work as an SSL encryption
wrapper between remote client and local (inetd-startable) or
remote servers. The goal is to facilitate SSL encryption and
authentication for non-SSL-aware programs.

stunnel can be used to add  SSL  functionality  to  commonly
used  inetd  daemons  like  POP-2,  POP-3  and  IMAP servers
without any changes in the programs' code.

### License

* [COPYING](COPYING.md) A short license overview
* [COPYRIGHT](COPYRIGHT.md) The complete terms and conditions
* [CREDITS](CREDITS.md) A list of major contributions

### Other useful files

* [NEWS](NEWS.md) What I did
* [TODO](TODO.md) What I'm going to do
* [BUGS](BUGS.md) Known bugs
* [INSTALL.FIPS](INSTALL.FIPS.md), [INSTALL.W32](INSTALL.W32.md) and
  [INSTALL.WCE](INSTALL.WCE.md) Additional installation notes
* [PORTS](PORTS.md) Known ports

### Reporting problems and other contacts

* [Support](https://www.stunnel.org/support.html) options
* [Contacts](https://www.stunnel.org/contact.html)
