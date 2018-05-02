---
layout:    page
title:     color_consensus
permalink: /color_consensus/
---

As part of my bachelor thesis, I am conducting an experiment to find out if blockchain technology can create new ways of decentralized music collaboration for sample based music.

![](/images/color_consensus/colors.png)

[color_consensus](http://colorconsensus.xyz) is a decentralized database of sounds matched with color values. I will be using this to create music based on the samples and color values chosen by the uploaders.
While I’ll be inviting a couple artists to participate for my focus group, the tool will be available to any user with an internet connection and 2 browser extensions. This means that anyone can collaborate by adding their own sounds to the database, even if I didn’t invite them.

As such, each user is personally responsible for the content they upload.
__Please only share your own content, and keep in mind that by doing so it might end up in the music.__

# IPFS
As opposed to server based location addressing of files (HTTP), IPFS accesses content via unique (and long) hashes.
In practise, this means that as long as at least one node has the files, anyone can access them. All samples, and even the whole client side web interface of this project are hosted on IPFS.

To upload files, a fast way to get started is to use IPFS Companion for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ipfs-companion/) or [Chrome](https://chrome.google.com/webstore/detail/ipfs-companion/nibjojkomfdiaoajekhjakgkdhaomnch).

![](/images/color_consensus/ipfs_companion_embedded.png)

If you add a sound file to IPFS using the plugin, it'll spit out a long hash starting with Qm..

![](/images/color_consensus/ipfs_hash.png)

This hash references back to your sound file. To share it with the world, it needs to be stored in a public way.

# Ethereum

Ethereum serves as the database which stores the hashes linking to audio samples. As it currently runs on a proof-of-work blockchain, storing data costs a small amount of gas. Reading from it, however, is free. The gas cost acts as a form of spam prevention, as a spammer would need to have infinite funds to spam the network long term.

To connect to the Ethereum blockchain, please install the [Metamask](https://metamask.io/) extension. __Be sure to select the Rinkeby test network, as we're not using money with real value in this experiment.__

![](/images/color_consensus/metamask.png)

# Usage

You don’t have to finish tracks or be a great sound designer to participate. [color_consensus](http://colorconsensus.xyz) allows users to upload any type of audio material and pass it back into the database for others to use.
To get started, here are some ideas of what you could do:

- create samples from scratch
- share field recordings you weren't going to use anyways
- sample/process existing files to feed back into the database
- sequence existing files into loops, melodies & grooves
- get inspired by the pretty colors and make some music

The more samples we create in the process, the more fun it’ll be!
