+++
title = "elastOS (Trinity)"
weight = 80
chapter = false
pre = ""
alwaysopen = false
+++

### About

**elastOS** is a container that provides Elastos DApp running environment. Based on the trusted running environment of Elastos Runtime, elastOS provides a reliable running environment for applications to protect digital contents.

elastOS integrates all the services that Elastos provides and combines them into a singular mobile application/framework for DApp developers to use. For this reason, DApp developers only need to write their application using ionic javascript framework and have only one set of Runtime APIs to manage. 

elastOS is supported on both Android and iOS, DApp developers only need to develop their application using one set of code in order to run on both platforms, inside the elastOS app.

**Ionic** is a powerful HTML5 application development framework (HTML5 Hybrid Mobile App Framework). The developers can use HTML, CSS and Javascript web develoment skills to create an App with near native  experiences. Ionic framework focus on outlook, users' experiences and interaction. It is most suitable for devlopment of HTML5 hybrid mobile App.

Ionic is a lightweight UI library. It is responsive with modern and beautiful interfaces.

### Status

End users can already use elastOS - albeit as a minimal viable product - and access some of its core features. That said, throughout 2019 elastOS is scheduled to undergo a variety of changes and augment a number of new features, so the finished product may not at all resemble elastOS Browser in its early stages. As of now, it has entered an open beta where community members can begin using the Browser and reporting bugs to the developers. Developers then play two major roles throughout the beta process: they provide fixes to reported bugs and continue to create new features as they build out the beta. While elastOS is by no means prepared for mass production, it is nonetheless at a meaningful development stage where testing and trial runs have begun.

### Why is elastOS special?

What elastOS offers is one level above blockchain-based trust because it interacts with all the Elastos services such as Elastos mainchain, DID sidechain, Ethereum sidechain, NEO sidechain, token sidechain, Elastos Carrier, Elastos Hive, etc while preventing applications from accessing any APIs or plugins that are not supported by the Elastos runtime. In that way, users can utilize the blockchain or run smart contracts via the DApps that everyday users use on their devices without having to interface with the blockchain to begin with. elastOS hides away the infrastructure layer and provides a set number of APIs for DApp developers to use. In turn, users access the DApps with the trust and security of the blockchain without ever having to deal with it directly. Rather profoundly, elastOS combines on-chain and off-chain scalability solutions into one platform and packages data in such a way that developers don’t have to learn anything new to develop their DApps on its platform. It is a portal to the vast Elastos ecosystem that everyday users will interact with on a daily basis.

### elastOS vs native Elastos apps
- You can build Apps for elastOS (Elastos Browser) using Ionic/Cordova framework while native apps are written in Android/Swift
- http/https is disabled by default inside elastOS and Apps can only use Elastos Carrier to communicate to the outside world so this means current internet sites such as google, facebook won't be directly accessible
- elastOS is itself an app that can be downloaded onto a smart phone via Android or Apple store so elastOS App(aka Elastos Browser app) is just an app like any other on your smart phone. However, when you open elastOS, you get to yet another home screen of the Elastos Ecosystem where you'll find Ionic based apps and these apps can only run inside elastOS Browser
- The kind of apps you can build for elastOS browser are not going to be as sophisticated as native apps such as gaming apps that use a lot of resources and memory. Most of the Apps for elastOS will include platforms to interact with the blockchain for authentication and payment and smart contract logic, sending message over a secure channel using Elastos Carrier and storing data in a decentralized storage called Elastos Hive. So, in a way, the kind of apps that are best suitable for elastOS are those that prioritize the safety of personal data and digital assets
- Ionic based apps are hybrid apps in a sense that they're interacting with the base hardware(smart phones) via Cordova plugins which means apps for elastOS browser will usually be slower compared to Native apps which directly communicate with the hardware. A little bit of speed is sacrificed for a massive security gain that users will see for using apps made for elastOS
- Apps such as Elephant Wallet use a blockchain node to perform actions such as authenticating someone using DID or sending ELA to another person. This means the wallet is interacting with nodes that are controlled by the Elephant Wallet team. This is not 100% centralized but still a good solution because this app sacrifices some decentralization in favor of speed. However, if you were to create a wallet for elastOS, it would have to be an SPV based wallet which would be a completely decentralized wallet as there's no one entity controlling any blockchain nodes. The currently available ELA wallet for android/iphone is also a type of SPV wallet. There are tradeoffs to be considered when choosing to develop an app for elastOS as 100% decentralized solutions might not be suitable for all use cases as they tend to be slower compared to centralized apps

### DApp Lifecycle in elastOS Browser
- Build an application using the Ionic javascript framework, utilizing various cordova plugins supported by the browser such as elastos carrier plugin, camera plugin, etc.
- Use the toolchain scripts provided as part of the framework in order to convert your Ionic application to an elastos application that can be run inside elastOS. This application will be signed using a developer’s own DID
- Once the .epk (elastos package) file is created using toolchain scripts, it’s ready to be deployed. The next step is to use the tools provided in order to register this .epk file (a elastOS dapp) on DApp sidechain. The app package itself can be stored on a decentralized storage such as Elastos Hive
- Once the elastos app is registered on the DApp sidechain, the DApp Center inside elastOS Browser will automatically display the registered application showing all the details of the app including the developer’s DID who developed the application
- Users are then free to download this app and install it inside elastOS Browser and can run the application after that

elastOS tools are here to help during those steps, to make then as easy as possible.
