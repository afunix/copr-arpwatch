# copr-arpwatch
Repository for Copr to fix crash in arpwatch when a hostname is longer than 33 characters.

Fixes CentOS issues:
- https://bugs.centos.org/view.php?id=12881
- https://bugs.centos.org/view.php?id=17807

# installation
Copr repo: https://copr.fedorainfracloud.org/coprs/afunix/arpwatch/

To install on CentOS 7:
```
yum copr enable -y 'afunix/arpwatch'
yum install arpwatch
```

# background
Based on specs and patches from CentOS 7: https://git.centos.org/rpms/arpwatch/tree/c7

Added the patch from [0012881](https://bugs.centos.org/view.php?id=12881).
