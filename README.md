#Metaverse

##Goal
The goal of the Etheric Metaverse project is to create a 3D MMO layer of the WWW.  Some URLs that users navigate to will allow users to enter 3D worlds where they can bring their avatars and virtual property, which can be traded.  Smart-Contracts can also be signed to change the rules of the game.

##How

###The Basic Idea
The Ethereum blockchain keeps track of ownership of property.  We associate a whisper (Ethereum Whisper) channel with each website domain name (sub-channels will need to be designed as well), which is where the users present at a website can meet each other.  The users use the whisper channel to form a p2p network for higher bandwidth communication.  Whisper is private but has very low bandwidth, so we will only use it as a signaling service for the p2p networks and for private communications between users.  Users can also communicate with the server.  Any assets that need to be available to all users, such as the assets associated with user (as opposed to server) property, will be stored in decentralized storage such as swarm.

###Adding VR
Each server can host a 3D realm and enforce how the users can navigate through it (for instance, no teleporting).

To keep data at a minimum, a standard language similar to HTML may be needed for specifying rooms and layouts of objects.  We can then style the 3D scene with an extension of CSS and modify the 3D version of the DOM with javascript or webasm.  We should be as friendly as possible with previous work in this direction.

To ensure that the servers cannot censor users' property, the VR client should be standard across all websites.

###Why the blockchain?
The blockchain ensures that all users can see each others' property.  This way a server cannot decide which property to honor or revoke.

###Why the p2p network for users?
The p2p network ensures that some data can always be communicated between users of a website without the interference of the server.  As a simple example, this would be used for users to chat and to announce their locations in the realm so that the server cannot completely censor them.

##How to Prevent Heinous Avatars in Kid Friendly Spaces
Each website can, if it wishes, have complete control over all assets displayed in the VR client.  While many websites would benefit from allowing user-defined assets, this is completely option.

##MVP
The MVP will not need any graphics.  At the least, it would allow the creation of a whisper channel and p2p network for any website.  Thus, the MVP will enable meeting other people through browsing the web.

#Astral Cat
Astral Cat will be low level portion of the Metaverse suite that joins a website's whisper channel and p2p network, enabling meeting other people.

#EthericVR
EthericVR will be the VR client and anything else needed to get the VR world working

---

(1) https://github.com/ethereum/wiki/wiki/Whisper
