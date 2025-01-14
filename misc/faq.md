---
description: Frequently Asked Questions
---

# FAQ

## My Moralis app ID is publicly visible on the frontend. Is this a security risk?

No. The app ID ("Application ID") is meant to be public and is included in all requests to Moralis. It's ok to include the app ID in a public code repository, such as GitHub. With the app ID, a user can create accounts and call any type of cloud function. To control when new users can sign up, use a "[beforeSave" trigger](https://docs.moralis.io/triggers#beforesave) on the user collection. To learn more about how to lock down your app, see the [Security docs](https://docs.moralis.io/security).

Please Note: You want to protect the master key since it can override all permissions and has full access to read, write, and delete. It's best to use the master key only on the server (i.e., cloud functions). Never use the master key on the frontend.

## FRPC

### What version should I use on Mac?

* frp\_x.xx.x\_darwin\_amd64.tar.gz

### How should I run frpc on Mac?

* Open a terminal.
* Navigate to frpc directory.
* Type `./frpc -c frpc.ini`.

### Why does Mac say that `frpc` is from an "Unidentified Developer"?

This is because `frpc` is not signed for Mac. To allow it to run, follow these steps:

* Navigate to `frpc` folder in Finder.
* Right-click on the `frpc` executable while pressing the "**Ctrl" **key.
* Select **Open**.

Mac will give you information about the risks of overriding the system's security. Please read it carefully and click "**Open"** in the pop-up if you agree.

### What are the risks of giving permissions to `frpc`, even if it is from an "Unidentified Developer"?

`frpc` executable is not signed by Apple. It means that the OS cannot know what kind of code it's going to execute. By accepting to override, or skip the system security, you're telling the OS that you trust the app. Please do so at your own responsibility and risk. To avoid any issues, make sure you've downloaded `frpc` from the official repository at [https://github.com/fatedier/frp/releases](https://github.com/fatedier/frp/releases).

## OpenSea NFTs

### Why are number of NFTs different on OpenSea compared to Moralis API?

Our API can only read data that is public onchain. Lazy minted NFTs on an OpenSea shared contract are stored only in a centralized OpenSea database until the first transfer.

You can find more information on the OpenSea blog: [https://opensea.io/blog/announcements/introducing-the-collection-manager/](https://opensea.io/blog/announcements/introducing-the-collection-manager/).

Another reason may be that the NFTs from the OpenSea inventory are in different chains. In this case, you need to make API requests for each network.

## Sleeping Servers

### What are sleeping servers?

Moralis is on a mission to provide available tools to the web3 development community. This means that we have very generous free plans. This also means that we allow anyone to sign up and spin up Moralis Servers.

However the fact that Moralis Servers are free means that some of them are left running indefinitely without any use. We want all our resources to go to building amazing web3 tech and growing the Moralis Community - we don't want to waste resources running inactive servers.

Thankfully we found a very simple solution 🤩&#x20;

If you are a free tier user you need to confirm that you are still using your servers on a weekly basis. This is how it works 👇

### 😴 Prevent Your Servers from Sleeping&#x20;

Once a week you will get an email prompting you to login to your Moralis account and prevent your server from going to sleep by clicking the _**"Prevent Sleep"**_ button.&#x20;

You have 48 hours to prevent your Moralis server from sleeping. If you don't prevent your server from sleeping it will be temporarily shut down (it will go to sleep 🥱).&#x20;

When a server is shutdown you will experience down time until you wake it up by clicking the _**"Wake Up"**_.

Don't worry - the wake up process will take approximately 30 seconds and your server will be restored to exactly the same state that it was before.

### 🛑 If Your Server Stays Shutdown for 48h

If a server stays shutdown for a period longer than 48 hours it will be terminated.&#x20;

But don't worry - we will back up your server configuration and save it in archive. You will need to recover it by clicking the _**"Recover" **_button.&#x20;

This process is a bit longer than a normal "Wake Up" and can take a few minutes.

Your server will be restored but it will be a fresh server with a new IP and a new URL.

### 🤩 How to Avoid Sleeping Server

To avoid the Sleeping Servers please upgrade to a paid plan.&#x20;

This will support the Moralis developers so that we can continue delivering world-class open source web3 tools without wasting money on inactive servers 🙏

You can upgrade by [clicking here](https://moralis.io/pricing).

As you know we are also working on a self-hosted version of the Moralis Server. When it's out you will be able to host your server on your own server in the future 🏆

### 🤝 If You Need Help

If you want more information regarding sleeping servers or need help please email us at hello@moralis.io and we will help asap!

Keep BUIDLing 👷‍♂️
