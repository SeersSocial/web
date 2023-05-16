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
                <span slot="header">1 - Product / Service Overview</span>
                <div  class="space-y-4">
                <p>Seers is a fully featured social network application running on the Internet Computer
                    blockchain similar to Twitter.
                </p>
                <p>
                    It is a responsive, progressive web application (PWA) and as such scales to take
                    advantage of any screen size and integrates with devices in a similar way to native
                    apps, with notifications on desktop and Android devices, and on iOS from next year. You can find the full development roadmap here.
                </p>
                <p> 
                    The app is open source and runs as a collection of canister smart-contracts. It is possible to see the
                    code running on any canister at any time with a link back to the particular version
                    in source control and to independently verify this is true.
                </p>
                    
                <p>A canister is created for each user which holds their direct chat data, links to the
                    groups they are members of, and also serves as a wallet allowing Seers users to
                    hold and manage tokens. Each community is also implemented as its
                    own canister. This architecture will allow Seers to scale to every person on the
                    planet. For details of the architecture please see here. 
                    
                </p>
                <p>
                    Seers users can send messages to each other containing tokens such as ICP and
                    ckBTC and so can be used for global remittance. 
                </p>
                <p>
                    However, the ground-breaking difference between Seers and other similar apps, is
                    that it will soon be governed as a DAO with its own token called SEER, analogous to
                    ICP. The DAO will be realized by a system called the SNS
                    (Service Nervous System) analogous to the NNS (Network Nervous System) on the Internet Computer. 
                </p> 
                <p>The focus of the founding dev team has been first and foremost on building a rich,
                    fully featured chat app on par with its web2 counterparts. Only by first building an
                    app that people are happy to use will the rocket fuel of tokenization enable
                    Seers to grow and challenge monopolistic big tech incumbents.
                </p>
                </div>
            </AccordionItem>
            <AccordionItem>
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
                        TODO    
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
            
            
          </Accordion>
    </div>
</section>