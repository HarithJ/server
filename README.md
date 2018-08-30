# Virtualisation with Virtualbox and Vagrant

Virtualisation in simple terms is running an operating system in another operating system. It can help you set up a new environment without impacting or modifying anything on your underlying main operating system by creating a completely new machine, with an independent operating system and only utilizing a small required amount of resources from the underlying system hardware.

To implement this, we are going to need two applications, `Virtualbox` and `Vagrant`.
Make sure you have Virtualbox and Vagrant installed on your machine. If you are using a MacOS machine, you can install them with brew. If you don't have brew installed on your Mac, ~~there's no hope for you,~~ you can follow this [link](https://brew.sh/) to redeem yourself.

#### To install them, run these commands:

Vagrant

`brew cask install vagrant`

Virtualbox:

`brew cask install VIrtualbox`

Vagrant is a tool for building and managing virtual machine environments and makes it quite easy to work with virtual machines.

Virtualbox

Virtualbox is a cross platform virtualisation application. There are other virtualisation applications on the market like VMWare which is cross platform and HyperV a windows specific application but both of these are proprietary software. My preference for free things will have me tell you Virtualbox is the best among them, an unverified personal opinion.

I will be using these 2 (Vagrant and Virtualbox) applications together to setup a windows server on my MacOs computer.

#### Steps

1. Clone this repository

2. Head over to the root folder from the terminal.

3. Run:

   `vagrant up`

   This command will start to download an image has been configured (in our case: https://app.vagrantup.com/jacqinthebox/boxes/windowsserver2016) as per it's details on the Vagrant cloud site to your local machine.

4. Once it's done downloading, it will automatically be setup in virtualbox.

#### Things to note
You can choose your own server image by heading over to https://vagrantcloud.com/ and searching for the image that suits your needs. Once you have found the image you need, click on it and it will take you to a page where there will be details on how to use it. 

When choosing a server to setup up with virtualisation on your local computer you need to take into consideration the minimum requirements necessary for the server to run in comparison with the hardware available on your computer so as not to overwhelm the computer and render it unable to perform tasks on either of the Operating systems optimumly.

If you configure the resources you would like virtual machine to use for a particular box, make sure to leave enough for the operating system on the computer to work optimumly to avoid a slowed performance or the computer freezing entirely.

#### Screenshot of the Server running in Virtualbox

<img width="1680" alt="screen shot 2018-08-16 at 20 20 05" src="https://user-images.githubusercontent.com/5388763/44230028-8f8daa00-a1a2-11e8-9553-38a211435bb7.png">
