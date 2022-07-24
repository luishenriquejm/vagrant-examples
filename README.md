# vagrant-examples
Vagrantfile examples

Here you will find some Vagrantfile examples that I use in my daily life.

[Original](Vagrantfile_original) => Original file from version 2.2.19

[Simple](Vagrantfile_simple) - Simple Vagrantfile with just the vm image and a public network in bridge mode

[Custom](Vagrantfile_custom) - Some custom configurations

[Mutiple-VMs](Vagrantfile_multiple_vms) - Multiple vms in the same Vagrantfile

[Loop](Vagrantfile_loop) - A loop structure to create as much vms as you want with the same configuration

[Mutiple-VMs-with-loop](Vagrantfile_multiple_vms_with_loop) - Multiple vms with loop config to create more than one vm with the same image/config

[VirtualBox-provider](Vagrantfile_virtualbox) - Simple configs for VirtualBox provider

[VMWare-provider](Vagrant_vmware) - Simple configs for VMWare provider

You can find the availables vagrant boxes here &rarr; <https://app.vagrantup.com/boxes/search>

---

## Managing box images

### List all local image boxes:
```
vagrant box list
```

### List and give the status of all created boxes:
```
vagrant global-status
vagrant global-status --prune
```

### If you prefer to pre download you vagrant boxes:

```
vagrant box add generic/oracle8
vagrant box add generic/oracle8 --provider vmware_desktop
vagrant box add generic/oracle8 --provider vmware_desktop --box-version 4.0.2
```

### Updating vagrant boxes
```
vagrant box outdated --global
vagrant box update --box <box_image_name>
```

### Removing boxes:
```
vagrant box remove generic/oracle8
vagrant box remove generic/oracle8 --provider vmware_desktop
vagrant box remove generic/oracle8 --provider vmware_desktop --box-version 4.0.2
```