---
layout:    page
title:     color_consensus
permalink: /color_consensus/
---

__The tool is not live yet, but this guide should get everything you need ready.
This page will be updated with more info once the tool is finished.__

As part of my bachelor thesis, I am conducting an experiment to find out if blockchain technology can create new ways of decentralized music collaboration for sample based music.
I'm using the term "blockchain" to describe a broad set of components, which together create a decentralized online platform which is immutable, censorship resistant and open to everyone.

This project will be used to create a sample based electronic music EP in collaboration with other artists. While I’ll be inviting a selected few to participate for my focus group, the tool will be available to any user with an internet connection and 2 browser extensions. This means that anyone can collaborate by adding their own sounds to the database, even if I didn’t invite them.

As such, each user is personally responsible for the content they upload.
Please only share your own content, and keep in mind that by doing so it might end up in the music.

# IPFS
As opposed to server based location addressing of files (HTTP), IPFS accesses content via unique (and long) hashes.
In practise, this means that as long as at least one node has the files, anyone can access them. All samples, and even the whole client side web interface of this project are hosted on IPFS.

To upload files, a fast way to get started is to use IPFS Companion for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ipfs-companion/) or [Chrome](https://chrome.google.com/webstore/detail/ipfs-companion/nibjojkomfdiaoajekhjakgkdhaomnch).

![](/images/resample-space/ipfs_companion_embedded.png)

If you add a sound file to IPFS using the plugin, you'll get a long hash, which represents the file in the network.

![](/images/resample-space/ipfs_hash.PNG)

# Ethereum

Ethereum serves as the database which stores the hashes linking to audio samples. As it currently runs on a proof-of-work blockchain, storing data costs a small amount of gas. Reading from it, however, is free. The gas cost acts as a form of spam prevention, as a spammer would need to have infinite funds to spam the network long term.

To connect to the Ethereum blockchain, we use the [Metamask](https://metamask.io/) extension. Be sure to stay on the Rinkeby test network, as we're not using money with real value in this experiment.

![](/images/resample-space/metamask.png)

# Usage

You don’t have to finish tracks or be a great mix engineer to participate. resample.space allows users to take existing audio material, add to it and pass it back into the database for other users to iterate over. The most exciting pieces of music to result from this experiment are the ones slowly created from various different artists over multiple iterations.
To get started, here are some ideas of what you could do:

- create samples to upload
- sample/process existing files to feed back into the database
- sequence existing files into loops, melodies & grooves

The more samples we create in the process, the more fun it’ll be!
