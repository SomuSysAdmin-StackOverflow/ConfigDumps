**This file is to provide a repository for the files referenced in the StackOverflow Question :** [
Host can't talk to the guest VM when the IP is changed from DHCP assigned dynamic to static
](https://superuser.com/questions/1298203/host-cant-talk-to-the-guest-vm-when-the-ip-is-changed-from-dhcp-assigned-dynami) by _@SomuSysAdmin_

---

## Host Config:
### 1. Nat Config
[Contents of `/etc/vmware/vmnet10/nat/nat.conf` of the **host**](https://github.com/SomuSysAdmin-StackOverflow/ConfigDumps/blob/master/1.NetworkSetup_VMnet10/host_vmnet10_nat.conf)

### 2. DHCP Config:
[Contents of `/etc/vmware/vmnet10/dhcpd/dhcpd.conf` file of the **host**](https://github.com/SomuSysAdmin-StackOverflow/ConfigDumps/blob/master/1.NetworkSetup_VMnet10/host_vmnet10_dhcpd.conf)

### 3. Network Scripts:
* [Contents of `/etc/sysconfig/network-scripts/ifcfg-SomuVMnetWifi`](https://github.com/SomuSysAdmin-StackOverflow/ConfigDumps/blob/master/1.NetworkSetup_VMnet10/ifcfg-SomuVMnetWifi)

* [Output of `$ ifconfig vmnet10` on **host**](https://github.com/SomuSysAdmin-StackOverflow/ConfigDumps/blob/master/1.NetworkSetup_VMnet10/host_vmnet10_ifconfig_output)

---

## Guest Config:
### 1. Guest with DHCP IP [CAN CONNECT WITH HOST]:
[Contents of `/etc/sysconfig/network-scripts/ifcfg-ens33`](https://github.com/SomuSysAdmin-StackOverflow/ConfigDumps/blob/master/1.NetworkSetup_VMnet10/guest_vmnet10_ifcfg-ens33)

### 2. Guest with static IP [CAN'T PING]:
[Contents of `/etc/sysconfig/network-scripts/ifcfg-somuVMnetLAN10`](https://github.com/SomuSysAdmin-StackOverflow/ConfigDumps/blob/master/1.NetworkSetup_VMnet10/guest_vmnet10_ifcfg-somuVMnetLAN10)
