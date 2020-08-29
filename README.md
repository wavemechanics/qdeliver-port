# qdeliver-port

This repo integrates [qdeliver](https://github.com/wavemechanics/qdeliver) into the FreeBSD ports system.

The contents of this repo should be visible under `/usr/local/ports/mail/qdeliver`.

Most of the time the ports tree is owned by root, so you may not be able to directly clone this repo into the ports directory.

But some ideas:
* `git clone` as root, or
* create a symlink from the ports tree into a cloned directory in your home, or
* rsync from your home to a poudriere instance somewhere else

I use the third method and it works ok.

Once the `mail/qdeliver` directory is populated, you can treat it as a normal port:

```
# cd /usr/ports/mail/qdeliver
# make install
```