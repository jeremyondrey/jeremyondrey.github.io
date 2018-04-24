---
layout:    page
title:     resample.space
permalink: /resample-space/
---

As part of my bachelor thesis, I am conducting an experiment to find out if blockchain technology can create new ways of music collaboration for sample based music.
I'm using the term "blockchain" to describe a broad set of components, which together create a decentralized online platform.

This project will be used to create an EP in collaboration with other artists. While I've explicitly invited a couple people to participate, the tool will be available to any user with an internet connection and 2 browser extensions.

# IPFS
As opposed to server based location addressing of files (HTTP), IPFS accesses content via unique (and long) hashes.
In practise, this means that as long as at least one node has the files, anyone can access them. All samples, and even the whole client side web interface of this project are hosted on IPFS.

To upload files, a fast way to get started is to use IPFS Companion for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ipfs-companion/) or [Chrome](https://chrome.google.com/webstore/detail/ipfs-companion/nibjojkomfdiaoajekhjakgkdhaomnch).

![](/images/resample-space/ipfs_companion_embedded.png)

If you add a sound file to IPFS using the plugin, you'll get a long hash, which represents the file in the network.

![](/images/resample-space/ipfs_hash.png)

# Ethereum

Ethereum serves as the database which stores posted audio samples. As it currently runs on a proof-of-work blockchain, storing data costs a small amount of gas. Reading from it, however, is free. The gas cost acts as a form of spam prevention, as a spammer would need to have infinite funds to spam the network.

To connect to the Ethereum blockchain, we use the [Metamask](https://metamask.io/) extension. Be sure to stay on the Rinkeby test network, as we're not using money with real value.

![](/images/resample-space/metamask.png)

If you have everything set up, head over to [resample.space](http://resample.space) to get involved!
