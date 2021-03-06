# ribbit A sound of frog

> Recommend to try this project on **Ropsten Test Network**.

An experimental, decentralized social media web application based on Ethereum platform.  


* [English](./README.md)


Demo: 

* ribbit: http://shd101wyy.github.io/ribbit/
* `#{ribbit}` topic (Ropsten): https://shd101wyy.github.io/ribbit/#/3/topic/ribbit

Smart Contract:

* Main Ethereum Network [0xbbf856d36d04a80d9f526510ceba01ea27627488]
* Ropsten Test Network [0xd8cb86af02684b8ce9c756a6f93f407b0feb4c73]

![](https://user-images.githubusercontent.com/1908863/39964114-7a7d8d20-5642-11e8-8d75-8a823240c36a.PNG)

---

> Below is the obsolete documentation.

**Please read this first:** 

* This project is still under development. We would recommend you to try this project on Ethereum `Ropsten Test Network` instead of `Main Ethereum Network`, because using Ribbit on `Ropsten Test Network` is completely free of charge, and we might deploy new smart contract in the future and deprecate the old one. We might also make changes to the smart contract on `Ropsten Test Network`, so your posts might lose. Please use this project at your own risk.  
* You are responsible for whatever you post. Think twice before you make a post because your post will stay on the blockchain **forever**. It is unchangeable and undeletable. All your posts will stay **public** on blockchain, so please don't post sensitive data.
* We do not host media files for you. We only save your text written in `markdown` to Ethereum blockchain.


<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

![signup1](https://user-images.githubusercontent.com/1908863/40032214-ce4c5ac2-57b8-11e8-960c-490efb893258.PNG)


> You may notice the `MetaMask` window pops up when you click `Publish profile to blockchain` button, that is because writing data to blockchain isn't free. You would have to pay for the miner to execute the transaction. You only need to change the `Gas Price` field in the MetaMask window. The higher `Gas Price` you set, the faster the transaction will be executed.
>
> ![metamask](https://user-images.githubusercontent.com/1908863/40032235-e3bf72fe-57b8-11e8-894a-6bfea9e39c3b.PNG)



## Make a post

To make post, click the green `Ribbit` button.

Posts in ribbit are written in Markdown.
There are two types of posts now:

* Normal post

for example:

```markdown
This is a normal post written in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).
```

* Article post

for example:

```markdown
![](article/cover/image.png)

# Article title

my content goes here
```

### Post to topic

You can make a post to a topic by writing `#{topic}`.  
For example:

```markdown
Hello #{world} will post this to `world` topic
```

### Mention a user

You can mention a person in your post by writing `@{username}`.  
For example:

```markdown
Hi @{ribbit} will notify the user `ribbit` this about post.
```

### Embed videos

For example: 


## What will be saved to blockchain and what will not

Will be on blockchain:
* Your profile information like your username, bio, avatar url, and cover url.
* Your posts written in markdown.

Will not be on blockchain:
* Your media files written in your markdown post, such as images, videos, etc...
* Your followings, faviorite topics, setttings will be saved locally in your browser. 


## Developer section

### Development

```bash
$ npm run frontend:prepare # install necessary node modules for development
                         # on Windows, you might need to run the following in advance:
                         #   $ npm install --global --production windows-build-tools
$ npm run frontend:dev     # start building and watching.
                         # then open a new terminal and run =>
$ npm run server:start     # start a static http server at address http://127.0.0.1:12345.
```

### Deployment

```bash
$ npm run frontend:build
```

then copy `./dist` to your server.


