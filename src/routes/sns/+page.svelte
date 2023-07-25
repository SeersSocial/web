<script>
    import { Accordion, AccordionItem } from "flowbite-svelte";
</script>

<svelte:head>
	<title>SNS</title>
	<meta name="description" content="SNS" />
</svelte:head>

<section class="w-full flex flex-col mt-14 text-lg justify-center justify-items-center content-center items-center">
	<div class="flex flex-col md:w-2/3 gap-4">
		<div>
		    <h3 class="font-bold">SNS Whitepaper</h3>
        </div>

        <Accordion activeClasses="" inactiveClasses="" defaultClass="">
            <AccordionItem>
                <span slot="header">1 - Product Overview</span>
                <div  class="space-y-4">
                    <h3 class="text-sky-600">Introduction</h3>
                    <p>Seers is a Web3 decentralized, fully on-chain social network built atop the groundbreaking technology of the Internet Computer. Drawing inspiration from Twitter's intuitive design, Seers improves user interaction with exclusive crypto features like prediction markets. This platform allows you to voice your thoughts and use cryptocurrencies to predict future events. But this is merely the beginning. We envision Seers evolving into a vibrant platform akin to Elon Musk's 'X', with the potential to redefine global interactions and transactions.</p>
                    <h3 class="text-sky-600">Prediction Markets</h3>
                    <p>
                        Prediction markets are financial markets where users can buy and sell shares based on the outcome of future events. By aggregating information and opinions from a large number of people, prediction markets provide more accurate predictions of event likelihoods.
                        For example, football fans can use ICP tokens as collateral to trade shares for the UEFA Champions League final between Real Madrid and Bayern Munich. Shares include "Real Madrid Wins," "Bayern Munich Wins," and "Match Ends in Draw." Users can stake ICP tokens to buy and sell these shares based on their predictions. Share prices fluctuate based on user activity and sentiment. After the final, winning shares can be exchanged back for ICP tokens, while unsuccessful shares result in the loss of the staked ICP collateral. In this way, Seers offers an interactive way for football enthusiasts to leverage ICP and participate in the excitement of the championship match.
                    </p>
                    <h3 class="text-sky-600">Seers' Accomplishments and Decentralised Future</h3>
                    <ul>
                        <li>Over the past year, Seers conducted extensive product-market fit experiments, featuring 200 prediction markets and engaging 3,000 users. Additionally, our community has created over 10,000 posts, reflecting active participation.</li>
                        <li>These efforts have resulted in a remarkable Total Value Locked (TVL) of $15,000 in ICP and an estimated yearly revenue of $25,000.</li>
                        <li>Importantly, we have recently distributed part of the revenue to our users according to their contributions over the previous month, with some members earning up to $100 per week.</li>
                    </ul>
                    <p>
                        While we consider these figures modest, we firmly believe that we will experience exponential growth as we continue to develop our roadmap and tap into the full potential of the Internet Computer's capabilities.
                        Decentralization is crucial to ramp up liquidity and deploy more powerful features, as outlined in the next section, which allows us to foster a truly user-driven and resilient ecosystem.
                        We instill confidence in our ability to vastly enhance the adoption of the Internet Computer and blockchain technologies, empowering users with greater ownership and control over their data.
                    </p>
                    <h3 class="text-sky-600">Features</h3>
                    <p>
                        Seers currently combines the main features of Twitter with the innovation of prediction markets. Looking ahead, we have ambitious plans to elevate our UI/UX and prediction markets to new heights, while also introducing a plethora of other exciting features and cutting-edge crypto primitives.
                        Some key features and planned developments of Seers include:
                    </p>
                    <ol>
                        <li>- Decentralised platform built on the Internet Computer.</li>
                        <li>- Intuitive UI/UX similar to Twitter, where user can create posts and prediction markets.</li>
                        <li>- Decentralised oracles for sport events.</li>
                        <li>- ckBTC staking, targeting an APY of up to 10%.</li>
                        <li>- Encrypted messages and posts using vetKeys.</li>
                        <li>- Communities with push button DAO, token creation and other features.</li>
                        <li>- Images drive with a view reminiscent of Instagram.</li>
                        <li>- We envision an internal NFT marketplace that is seamlessly connected with other marketplaces and the rest of the platform.</li>
                        <li>- Programable and decentralised AI.</li>
                        <li>- Integration with other social networks like Twitter, social graphs and protocols like ActivityPub (Mastodon, Threads). </li>
                        <li>- Our goals include up to the creation of a stable coin (we already started researching possible designs), used in combination with our social graph to develop an array of innovative features.</li>
                    </ol>
                    <h3 class="text-sky-600">Team</h3>
                    <p>Our team comprises a diverse and talented group of individuals with extensive experience in the web3 space, spanning across Europe and South America. Together, we bring a wealth of expertise in blockchain technology and decentralized applications. Our founder, ex Rust core developer for Polkadot and PhD, possesses deep insights into the inner workings of the blockchain ecosystem. Moreover, the team includes former Google employees who have contributed to large-scale projects, as well as individuals who have excelled in programming olympiads, showcasing their strong mathematical foundations. With their combined skills and knowledge, the Seers team is well-positioned to spearhead the revolution of social networking and prediction markets on a global scale.</p>
                </div>
            </AccordionItem>
            <AccordionItem>
                <span slot="header">2 - Seers DAO</span>
                <div  class="space-y-4">
                    <h3 class="text-sky-600">Summary</h3>
                    <ul>
                        <li>- The Seers DAO will be established to govern and guide the direction of the Seers platform, serving as a decentralized autonomous organization owned by the community.</li>
                        <li>- Both the Seers DAO and the Seers services will be fully integrated on the blockchain, eliminating the need for reliance on off-chain services.</li>
                        <li>- Seers will operate using NNS-blessed SNS canisters and the SNS subnet, ensuring a secure and scalable infrastructure.</li>
                        <li>- A proposal will be submitted to the NNS (Internet Computer's Network Nervous System) to seek approval for the creation of the Seers DAO and its associated public good, solidifying its legitimacy and community-driven nature.</li>
                    </ul>
                </div>
            </AccordionItem>
            <AccordionItem>
                <span slot="header">3 - SEER Token Utility</span>
                <div  class="space-y-4">
                    The SEER token offers an array of exciting use cases within the Seers ecosystem:
                    <ul>
                        <li><span class="text-sky-500">Governance and Voting:</span> SEER tokens can be staked as neurons, akin to ICP neurons, allowing token holders to actively participate in the governance of Seers by voting on proposals. By doing so, they earn voting rewards that increase over time, fostering long-term engagement and alignment with the platform's objectives.</li>
                        <li><span class="text-sky-500">Promotion of posts and markets:</span> Users can utilize SEER tokens to promote posts and prediction markets within the Seers ecosystem, increasing their visibility and reach among the community.</li>
                        <li><span  class="text-sky-500">Promotion of profiles:</span> SEER tokens can be used to secure featured placement on the Seers platform, highlighting specific profile, thus enhancing their exposure and attracting more followers.</li>
                        <li><span  class="text-sky-500">Content Moderation and Rewards:</span> Content moderators on Seers play a crucial role in maintaining the quality and integrity of the platform's content. To participate in content moderation, moderators are required to lock a specific amount of SEER tokens. This token commitment demonstrates their dedication to ensuring a safe and engaging environment for users. Through an automated reward mechanism, content moderators receive fair compensation based on their reputation scores. This incentivizes active participation, promotes the growth of a vibrant content ecosystem, and ensures the continuous improvement and quality of the content available on Seers.</li>
                        <li><span  class="text-sky-500">Access to Premium AI Services:</span>SEER tokens provide users with exclusive access to premium AI services within the Seers ecosystem. By leveraging their tokens, users can tap into the capabilities of state-of-the-art generative AI models, unlocking advanced functionalities for tasks such as content generation, creative design, and data synthesis. This integration of generative AI empowers users to explore new horizons of creativity, enabling them to generate unique and engaging content, collaborate with AI-powered tools, and unlock innovative possibilities within the Seers platform. The availability of these premium generative AI services adds an extra layer of value and creativity to the Seers experience, enhancing user engagement and pushing the boundaries of what's possible.</li>
                        <li><span  class="text-sky-500">Storage Payments:</span>SEER tokens can be used for payments related to storage services, such as on the Seers Drive, ensuring secure and efficient data storage within the platform.</li>
                        <li><span  class="text-sky-500">NFT Transactions on Seers Marketplace:</span> Within the Seers marketplace, users can buy and sell NFTs using SEER tokens. This facilitates seamless and secure transactions, fostering a vibrant marketplace for digital collectibles and unique assets.</li>
                    </ul>
                    These utility cases demonstrate the versatile and valuable nature of SEER tokens within the Seers ecosystem, encouraging active participation, rewarding contributions, and fueling the growth of the platform.
                </div>
            </AccordionItem>
          </Accordion>
    </div>
</section>