# pinera1n
<a href="https://www.pine64.org/pinephone/" >
  <img src="https://www.pine64.org/wp-content/uploads/2020/05/PinePhone-3.jpg" height="320"/>
</a>

## A jailbreak method with linux phone 

I think this is a great way to make checkra1n portable,runs on pinephone and you can use gui  oringinal latest release of checkra1n,and you can operate it with touchscreen ,It called pinera1n because it's checkra1n on pinephone,it's not a expensive but really useful phone,I had tested checkra1n on mobian,so I suggest user run checkra1n with mobian on pinephone,because it required usbmuxd ,others linux distribution might works with a bit different(if interesd about that ,contact me on [twitter](https://twitter.com/powen00hsiao)),it's the most important thing,without it ,iPhone won't connect correctly with pinephone ,now follow the steps to jailbreak with the awesome phone 

**NOTE:odysseyra1n works too on pinephone**

**ADD:others linux phone should work too,called pinera1n just because the first successed case was on pinephone,`distributions based on debian shold work too,like ubuntu touch`**

## Demo 
![Demo photo][1]
![Demo photo][2]
![Demo photo][3]

## Things you need(hardware and mobian image)
- [A pinephone](https://www.pine64.org/pinephone/)
- A usb-c docking bar (contain usb-A to lighting and usb-c charging port,must use usb-A to lightning connect iphone)
- usb-A to lightning
- charging supply with usb-c
- micro sd card 
- [latest release of mobian image](https://mobian-project.org)

## Things you need on mobian
- xterm(for resize terminal size)
- usbmuxd(must need to connect iphone correctly)
- [latest checkra1n release for linux arm64](https://checkra.in)
- king's cross(terminal program on mobian)

## `Things you need on mobian if want odysseyra1n(optional)`
- curl
- libusbmuxd-tools

## Getting  Start

Now following steps to get a friendly easily portable checkra1n ,with this while you lose jailbreak environment,just connect to pinephone,start with friendly gui to rejailbreak,don't need computer 

### Flash mobian to emmc or sd card 

First,you need to flash mobian to pinephone,check this [tutorial](https://wiki.pine64.org/wiki/PinePhone_Installation_Instructions)

### Perpare things will need on mobian

update it first 
```
sudo apt-get update
sudo apt-get upgrade
```
reboot after these 

now install xterm and usbmuxd 
```
sudo apt-get install xterm
sudo apt-get install usbmuxd
```
now give checkra1n permission
```
cd Downloads
chmod +x checkra1n
```
exit terminal and re-open it ,now set the terminal size and scale ,so that we can run checkra1n with GUI ,it will be more friendly to use 

`set terminal scale to 50 % first(set this with the menu on the right top corner) `
type this in terminal ,make sure W bigger than 80 and H 24
```
resize -s 80 24
```
**optional for odysseyra1n**

install curl and libusbmuxd-tools(these are optional,can skip if only need checkra1n)
```
sudo apt-get install curl
sudo apt-get install libusbmuxd-tools
```

### Now we can run checkra1n on pinephone 
connect iphone to pinephone through docking bar,make sure charge your pinephone when progress(charge with docking bar,must do this step ,without this connection will be unstable ),if iphone ask you to verify access to device ,select yes

open checkra1n and run it
```
cd Downloads
cd checkra1n
sudo ./checkra1n
```
if you are on untested version or something need to configure ,you can do that with optional,and you should see the start button avaliable,and follow checkra1n to complete jaibreak,if you want odysseyra1n ,don't open checkra1n ,and keep going

## `If want odysseyra1n then keep going`
quit checkra1n on pinephone and don't open checkra1n on iphone

make sure have installed optional dependencies for odysseyra1n

and paste the command
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/coolstar/Odyssey-bootstrap/master/procursus-deploy-linux-macos.sh)"`
it will require password and type
`alpine`
you will see sileo on iphone ,search and install libhooker and rocketbootstrap,end

## `Advantage of pinera1n`
- portable and friendly to operate with full GUI and touchscreen
- it's a linux phone ,so you can do others thing else,not just a phone for jailbreak
- it's a nice price for this awesome phone,with so much features only need 149 $ for standard pack
- just one command ,and you can get root easily in terminal
- you can underatand well how to do ,because it just need to conncet phone and phone
- with the offical support for linux on arm,it works better than android 
- you can use the latest release of checkra1n on pinephone
- no  complex progress,most of steps on phones
- **odysseyra1n works on pinephone**

## Demo video
just show how I do it ,have upload another video as tutorial video

<a href="https://www.youtube.com/watch?v=M5mNpY8a2zM">
  <img src="https://img.youtube.com/vi/M5mNpY8a2zM/maxresdefault.jpg" >
</a>

## Tutorial video
The progress I used odysseyra1n 

<a href="https://www.youtube.com/watch?v=Ite65xLu4TE">
  <img src="https://img.youtube.com/vi/Ite65xLu4TE/maxresdefault.jpg" >
</a>

## My repo
my repo for jailbreak tweaks [powen00hsiao repo](https://powenn.github.io/powen00hsiao/)

## Introduce pinephone
from wiki :The PinePhone is a smartphone developed by Hong Kong-based computer manufacturer Pine64, intended to allow the user to have full control over the device. Measures to ensure this are: running mainline Linux-based mobile operating systems, assembling the phone with screws, simplifying the disassembly for repairs and upgrades, and providing six kill switches/security switches for components of its hardware.The PinePhone ships with the Manjaro Linux-based operating system using the Plasma Mobile graphic interface, although other distributions can be installed by users.

It's a phone with arm architecture,and run different linux distribution,with linux ,you can do  something cool, like make checkra1n being portable with friendly GUI ,this phone is not expensive,for standard pack only 149 $,spent less than most android phone,but you can have GUI to operate checkra1n easily

# IF YOU HAVE ANY QUESTION,CONTACT ME ON [TWITTER](https://twitter.com/powen00hsiao)

<a href="https://twitter.com/powen00hsiao">
  <img src="https://pbs.twimg.com/profile_images/1404649867033550848/3m6kzjQa_400x400.jpg" height="320"/>
</a>

[1]:https://github.com/powenn/pinera1n/blob/main/photos/01.png
[2]:https://github.com/powenn/pinera1n/blob/main/photos/02.png
[3]:https://github.com/powenn/pinera1n/blob/main/photos/03.png
