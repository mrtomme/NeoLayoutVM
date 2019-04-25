# Implementing Neo Layout Mod 3 left and right for Virtualmachines.

This setup works for macOS Mojave / Parallels and VM with Windows7 / Windows 10

When using the Neo Layout on macOS in combination with Karabiner Elements
and virtual machines Mod3 does not work in the VM. 
To get Mod3 running you have to disable the key mapping from macOS for Mod3
when the window from the VM is acitve. Then the normal driver within the VM 
will recognize the original keycode for the two Mod3 keys and not the mapped 
keys for macOS. Then they can be handled from the driver which has to be 
installed in the VM.

For installation see further steps.

## Set up Simple Modifications.

Change the behaviour from caps_lock key. When pressed it should send the
keycode for pc application. This is necessarry because we will remap the 
application key in the VM to Caps-Lock.

## Set up Complex Modifications

Safe the json file to the path ~/.config/karabiner/assets/complex_modifications/
In Karabiner-Elements Preferences go to the Complex Modification Tab. Add rule.
In the list Enable All rules from Neo2_VM.

## Remap application key within the VM.

### Windows

* install the normal neo driver in your Windows VM
* Download randyrants/sharpkeys
* Map application key to caps_lock key

## Source
This mapping has be done by another user for Karabiner and Seil. You could find 
it on the Neo Layout Wiki which is not online while when writing this file.

