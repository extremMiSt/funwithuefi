# funwithuefi
I just wanted to have some fun with uefi.

## what is this?
This is a small pong game written with gnu-efi.

## how to build
first you need to install the gnu-efi package for your system.
I am on Linux Mint, where that is as easy as
```
sudo apt install gnu-efi
```
After that you should jsut be able to
```
make
```
The Makefile assumes that your gnu-efi files are in the standard paths for Linux Mint. on other systems you mgiht have to change that to the correct folders.
After compilation the resulting *.efi file needs to be moved to the ESP of your (virtual) machine, for example with:
```
cp ./hello.efi /boot/efi/EFI/
```
From there on it should be selectable as a bootable thing in your uefi firmware.

## how to play
After starting the game player 1 moves their paddle with `q` and `a`, while player 2 uses `o` and `l`.
