---
title: Ethereum Governance
description: An introduction to how decisions about Ethereum are made.
lang: en
---

# Introduction to Ethereum governance {#introduction}

_If no one owns Ethereum, how are decisions about changes to Ethereum made? Ethereum governance refers to the process that allows such decisions to be made._

<Divider />

## What is governance? {#what-is-governance}

Governance is the systems in place that allow decisions to be made. In a typical organizational structure, the executive team or a board of directors may have the final say in decision-making. Or perhaps shareholders vote on proposals to enact change. In a political system, elected officials may enact legislation that attempts to represent their constituents' desires.

## Decentralized governance {#decentralized-governance}

No one person owns or controls the Ethereum protocol, but decisions still need to be made about implementing changes to best ensure the longevity and prosperity of the network. This lack of ownership makes traditional governance systems incompatible with changes to Ethereum.

## Ethereum Governance {#ethereum-governance}

Ethereum governance is the process by which protocol changes are made. It's important to point out that this process isn't related to how people and applications use the protocol - Ethereum is permissionless to use. Anyone from anywhere in the world can participate in onchain activities. There are no rules set for who can or cannot build an application or send a transaction. However, there is a process to propose changes to the core protocol, which decentralized applications run on top of. Since so many people depend on Ethereum's stability, there is a very high coordination threshold for core changes, including social and technical processes, to ensure any changes to Ethereum are secure and widely supported by the community.

### Onchain vs offchain governance {#onchain-vs-offchain}

Blockchain technology allows for new governance capabilities, known as onchain governance. Onchain governance is when proposed protocol changes are decided by a stakeholder vote, usually by holders of a governance token, and voting happens on the blockchain. With some forms of onchain governance, the proposed protocol changes are implemented automatically via code if the stakeholders approve the changes by signing a transaction.

The opposite approach, offchain governance, is where any protocol change decisions happen through an informal process of social discussion which, if approved, are then implemented in code.

**Ethereum governance happens offchain** with a wide variety of stakeholders involved in the process.

_Whilst at the protocol level Ethereum governance is offchain, many use cases built on top of Ethereum, such as DAOs, use onchain governance._

<ButtonLink href="/dao/">
  More on DAOs
</ButtonLink>

<Divider />

## Who is involved? {#who-is-involved}

There are various stakeholders in the [Ethereum community](/community/), each playing a role in the governance process. Starting from the stakeholders furthest from the protocol and zooming in, we have:

- **Ether holders**: these people hold an arbitrary amount of ETH. [More on ETH](/eth/).
- **Application Users**: these people interact with applications on the Ethereum blockchain.
- **Application/Tooling Developers**: these people write applications that run on the Ethereum blockchain (e.g. DeFi, NFTs, etc.) or build tooling to interact with Ethereum (e.g. wallets, test suites, etc.). [More on dapps](/dapps/).
- **Node Operators**: these people run nodes that propagate blocks and transactions, rejecting any invalid transaction or block that they come across. [More on nodes](/developers/docs/nodes-and-clients/).
- **EIP Authors**: these people propose changes to the Ethereum protocol, in the form of Ethereum Improvement Proposals (EIPs). [More on EIPs](/eips/).
- **Validators**: these people run nodes that can add new blocks to the Ethereum blockchain.
- **Protocol Developers** (a.k.a. "Core Developers" ): these people maintain the various Ethereum implementations (e.g. Geth, Nethermind, Besu, Erigon, Reth at the execution layer or Prysm, Lighthouse, Nimbus, Teku, Lodestar, Grandine at the consensus layer). [More on Ethereum clients](/developers/docs/nodes-and-clients/).

_Note: any individual can be part of multiple of these groups (e.g. a protocol developer could champion an EIP, and run a beacon chain validator, and use DeFi applications). For conceptual clarity, it is easiest to distinguish between them._

<Divider />

## What is an EIP? {#what-is-an-eip}

One important process used in Ethereum governance is the proposal of **Ethereum Improvement Proposals (EIPs)**. EIPs are standards specifying potential new features or processes for Ethereum. Anyone within the Ethereum community can create an EIP. If you're interested in writing an EIP or participating in peer-review and/or governance, see:

<ButtonLink href="/eips/">
  More on EIPs
</ButtonLink>

<Divider />

## The formal process {#formal-process}

The formal process for introducing changes to the Ethereum protocol is as follows:

1. **Propose a Core EIP**: as described in [EIP-1](https://eips.ethereum.org/EIPS/eip-1#core-eips), the first step to formally proposing a change to Ethereum is to detail it in a Core EIP. This will act as the official specification for an EIP that Protocol Developers will implement if accepted.

2. **Present your EIP to Protocol Developers**: once you have a Core EIP for which you've gathered community input and implemented the [requisite tests](https://github.com/ethereum/execution-spec-tests), you should present it to Protocol Developers. You can do so by [proposing it](https://eips.ethereum.org/EIPS/eip-7723#proposed-for-inclusion) for discussion on an [AllCoreDevs call](https://github.com/ethereum/pm/issues?q=is%3Aissue%20state%3Aopen%20label%3AACD). It is expected that some discussion will have already happened asynchronously on the [Ethereum Magician's forum](https://ethereum-magicians.org/) or in the [Ethereum R&D Discord](https://discord.gg/mncqtgVSVw).

> Potential outcomes of this stage are:

> - The EIP will be considered for a future network upgrade ("[CFI](https://eips.ethereum.org/EIPS/eip-7723#considered-for-inclusion)")
> - Technical changes will be requested
> - It may be rejected if it is not a priority or the improvement is not large enough relative to the development effort ("[DFI](https://eips.ethereum.org/EIPS/eip-7723#declined-for-inclusion)")

3. **Iterate towards a final proposal:** after receiving feedback from all relevant stakeholders, you will likely need to make changes to your initial proposal to improve its security or better meet the needs of various users. Once your EIP has incorporated all the changes you believe are necessary, you will need to present it again to Protocol Developers. You will then move to the next step of this process, or new concerns will emerge, requiring another round of iterations. It also may be appropriate to schedule [breakout calls](https://github.com/ethereum/pm/issues?q=(label%3ABreakout%20label%3AConsensus)%20OR%20(label%3ABreakout%20label%3AExecution)%20) to iterate on the proposal.

4. **EIP Included in Network Upgrade**: assuming the EIP is approved, tested and implemented, it gets scheduled as part of a network upgrade. Given the high coordination costs of network upgrades (everyone needs to upgrade simultaneously), EIPs are generally bundled together in upgrades.

5. **Network Upgrade Activated**: after the network upgrade is activated, the EIP will be live on the Ethereum network.

This flow, while very simplified, gives an overview of the significant stages for a protocol change to be activated on Ethereum. Now, let's look at the informal factors at play during this process.

## The informal process {#informal-process}

### Understanding prior work {#prior-work}

EIP Champions should familiarise themselves with prior work and proposals before creating an EIP which can be seriously considered for deployment on the Ethereum Mainnet. This way, the EIP hopefully brings something new which hasn't been rejected before. The three main places to research this are [Ethereum Magicians](https://ethereum-magicians.org/), [ethresear.ch](https://ethresear.ch/), and the [EIP repository](https://github.com/ethereum/EIPs).

- ***Ethereum Magicians** is appropriate for most EIP discussions, e.g. pragmatic EIPs that improve the experience of developers or wallets, etc.*
- ***ethresear.ch** is for highly-technical, academic research, e.g. cryptographic advancements, scalability, security, and formal economic or game-theoretic analysis.*
- _The **EIP repo** is where proposals are formally drafted and submitted after sufficient discussion has taken place on Ethereum Magicians or ethresear.ch_

### Working groups {#working-groups}

The initial draft of an EIP is unlikely to be implemented on the Ethereum Mainnet without edits or changes. Generally, EIP Champions will work with a subset of Protocol Developers to specify, implement, test, iterate, and finalize their proposal. Historically, these working groups have required several months (and sometimes years!) of work. Similarly, EIP Champions for such changes should involve relevant Application/Tooling Developers early in their efforts to gather end-user feedback and mitigate any deployment risks.

### Community consensus {#community-consensus}

While some EIPs are straightforward technical improvements with minimal nuance, some are more complex and come with tradeoffs which will affect different stakeholders in different ways. This means some EIPs are more contentious within the community than others.

There is no clear playbook on how to handle contentious proposals. This is a result of Ethereum's decentralized design whereby no single stakeholder group can coerce the other through brute force: protocol developers can choose not to implement code changes; node operators can choose not to run the latest Ethereum client; application teams and users can choose not to transact on the chain. Since Protocol Developers have no way to force people to adopt network upgrades, they will generally avoid implementing EIPs where the contentiousness outweighs the benefits to the broader community.

EIP Champions are expected to solicit feedback from all relevant stakeholders. If you find yourself the champion of a contentious EIP, you should try and address objections to build consensus around your EIP. Given the size and diversity of the Ethereum community, there isn't a single metric (e.g. a coin vote) that can be used to gauge community consensus, and EIP Champions are expected to adapt to the circumstances of their proposal.

Beyond the security of the Ethereum network, significant weight has historically been placed by Protocol Developers on what Application/Tooling Developers and Application Users value, given that their using and developing on Ethereum is what makes the ecosystem attractive for other stakeholders. Additionally, EIPs need to be implemented across all client implementations, which are managed by distinct teams. Part of this process usually means convincing multiple teams of Protocol Developers that a particular change is valuable and that it helps end-users or solves a security issue.

<Divider />

## Handling disagreements {#disagreements}

Having many stakeholders with different motivations and beliefs means that disagreements are not uncommon.

Generally, disagreements are handled with long-form discussion in public forums to understand the root of the problem and allow anyone to weigh in. Typically, one group concedes, or a happy medium is achieved. If one group feels strongly enough, forcing through a particular change could result in a chain split. A chain split is when some stakeholders protest implementing a protocol change resulting in different, incompatible versions of the protocol operating, from which two distinct blockchains emerge.

### The DAO fork {#dao-fork}

Forks are when major technical upgrades or changes need to be made to the network and change the "rules" of the protocol. [Ethereum clients](/developers/docs/nodes-and-clients/) must update their software to implement the new fork rules.

The DAO fork was in response to the [2016 DAO attack](https://www.coindesk.com/understanding-dao-hack-journalists) where an insecure [DAO](/glossary/#dao) contract was drained of over 3.6 million ETH in a hack. The fork moved the funds from the faulty contract to a new contract allowing anyone who lost funds in the hack to recover them.

This course of action was voted on by the Ethereum community. Any ETH holder was able to vote via a transaction on [a voting platform](https://web.archive.org/web/20170620030820/http://v1.carbonvote.com/). The decision to fork reached over 85% of the votes.

It's important to note that whilst the protocol did fork to revert the hack, the weight the vote carried in deciding to fork is debatable for a few reasons:

- The turnout to vote was incredibly low
- Most people didn't know the vote was happening
- The vote only represented ETH holders, not any of the other participants in the system

A subset of the community refused to fork, largely because they felt the DAO incident wasn't a defect in the protocol. They went on to form [Ethereum Classic](https://ethereumclassic.org/).

Today, the Ethereum community has adopted a policy of non-intervention in cases of contract bugs or lost funds to maintain the credible neutrality of the system.

Watch more on the DAO hack:

<YouTube id="rNeLuBOVe8A" />

<Divider />

### The utility of forking {#forking-utility}

The Ethereum/Ethereum Classic fork is an excellent example of a healthy fork. We had two groups who disagreed strongly enough with each other on some core values to feel it was worth the risks involved to pursue their specific courses of action.

The ability to fork in the face of significant political, philosophical or economic differences plays a large part in the success of Ethereum governance. Without the ability to fork the alternative was ongoing in-fighting, forced reluctant participation for those who eventually formed Ethereum Classic and an increasingly differing vision of how success for Ethereum looks.

<Divider />

## Beacon Chain governance {#beacon-chain}

The Ethereum governance process often trades off speed and efficiency for openness and inclusivity. In order to accelerate the transition from proof-of-work to proof-of-stake, the Beacon Chain (now known as the Consensus Layer) was launched separately from the proof-of-work Ethereum network and followed its own governance practices.

While the specification and development implementations have always been fully open source, the formal processes described above weren't initially used in Beacon Chain development. This allowed changes to be specified and agreed upon quicker by researchers and implementers.

When the Beacon Chain merged with the Ethereum execution layer on September 15th 2022, *the Merge* was completed as part of the [Paris network upgrade](/history/#paris). The proposal [EIP-3675](https://eips.ethereum.org/EIPS/eip-3675) was changed from 'Last Call' to 'Final', completing the transition to proof-of-stake.

<ButtonLink href="/roadmap/merge/">
  More on The Merge
</ButtonLink>

<Divider />

## How can I get involved? {#get-involved}

- [Propose an EIP](/eips/#participate)
- Discuss [current proposals](https://ethereum-magicians.org/)
- Get involved in [R&D discussion](https://ethresear.ch/)
- Join the [Ethereum R&D discord](https://discord.gg/mncqtgVSVw)
- [Run a node](/developers/docs/nodes-and-clients/run-a-node/)
- Contribute to [client development](/developers/docs/nodes-and-clients/#execution-clients)
- Apply to the [Ethereum Protocol Fellowship](https://epf.wiki/#/)

## Further reading {#further-reading}

Governance in Ethereum isn’t rigidly defined. Various community participants have diverse perspectives on it. Here are a few of them:

- [Rough Consensus: An Informal Guide to Participation](https://mirror.xyz/nixo.eth/hT5F3Eo4iqQYNtoZCNqobogAr_Kd2QOmzqEtoizG5GA) - _Nixo, 2025_
- [The Ethereum Government](https://www.galaxy.com/insights/research/ethereum-governance/) - _Christine Kim, 2024_
- [Understanding Blockchain Governance](https://research.2077.xyz/understanding-blockchain-governance) - _2077 Research, 2024_
- [Moving beyond coin voting governance](https://vitalik.eth.limo/general/2021/08/16/voting3.html) - _Vitalik Buterin, 2021_
- [How Ethereum governance works](https://medium.com/coinmonks/how-ethereum-governance-works-71856426b63a) – _Micah Zoltu, 2021_
- [How does Ethereum Governance work?](https://cryptotesters.com/blog/ethereum-governance) – _Cryptotesters, 2021_
- [What is an Ethereum core developer?](https://hudsonjameson.com/2020-06-22-what-is-an-ethereum-core-developer/) - _Hudson Jameson, 2020_
- [Governance, Part 2: Plutocracy Is Still Bad](https://vitalik.eth.limo/general/2018/03/28/plutocracy.html) - _Vitalik Buterin, 2018_
- [Notes on Blockchain Governance](https://vitalik.eth.limo/general/2017/12/17/voting.html) - _Vitalik Buterin, 2017_
