# RescYou
Resc-You is a chat app for recovering addicts that helps to solve the problem of isolation and lack of support that many people in recovery face. It provides a safe and supportive space for users to connect with each other, share their experiences, and offer support and encouragement to each other.

With Resc-You, users can:

--> Connect with other recovering addicts from around the world and build a supportive network of peers
--> Share their experiences and offer support and guidance to others in recovery
--> Find resources and information on topics related to addiction and recovery
--> Connect with trained professionals or sponsors for more specialized support and guidance
--> Participate in recovery-focused groups and discussions
--> Find support and connection when they need it most

Overall, Resc-You makes it easier and safer for recovering addicts to connect with each other and find the support they need to stay sober. It provides a valuable resource for people in recovery, helping them to feel less alone and more connected to a supportive community.

Challenges I ran into
One of the challenges that I faced while building this project was time constraints. With limited time available, it was difficult to fully explore all of the features and functionality that I wanted to include in the chat app. I had to prioritize certain tasks and focus on the most essential features, which meant that some aspects of the app may not be as fully developed as I would have liked.

To overcome this challenge, I had to be strategic in my time management and stay organized to make the most of the time I had available. I also had to be willing to make compromises and be flexible in my approach, so that I could still deliver a functional and useful app within the constraints of the time frame.

Overall, time constraints can be a significant challenge when building any project, but by being strategic and flexible, it is possible to overcome them and deliver a successful product.


## Getting Started

You can clone this repository by running the following command:

```
git clone https://github.com/arncv/RescYou.git
```

Copy the `.env.sample` file and rename the copy to `.env`

Then update the newly renamed `.env` file with your Hedera Testnet account info as indicated. For example:

```
ACCOUNT_ID=0.0.123456789
PRIVATE_KEY=302e020100300506032b657004220420f4361ec73dc43e568f1620a7b7ecb7330790b8a1c7620f1ce353aa1de4f0eaa6
TOPIC_ID=0.0.28583
```
The `TOPIC_ID` is used when connecting to an existing topic. If you don't have one, you can leave it as is.

After downloading and setting up our environment, we'll install our packages via [npm](https://docs.npmjs.com/about-npm/).

```
npm install
```

If installing the dependencies was succesful, now try to run the server!

```
node server.js
```

After running your server, it will prompt you to configure your chat, e.g.

```
1. What mode do you want to run in?  <--- "Default", "Minimal", "Debug"
2. What's your account ID?           <---  defaults to the .env schema
3. What's your private key?          <---  defaults to the .env schema
4. Should we create a new HCS topic, or connect to an existing one?
```

If everything was configured properly, the chat should now open at a random port location.

You can additionally run another instance of the chat application by creating a new terminal, and running the application again. This will find another unused, random port location, and deploy multiple instances to your local machine. With the environment configurability, you can test out multi-client chats.
