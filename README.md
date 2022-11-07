# ansible_tutorial

This is my New ansible Repository!!!

IOS Open-ssh Bug Fix
https://community.cisco.com/t5/cisco-bug-discussions/cisco-ios-does-not-support-openssh-6-4/td-p/2354553

In /etc/ssh/ssh_config write:

Host *
        GSSAPIAuthentication yes
#       KexAlgorithms=diffie-hellman-group14-sha1
        KexAlgorithms=curve25519-sha256@libssh.org,ecdh-sha2-nistp256,ecdh-sha2-nistp384,ecdh-sha2-nistp521,diffie-hellman-group-exchange-sha256,diffie-hellman-group14-sha1,diffie-hellman-group1-sha1
