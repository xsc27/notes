
## Silverblue Experiment

- Lorax [[docs](https://weldr.io/lorax/)][[source](https://github.com/weldr/lorax)]\
  Lorax is used to build the Anaconda Installer boot.iso.
- Config: https://pagure.io/pungi-fedora/blob/main/f/fedora.conf#_769-796

```sh
mkdir ${HOME}isobuild && cd ${HOME}isobuild
dnf install --assume-yes rpm-ostree lorax git-core
git clone --branch main --depth=1 https://pagure.io/fedora-lorax-templates.git
lorax \
  --product Fedora \
  --version rawhide \
  --release "$(printf '%(%Y-%m-%d)T')" \
  --source https://kojipkgs.fedoraproject.org/compose/rawhide/latest-Fedora-Rawhide/compose/Everything/x86_64/os/ \
  --variant Silverblue \
  --volid Fedora-SB-ostree-x86_64-rawhide \
  --nomacboot \
  --logfile $(pwd)/lorax.log \
  --tmp $(pwd)/tmp \
  --add-template $(pwd)/fedora-lorax-templates/ostree-based-installer/lorax-configure-repo.tmpl \
  --add-template $(pwd)/fedora-lorax-templates/ostree-based-installer/lorax-embed-repo.tmpl \
  --add-template $(pwd)/fedora-lorax-templates/ostree-based-installer/lorax-embed-flatpaks.tmpl \
  --add-template-var ostree_install_repo=ostree_install_repo=https://kojipkgs.fedoraproject.org/compose/ostree/repo/ \
  --add-template-var ostree_update_repo=ostree_update_repo=https://ostree.fedoraproject.org \
  --add-template-var ostree_osname=fedora \
  --add-template-var ostree_oskey=fedora-37-primary \
  --add-template-var ostree_contenturl=mirrorlist=https://ostree.fedoraproject.org/mirrorlist \
  --add-template-var ostree_install_ref=fedora/rawhide/x86_64/silverblue \
  --add-template-var ostree_update_ref=fedora/rawhide/x86_64/silverblue \
  --add-template-var flatpak_remote_name=fedora \
  --add-template-var flatpak_remote_url=oci+https://registry-no-cdn.fedoraproject.org \
  --rootfs-size 8 \
  --skip-branding \
  ./results/
```

### Error
```
subprocess.CalledProcessError: Command '['ostree', '--repo=/root/isobuild/tmp/lorax.gywgheib/installtree/ostree/repo', 'pull', '--mirror', 'fedora', 'fedora/rawhide/x86_64/silverblue']' returned non-zero exit status 1.
```
https://gist.github.com/JayDoubleu/6d0409b657fe84ea53ef0fa9da8d8e63
```sh
--add-template-var "ostree_install_repo=file://$(pwd)/repo" \
--add-template-var "ostree_update_repo=file://$(pwd)/repo" \
```
		
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3MzgzODcwNjksLTc2ODc1NTQ3MywtMT
czNDE0NTg4NywtMTEwMzA0Mzc1NSwxMjA0NTE1MDMwLC05MDYy
MzQ5ODQsLTg4MjQwNDIwNSwxNzc1MzEwNzU5LDExMzUzMTkyNj
FdfQ==
-->