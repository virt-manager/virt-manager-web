# Manage virtual machines with virt-manager

The virt-manager application is a desktop user interface for managing
virtual machines through libvirt. It primarily targets KVM VMs, but
also manages Xen and LXC (linux containers). It presents a summary
view of running domains, their live performance & resource utilization
statistics. Wizards enable the creation of new domains, and configuration
& adjustment of a domain’s resource allocation & virtual hardware. An
embedded VNC and SPICE client viewer presents a full graphical console
to the guest domain.

<script type="text/javascript" src="jquery.fancybox/jquery-1.3.2.min.js"></script>
<script type="text/javascript" src="jquery.fancybox/jquery.easing.1.3.js"></script>
<script type="text/javascript" src="jquery.fancybox/jquery.fancybox-1.2.1.js"></script>
<script type="text/javascript">
  $(document).ready(function() {
      $("a.fb").fancybox({
        'hideOnContentClick': true,
        'overlayOpacity': 0.9,
        'overlayShow': true,
        'padding': '20',     });
  });
</script>

<p class="screenshots">
  <span class="image">
    <a class="fb" title="Virtual machine list" href="static/manager.png" rel="ss">
      <img src="static/manager-small.png" alt="Virtual machine list" width="350" height="197" />
    </a>
  </span>
  <span class="image">
    <a class="fb" title="Guest CPU" href="static/details.png" rel="ss">
      <img src="static/details-small.png" alt="Guest CPU" width="350" height="197" />
    </a>
  </span>
  <span class="image">
    <a class="fb" title="Guest console" href="static/console.png" rel="ss">
      <img src="static/console-small.png" alt="Guest console" width="350" height="197" />
    </a>
  </span>
</p>

## About virt-manager’s supporting tools

* *virt-install* is a command line tool which provides an easy way to
  provision operating systems into virtual machines.

* **virt-viewer** is a lightweight UI interface for interacting with the
  graphical display of virtualized guest OS. It can display VNC or SPICE,
  and uses libvirt to lookup the graphical connection details.

* **virt-clone** is a command line tool for cloning existing inactive guests.
  It copies the disk images, and defines a config with new name, UUID and MAC
  address pointing to the copied disks.

* **virt-xml** is a command line tool for easily editing libvirt domain XML
  using virt-install’s command line options.

* **virt-bootstrap** is a command line tool providing an easy way to setup
  the root file system for libvirt-based containers.
