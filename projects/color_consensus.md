---
layout:    page
title:     color_consensus
permalink: /color_consensus/
---


#NOTE: most info on this page is outdated, as I'm currently looking into Bitcoin/Lightning based systems.


As part of my bachelor thesis, I am conducting an experiment to find out if blockchain technology can create new ways of decentralized music collaboration for sample based music.

![](/images/color_consensus/colors.png)

[color_consensus](http://colorconsensus.xyz) is a decentralized database of sounds matched with color values. Its main components are:

- a content addressed data structure (IPFS), which makes sound files available to users regardless of who hosts them

- a blockchain (Ethereum) and smart contracts, which list files and their matching color values

Traditional music distribution is struggling with the fact that digital files are easy to share, color_consensus uses this as its main feature. The platform is designed to encourage a free flow of ideas, while being as simplified and open as possible. Music as a form of expression should not have to depend on centralized platforms, which can shut down, lose data or get hacked.
Since all transactions are public, every upload can be traced back to the original uploader.

I’ll be inviting a couple artists to collaborate for a music project, but the page will be available to any user with an internet connection and 2 browser extensions. This means that anyone can participate by adding their own sounds to the database, even if I didn’t invite them.

As such, each user is personally responsible for the content they upload.
__Please only share your own content, and keep in mind that by doing so it might end up in other people's work.__


# IPFS
As opposed to server based location addressing of files (HTTP), the Inter Planetary File System accesses content via unique cryptographic hashes.
In practise, this means that as long as at least one node in the network has the files, anyone can access them. All samples, and even the whole client side web interface of this project are hosted on IPFS.

To upload files, a fast way to get started is to use IPFS Companion for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ipfs-companion/) or [Chrome](https://chrome.google.com/webstore/detail/ipfs-companion/nibjojkomfdiaoajekhjakgkdhaomnch).

![](/images/color_consensus/ipfs_companion_embedded.png)

To directly connect to IPFS nodes, it is recommended to install the [CLI](https://ipfs.io/docs/install/). The directory contains an install.sh file, after which you run the commands `ipfs init` and `ipfs daemon` in your favorite command line. If you only use the web extension, links will default to the ipfs.io gateway.

If you add a sound file to IPFS using the plugin, it'll spit out a long hash starting with Qm..

![](/images/color_consensus/ipfs_hash.png)

This hash references back to your sound file. When another user requests the file, it will be served directly from the IPFS node in your browser. As more nodes have access to the file over time, the file becomes more accessible and increasingly more robust.

If nobody knows the content hash, the sound can’t be heard by anyone. To solve this, we need a way of sharing it with the public.

# Ethereum

[Ethereum](https://en.m.wikipedia.org/wiki/Ethereum) serves as the database which stores our sounds. Because IPFS hashes are hard to read by humans, users get to pick a matching color for each upload.

__Once a hash is stored in the database, it cannot be deleted. It will remain in the blockchain for as long as Ethereum exists.__

To connect to the Ethereum blockchain, please install the [Metamask](https://metamask.io/) extension. __Be sure to select the Rinkeby test network, as we're not using real money in this experiment.__

![](/images/color_consensus/metamask.png)

With this extension, we are able to interact with the Ethereum blockchain. Reading from it is free, but writing to it costs a small amount of gas. Because Rinkeby is a test network, the currency we are using can be obtained [for free](https://faucet.rinkeby.io/)

# Usage

You don’t have to finish tracks or be a great sound designer to participate. [color_consensus](http://colorconsensus.xyz) allows users to upload any type of audio material and pass it back into the database for others to use.
To get started, here are some ideas of what you could do:

- create samples from scratch
- share field recordings you weren't going to use anyways
- sample/process existing files to feed back into the database
- sequence existing files into loops, melodies & grooves
- get inspired by the pretty colors and make some music

The more samples we create in the process, the more fun it’ll be!
