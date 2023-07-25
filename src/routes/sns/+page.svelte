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
                <span slot="header">Product Overview</span>
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
                <span slot="header">Seers DAO</span>
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
                <span slot="header">SEER Token Utility</span>
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
            <AccordionItem>
                <span slot="header">Token allocation at SNS genesis</span>
                <div  class="space-y-4">
                    The SNS will be initialized with 100 million SEER tokens allocated in the following proportions.
                    <img alt="" class="w-300 my-2" src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fdf1d2afe-e21c-41dc-bac3-0f0fcc6ef3a9%2FScreenshot_2023-07-23_at_18.43.20.png?table=block&id=4e61041d-1358-4652-88d5-a0ac17c1d3fe&spaceId=99cf4b46-040e-4088-b8a9-635bbdc239a0&width=2000&userId=35d25b55-082d-4e6c-83cf-28ce5dc9dd4f&cache=v2"/>    
                    <h3 class="text-sky-600">Decentralization Sale</h3>

                    <p>To decentralize governance and raise funds for the Seers SNS, a total of 25% of the token supply will be made available for sale. The maximum amount that can be raised through this sale will be set at 1,000,000 ICP, while the minimum will be 500,000 ICP.</p>

                    <p>We are seeking a contribution of 333,333 ICP from the Neuron Fund (NF), with the remaining 666,667 ICP to be raised from participants in the decentralization sale.</p>

                    <p>During the sale, participants will deposit ICP into the SNS. Once the sale concludes, they will receive SEER tokens in proportion to their share of the deposited ICP. Each participant will receive their SEER tokens in the form of a basket containing 5 neurons of equal value. The first neuron will have no dissolve delay, allowing for immediate disbursement of liquid SEER tokens. The remaining neurons will have dissolve delays of 3, 6, 9, and 12 months, respectively.</p>

                    <p>Participants from the Neuron Fund will also receive their share of tokens as a basket of 5 neurons, following the same configuration as described above.</p>
                
                    <h3 class="text-sky-600">Founders and Funders</h3>

                    <p>The Seers team has been diligently developing and running Seers since July 2022. Following the SNS sale of SEER tokens, the Seers Foundation will be established. The foundation will receive 15% (15,000,000) of the SEER tokens, distributed across 5 equal neurons. Each of these neurons will have a dissolve delay of 1 month, with "vesting periods" set at 0, 1, 2, 3, and 4 years, respectively.</p>

                    <p>Seed funders, on the other hand, will receive 8% of the SEER tokens as a basket of 5 equal neurons. Each neuron will have a dissolve delay of 1 month and "vesting periods" of 0, 6, 12, 18, and 24 months, respectively.</p>

                    <p>It is important to note that neurons with a "vesting period" cannot be accessed until the specified period has elapsed, including any potential extension of the dissolve delay. This mechanism ensures that founders and funders are prevented from rug-pulling investors and provides a continuous incentive to drive the success of Seers.</p>

                    <p>Since these founder/funder neurons have relatively short dissolve delays of 1 month that cannot be extended, it ensures reduced voting power compared to the community. This intentional design ensures proper decentralization of governance, empowering the community to have a significant say in shaping the future of Seers.</p>
                    <img alt="" class="w-300 my-2" src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F255aec2c-c158-4045-8e99-c6438f67245f%2FScreenshot_2023-07-23_at_18.43.44.png?table=block&id=910ab51c-abd7-4c0c-aa2d-bed62b1a973c&spaceId=99cf4b46-040e-4088-b8a9-635bbdc239a0&width=2000&userId=35d25b55-082d-4e6c-83cf-28ce5dc9dd4f&cache=v2"/>    
                    
                    <h3 class="text-sky-600">SNS Treasury</h3>

                    <p>Following the decentralization sale, the SNS will retain a treasury consisting of the remaining 52% of SEER tokens. This treasury will serve various purposes to support the growth and development of Seers.</p>

                    <p>The majority of the tokens will be utilized over time to automatically reward content moderators, fostering a thriving content ecosystem and facilitating the expansion of Seers. Additionally, the treasury will be available to fund community bounties through SNS proposals, compensating individuals who contribute to Seers in various ways. This includes rewarding third-party developers for their valuable code contributions.</p>

                    <p>A small portion, approximately 2%, will be allocated to provide initial liquidity pools for decentralized exchanges (DEXes). To enable the trading of SEER tokens, it is essential to list SEER on one or more exchanges. The intention is to list SEER on IC-based DEXes. Listing SEER on a DEX that implements an Automated Market Maker (AMM) requires the provision of a liquidity pool consisting of SEER tokens and another token, in this case, ICP raised from the decentralization sale. The plan is to make SEER available on multiple DEXes as they become available. Each DEX listing will require a proposal to transfer a specific amount of SEER from the SNS to the DEX, along with a corresponding proposal to transfer an equal value of ICP from the SNS to the DEX.</p>

                    <p>The SNS treasury plays a crucial role in supporting the Seers ecosystem, rewarding contributors, promoting liquidity, and facilitating the growth and accessibility of the SEER token on decentralized exchanges.</p>
                
                    <h3 class="text-sky-600">Valuation Range</h3>

                    <p>The inclusion of a maximum target is intended to provide participants with a guaranteed minimum allocation of SEER tokens in exchange for their ICP investment. With a lower bound of 500,000 ICP and an upper bound of 1,000,000 ICP for 25% of the tokens, the Seers DAO achieves an initial valuation range between 2M ICP and 4M ICP. Consequently, the initial value of 1 SEER token would range from 0.02 ICP to 0.04 ICP. This valuation range ensures transparency and establishes a framework for participants to assess the potential value of their investment in the Seers ecosystem.</p>
                </div>
            </AccordionItem>
            <AccordionItem>
                <span slot="header">Roadmap</span>
                <div  class="space-y-4">
                    <h3 class="text-sky-600">Q3 2023</h3>

                    <p>Complete preparations for the SNS launch, perform post-launch tasks, and work towards reintroducing prediction markets in a decentralised manner. Focus on developing decentralised content moderation strategies and enhancing the user interface and user experience (UI/UX).</p>
                    <h3 class="text-sky-600">Q4 2023</h3>

                    <p>Roll out the decentralised sports oracle, offering support for prediction markets across all sports. Deploy the improved UI/UX, and integrate features such as private messaging and community creation.</p>

                    <h3 class="text-sky-600">Q1 2024</h3>

                    <p>Work on increasing the efficiency of liquidity in prediction markets and institute rewards for liquidity providers and content moderators. Continue the development of communities, AI bots, and entertaining games like poker. Initiate the development of native Android and iOS applications.</p>

                    <h3 class="text-sky-600">Q2 2024</h3>

                    <p>Facilitate token and DAO creation within communities and develop any additional features that these communities may require. Advance the development of peer-to-peer (p2p) prediction markets and NFT minting capabilities.</p>

                    <h3 class="text-sky-600">Q3 2024</h3>

                    <p>Finalise the implementation of peer-to-peer prediction markets, including the related contracts. Incorporate on-chain encryption and establish connections with other social networks like Twitter and Mastodon.</p>
                </div>
            </AccordionItem> 
            <AccordionItem>
                <span slot="header">Disclaimer</span>
                <div  class="space-y-4">
                        <p>The information presented in this white paper is subject to change or update, and should not be considered a commitment, promise, or guarantee by any individual or organization mentioned in the document regarding the future availability of services related to the use of tokens or their future performance or value. Approval from Seers SNS DAO members is required for the features or other aspects of the platform mentioned in the white paper</p>

                        <p>This document is for informational purposes only and does not constitute an offer or solicitation to sell any securities or shares. It should not be construed as an invitation to buy or subscribe for any securities, nor should it form the basis of any contract or commitment. Seers DAO assumes no responsibility for any loss or damage arising from reliance on the information contained in this document, including any errors or inaccuracies. Any actions taken based on the information in this document are taken at the reader's own risk.</p>

                        <p>This document is for informational purposes only and should not be construed as a recommendation to buy or financial advice. Investing or trading in any tokens, companies, or entities based solely on this information involves substantial risks, including but not limited to pricing volatility, inadequate liquidity, and the potential complete loss of principal. Investors are advised to conduct independent due diligence, seek assistance from professional financial, legal, and tax experts, and develop a standalone judgment of the relevant markets before making any investment decision. The information presented in this document does not create an attorney-client relationship and is not a substitute for legal advice from a qualified attorney.</p>

                        <p>This document is provided "as is" without warranty of any kind, whether expressed or implied. We have prepared all information herein based upon selected public market data, which we believe to be accurate and reliable, and our view as of this date. However, we do not warrant the completeness or accuracy of the information presented herein, and it is accordingly subject to change without notice. The graphs, charts, and other visual aids are for informational purposes only and cannot be used alone to make investment decisions. None of these visual aids can capture all factors and variables required in making such decisions. Therefore, no representation is made that these will assist any person in making investment decisions.</p>

                        <p>This document may contain forward-looking statements, including projections, forecasts, and estimates that are speculative in nature and based on certain assumptions. These statements are not guarantees of future performance and may be impacted by inaccurate assumptions or known or unknown risks, uncertainties, and other factors beyond the control of the parties involved. As a result, actual results may vary significantly from the forward-looking statements contained in this document. No representations or warranties are made as to the accuracy of the forward-looking statements.</p>
                </div>
            </AccordionItem>
          </Accordion>
    </div>
</section>