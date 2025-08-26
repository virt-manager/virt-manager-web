# Download

## Current releases

### virt-manager

[virt-manager 5.1.0](https://releases.pagure.org/virt-manager/virt-manager-5.1.0.tar.xz) [(gpg)](https://releases.pagure.org/virt-manager/virt-manager-5.1.0.tar.xz.asc) Tuesday August 26, 2025


Releases are curently GPG signed by Pavel Hrdina using
a key having the fingerprint:

```
4252 D86A 5204 1137 C291 CADF C85C 5E95 7062 A701 (4096R)
```

Releases 4.1.0 and older are GPG signed by Cole Robinson using
a key having the fingerprint:

```
D8F5 BE72 9291 CC5E FE4B 4D09 6455 9E28 C21C C7A8 (4096R)
```

* cli: Support --cpu maximum (Andrea Bolognani)
* Prefer maximum mode for many emulated guests (Andrea Bolognani)
* virt-manager: Fill in model combo with advertised values by libvirt (Lin Ma)
* virt-manager: Default to same snapshot mode as currently used snapshot
* virt-manager: Warn users to not mix snapshot modes
* cli: Add --memdev target.dynamicMemslots support for virtio-mem (Lin Ma)
* cli: add target.memReserve for pci-bridge and pcie-root-port controllers (Lin Ma)
* cli: Add --disk driver.queue_size support (Lin Ma)
* cli: Add 'poll' settings for iothread (Lin Ma)
* cli: Add --tpm backend.profile.{source,removeDisabled} support (Lin Ma)
* cli: Add nvram.templateFormat to indicate template format (Lin Ma)
* cli: Add --features hyperv.xmm_input.state=on/off (Lin Ma)
* cli: Add --features hyperv.emsr_bitmap.state=on/off (Lin Ma)
* cli: Add --features hyperv.tlbflush.direct.state=on/off (Lin Ma)
* cli: Add --features hyperv.tlbflush.extended.state=on/off (Lin Ma)
* virt-manager: Add riscv64 to prioritized architectures (Heinrich Schuchardt)
* virtinst: Add --pstore backend=acpi-erst,path=XX,size=YY support (Lin Ma)
* XML: Fix escaping special characters twice in some cases (Marius Vollmer)
* Add riscv64 architecture for Debian ISO/URL detection (Heinrich Schuchardt)
* virt-manager: list virtual networks when creating new QEMU Session VM
* Add support for vDPA network devices (Joren)
* virt-install: Detect wayland in order to start virt-viewer
* Improve Debian/Ubuntu detection for ISO images
* Allow spaces, disallow slashes in names (AbhinavTiruvee)
* cli: Add support to fetch cloud-init config files from URL
* virt-manager: Fix error when opening File Browser (Zahid Kizmaz)
* virt-manager: Add Ctrl+Alt+Shift+Esc key command for logind's SecureAttentionKey (n3rdopolis)
* cli: Add support for creating TDX VMs
* virt-install: Improve default device models to improve Windows ARM support (Akihiko Odaki)
* Add support to configure startup policy for USB passed through devices (Lin Ma)

### virt-viewer

[virt-viewer 11.0](https://releases.pagure.org/virt-viewer/virt-viewer-11.0.tar.xz)
[(gpg)](https://releases.pagure.org/virt-viewer/virt-viewer-11.0.tar.xz.asc)
Friday November 18th, 2021
[Win x86 MSI](https://releases.pagure.org/virt-viewer/virt-viewer-x86-11.0-1.0.msi)
[(gpg)](https://releases.pagure.org/virt-viewer/virt-viewer-x86-11.0-1.0.msi.asc)
[Win x64 MSI](https://releases.pagure.org/virt-viewer/virt-viewer-x64-11.0-1.0.msi)
[(gpg)](https://releases.pagure.org/virt-viewer/virt-viewer-x64-11.0-1.0.msi.asc)

Virt-viewer releases are curently GPG signed by Daniel P. Berrange using
a key having the fingerprint:

```
DAF3 A6FD B26B 6291 2D0E 8E3F BE86 EBB4 1510 4FDF (4096R)
```

This same fingerprint is listed at time of the release announcements mails
on the mailing list

* Minimum libgovirt is now 0.3.7
* CentOS 7 is no longer a supported build platform
* Use header bar for oVirt ISO dialog
* Add change CD button to toolbar for oVirt
* Support using ISOs in oVirt DATA storage domains
* Remove clashing -r command line shortcut for ‘resize’ that clashed with
  existing ‘reconnect’ shortcut
* Support modifier-only hotkeys for cursor release
* Fix smartcard and USB hotkey configuration regression
* Add USB device reset hotkey support
* Fix various mixed up GTK actions for hotkeys
* Release keyboard grab at same time as mouse grab with SPICE
* Fix misc compiler warnings with glib > 2.68
* Fix creation of window when guest uses multiple heads with a single QXL
  video card
* Updated translations from weblate
* Avoid warnings from GTK from overly strict minimum desktop width/height rules
* Update window action sensitivity to fix regression causing disabled send key
  menu items
* Fix mixed up action / menu state when user cancels a quit request
* Ensure auth dialog credential fields are cleared
* Fix setting os-id when building RPMs
* Avoid extra hyphen in build ID strings
* Explicitly disable spice/ovirt features when invoking meson for RPM builds
* Fix uninitialized variable for keymaps

### virt-bootstrap

[virt-bootstrap 1.1.1](https://releases.pagure.org/virt-bootstrap/virt-bootstrap-1.1.1.tar.gz) [(gpg)](https://releases.pagure.org/virt-bootstrap/virt-bootstrap-1.1.1.tar.gz.sig) Tuesday Jul 9th, 2019

* Don’t expose the root password via command line
* Set SElinux file context of destination folder
* Use absolute destination path
* safe-untar: Inherit SElinux context
* don’t allow overwriting of the root partition

## Previous releases

* virt-manager: [Sources](https://releases.pagure.org/virt-manager/) and [Changelogs](https://github.com/virt-manager/virt-manager/blob/master/NEWS.md)
* virt-viewer: [Sources](https://releases.pagure.org/virt-viewer/) and [Changelogs](https://gitlab.com/virt-viewer/virt-viewer/-/raw/master/NEWS)
* virt-bootstrap: [Sources](https://releases.pagure.org/virt-bootstrap/) and [Changelogs](https://github.com/virt-manager/virt-bootstrap/blob/master/NEWS.md)

## Verifying gpg signatures

As a quick guide, to import a key from the key servers and verify downloads use.

```
$ gpg --recv-key 0xBE86EBB415104FDF
$ gpg --fingerprint 0xBE86EBB415104FDF
...check it matches fingerprint above...
$ gpg --verify SIGNATURE-FILE  SOURCE-FILE
```
