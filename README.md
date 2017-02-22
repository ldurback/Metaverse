#Goal
The goal of the Etheric Metaverse project is to create a 3D MMO layer of the world wide web.  Some URLs that users navigate to will allow users to enter 3D worlds where they can bring their avatars and virtual property, which can be traded.  Smart-Contracts can also be signed to change the rules of the game.

---

#Astrum
Astrum will be the low level portion of the Metaverse suite that allows forming and joining a URL's realm and meeting other people.

#EthericVR
EthericVR will be the VR web browser and any client side programming languages the web browser can interpret.

---

#How and What

##Astrum
The Ethereum blockchain keeps track of ownership of property.  We associate a whisper (1) channel with each URL, which is where the users present at a URL can meet each other.  The users use the whisper channel to form a p2p network for higher bandwidth communication.  Whisper is private but has very low bandwidth, so we will only use it as a signaling service for the p2p networks and for private communications between users.  Users can also communicate with the website's server.  Any assets that need to be available to all users, such as the assets associated with user (as opposed to server) property, will be stored in decentralized storage such as swarm.

##EthericVR
Each server can host a 3D realm and enforce how the users can navigate through it (for instance, no teleporting).

To keep data at a minimum, a standard language similar to HTML may be needed for specifying rooms and layouts of objects.  We can then style the 3D scene with an extension of CSS and modify the 3D version of the DOM with javascript or webasm.  We should be as friendly as possible with previous work in this direction.

---

##Why the blockchain?
The blockchain ensures that all users can see each others' property and the users themselves are in control of their property.  This way a server cannot decide which property to honor or revoke.

##Why the whisper channel and p2p network associated with each website?
The p2p communication channels ensure that data can always be communicated between users of a website without the interference of the server.  As a simple example, this could be used for users to chat and to announce their locations in the realm.

##Filtered Mode
Some of the data flowing through p2p communications will be unsafe for viewing by the user.  Additionally, the designers of the website may want to stylize data that flows through the p2p network.  To achieve this, a website only needs to listen to the public p2p messages and then broadcast officiated revisions of the messages.  This mode can be toggled on the client side.

---

(1) https://github.com/ethereum/wiki/wiki/Whisper
