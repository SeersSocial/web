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
		    <h3 class="font-bold">SNS Information</h3>
        </div>

        <Accordion activeClasses="" inactiveClasses="" defaultClass="">
            <AccordionItem>
                <span slot="header">1 - Product Overview</span>
                <div  class="space-y-4">
                    <p>Seers is a Web3 decentralized, fully on-chain social network built atop the groundbreaking technology of the Internet Computer. Drawing inspiration from Twitter's intuitive design, Seers improves user interaction with exclusive crypto features like prediction markets. This platform allows you to voice your thoughts and use cryptocurrencies to predict future events. But this is merely the beginning. We envision Seers evolving into a vibrant platform akin to Elon Musk's 'X', with the potential to redefine global interactions and transactions.</p>
                </div>
            </AccordionItem>
            <!-- <AccordionItem>
              <span slot="header">
                2 - Internet Computer Overview</span>
                <div class="space-y-4">
                    <p>
                        The Internet Computer  (IC) is a decentralized global compute platform which uses ground-breaking blockchain technology to achieve consensus within subnets. It is globally distributed in numerous independent data centers, is tamper proof and unstoppable.
                    </p>
                    <p>
                        It can serve applications fully on-chain without needing any centralized frontend layer. It is extremely efficient and is several orders of magnitude cheaper to run and store data than most other blockchains. It uses a reverse-gas model so computation and storage costs are paid by the app/service providers rather than users.
                    </p>
                    <p> 
                        Canister smart-contracts
                        Applications on the IC are composed of canister smart-contracts organized into subnets. A subnet can contain 100,000s of canisters and is composed of (typically 13) node machines each of which runs in a different independent data center around the globe such that the nodes within each subnet are as geographically and jurisdictionally diverse as possible. Canisters can communicate securely with canisters on other subnets allowing the IC to scale horizontally.
                    </p>
                    <p> 
                        A canister runs on a virtual machine (as a WASM) that is replicated across a subnet. It implements the actor model, and so is single threaded, processing a queue of input messages one at a time, optionally sending messages to other canisters, and adding a response message to an output queue.
                    </p>
                    <p> 
                        It can be called by clients (or other canisters) using queries or updates. A query can be served immediately from any node but cannot change state. An update can change state and goes through a process of consensus for the nodes to agree on the same result before responding to the caller. Achieving consensus is where the blockchain comes into play but is beyond the scope of this document.
                    </p>
                    <p> 
                        Canisters have the property of orthogonal persistence  which means as a programmer you just write data objects to memory and they are automatically persisted by the system. This removes the need for a database and is one of the reasons writing and running applications on the IC is simplified compared to traditional IT stacks.
                    </p>
                    <p> 
                        Network Nervous System (NNS)
                        A key feature of the Internet Computer blockchain is the Network Nervous System (NNS), an open algorithmic governance system that oversees the network and the token economics.
                    </p>
                    <p> 
                        Holders of the Internet Computer’s ICP utility tokens can lock their tokens in neurons to participate in governance and contribute to decision-making, such as voting to determine whether or not a new subnet should be added to the network. By participating in governance, voters earn rewards which can be converted to ICP. In turn they can burn ICP to fuel the computation of their canisters.
                    </p>
                    <p>   
                        Read here for more information on the NNS.
                    </p>
                </div>
            </AccordionItem>
            <AccordionItem>
                <span slot="header">
                  3 - Seers DAO</span>
                  <div class="space-y-4">
                      <p>
                        The Seers DAO is being formed to operate and steer the direction of Seers and can be considered a public good, owned by no-one.
                        The Seers DAO and the Seers service are fully on-chain with no direct dependencies on off-chain services.
                        The Seers DAO is operated using NNS blessed SNS canisters and SNS subnet.
                        A proposal to the NNS will be made to ask for the approval necessary to create this DAO and associated public good.
                    </p>
                </div> 
            </AccordionItem> 
            <AccordionItem>
                <span slot="header">
                  4 - Purpose of the SEER utility token</span>
                  <div class="space-y-4">
                      <p>
                        It can be staked as neurons (very similar to ICP neurons) allowing token holders to participate in the governance of Seers by voting on SNS proposals, and by doing so, earn voting rewards. 
                        These rewards increase the longer the tokens are staked and so token holders are incentivised to act in the long term interests of Seers.
                        It can be used by Seers users to pay for premium features.
                        It can be used to reward contributions to the evolution or growth of the Seers service either through automated user rewards or by SNS proposal.   
                    </p>
                </div> 
            </AccordionItem> 
            <AccordionItem>
                <span slot="header">
                    5 - Token allocation at SNS genesis</span>
                  <div class="space-y-4">
                      <p>
                        TODO    
                    </p>
                </div> 
            </AccordionItem> 
            <AccordionItem>
                <span slot="header">
                    6 - Seers SNS treasury</span>
                  <div class="space-y-4">
                      <p>
                        TODO    
                    </p>
                </div> 
            </AccordionItem> 
            <AccordionItem>
                <span slot="header">
                    7 - Tokenomics</span>
                  <div class="space-y-4">
                      <p>
                        TODO
                    </p>
                </div> 
            </AccordionItem> 
             -->
            
          </Accordion>
    </div>
</section>