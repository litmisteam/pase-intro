PASE is sometimes referred to as "the other side" of IBM i. It can
seem like a vague cloud of discomfort whenever we have to venture into
it. The only way to alleviate discomfort is to take some medicine, and
the prescription we have to offer you is knowledge.

By the end of this tutorial we hope you've gained a lot more knowledge
about PASE and how it works - but even more so, how it can help your
business succeed.

---

The [IBM i Knowledge
Center](http://www.ibm.com/support/knowledgecenter/) has this to say
about [PASE](http://krengel.tech/ibmkn2ecba): 

>PASE for i enables you to run many of your AIX® applications on the IBM® i operating system with little or no change, and effectively expands your platform solution
portfolio.

They *should* end that sentence with an exclamation point to convey the
incredible amount of possibilities this opens for IBM i. Some things
that can be attributed to PASE (listed in alphabetical order):

-   [Apache](http://httpd.apache.org/)

-   [Git](https://git-scm.com)

-   [Java](https://java.com/en/)

-   [MySQL](http://www.mysql.com/)

-   [Node.js](https://nodejs.org)

-   [OpenSSL](https://www.openssl.org/)

-   [Perl](https://www.perl.org/)

-   [PHP](http://php.net/) from [Zend](http://zend.com)

-   [Python](https://www.python.org/)

-   [Redis](https://redis.io/)

-   [Ruby](https://www.ruby-lang.org) from [PowerRuby](http://powerruby.com)

-   [SFTP](https://en.wikipedia.org/wiki/SSH_File_Transfer_Protocol)

-   [OpenSSH](https://www.openssh.com/)

-   zip and unzip

PASE is like AIX is like Linux
==============================

PASE is more or less AIX running on IBM i and is using IBM i as its
kernel. This is why the majority of AIX binaries run in PASE unchanged.
AIX has many similarities to Linux. Because of the close affinity AIX
has with Linux it means many things birthed in the Linux world can be
made to work in PASE on IBM i.

**PASE Facts:**

-   PASE is AIX except using IBM i kernel instead of AIX kernel

-   AIX compiled binaries are **not** emulated in any way

-   PASE processes run in IBM i jobs

-   PASE enforces IBM i security

-   PASE exists as licensed program 5770SS1 option

Here's a visual that shows how PASE communicates with the IBM i SLIC
kernel.

```
          :-------->NODEUSER/QTMHHTTP/432346<---------:
          :                     :                     :
      |----------|---------|  | : |  |----------|---------|
      |        PASE        |  | : |  |       OS/400       |
      | PHP       libc.a   |  | : |  | *PGM       *SRVPGM |
      ========================| : |======================== MI (OS/400)
      AIX/PASE SYSCALL        | : |MI instructions
      privileged mode boundary| : |privileged mode boundary
      ========================| : |========================
      | IBM i SLIC kernel, same for OS/400 + PASE         |
      | (completely replaced AIX kernel /unix)            |
      |---------------------------------------------------|
      |  POWER PC hardware processor                      |
      |---------------------------------------------------|
```

## Please proceed to the next step.
