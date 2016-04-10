---
title: How to fix the OpenVPN client issue in El Capitan
---

<p>With El Capitan, Apple introduced a new security feature: System Integrity Protection, preventing admin users from modifying many system files and directories.</p>

<p>That new feature can also prevent you from using the OpenVPN client, therefore if you're getting an error like this:</p>

<img src="https://farm2.staticflickr.com/1615/26285322271_e4d31d27d6_o.jpg" width="362" height="101" alt="openvpn_error_elcapitan">

<p>You'll need to disable System Integrity Protection using the following procedure:</p>

<ul>
<li>Reboot the Mac and hold down the <code>cmd+R</code> keys simultaneously after the screen turns black until the Mac boots into Recovery Mode.
<li>When the <b>OS X Utilities</b> screen appears, click on <b>Utilities</b> in the menu bar and select <b>Terminal</b>.
<li>To disable SIP, enter the following and press return:
<code>csrutil disable</code>
<li>A confirmation message will then ask you to reboot, type <code>reboot</code> and hit return.
</ul>

<p></p>

<p>If you wish to re-enable SIP, repeat the above steps and type:
<code>csrutil enable</code></p>