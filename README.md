![Ww0Xt1mAMy31Ofar0GYu8Oab0v2k0uF1XT_zTt5kPU1M8o58sT5OOXCsSxv3nNGxsG8dG4zI=w1060-fcrop64=1,00005a57ffffa5a8-k-c0xffffffff-no-nd-rj (1)](https://user-images.githubusercontent.com/1176339/155262320-ce1406f0-d35d-418e-a8b9-60b928cceeb2.jpeg)

# 🔥🔥 RASPBERRY PI PROJECTS WITH OCULUS: I HACKED AN RC Car To Drive It With VR! 🔥🔥

## YouTube Video:

[![IMAGE ALT TEXT](http://img.youtube.com/vi/MYJcSZqk_Tg/maxresdefault.jpg)](https://youtu.be/MYJcSZqk_Tg "YouTube video")

<https://youtu.be/MYJcSZqk_Tg>

## Projects breakdown

### Oculus Unity App

#### Unity instructions

##### Unity Editor Version
2021.3.8f1

Complete the Official Oculus Tutorial back to back
https://developer.oculus.com/documentation/unity/unity-gs-overview/

Open <https://github.com/security-union/oculus-rc-car-control/tree/main/VR%20Control> and make sure to Set OVRPlugin to Legacy:
<img width="100%" alt="Schermata 2022-08-31 alle 9 22 28 PM" src="https://user-images.githubusercontent.com/1176339/187812466-7089cf51-85a3-444b-92e4-cbc109dd94e0.png">

### Raspberry PI

<https://github.com/security-union/oculus-rc-car-control/tree/main/raspberry-pi>

### Protobuf

Messages used to communicate the raspberry pi with the Oculus

<https://github.com/security-union/oculus-rc-car-control/tree/main/protobuf>

## Instruction for the project

### To know

First of all, you have to know that some libraries are bound to evolve and that can generate errors during compilation. This tutorial applies an update of some libraries like Rav1e which was previously in version 0.5.1 in this project. We will use version 0.6.1 to be able to compile this project.

### To do

#### on the raspberry pi

Update and upgrade the system

<pre><code>sudo apt-get update
sudo apt-get upgrade
</code></pre>

After you need to install cargo

<pre><code>sudo apt-get install curl
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
</code></pre>

Modify the Cargo.toml in Oculus-rc-car-control-main/raspberry-pi/video-streaming/Cargo.toml

On the line rav1e = "0.5.1" -> rav1e = "0.6.1"

Make a cargo build

<pre><code>cargo build
</code></pre>

#### on the dev machine

Update and upgrade the system

<pre><code>sudo apt-get update
sudo apt-get upgrade
</code></pre>

After you need to install cargo

<pre><code>sudo apt-get install curl
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
</code></pre>

Modify the Cargo.toml in Oculus-rc-car-control-main/raspberry-pi/video-streaming/Cargo.toml

On the line rav1e = "0.5.1" -> rav1e = "0.6.1"

Make a cargo build

<pre><code>cargo build
</code></pre>

#### on unity

