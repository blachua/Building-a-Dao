![image](https://user-images.githubusercontent.com/116645635/224873301-878e415d-7bcc-4e46-8e69-60248c67782e.png)

What is a DAO?
DAO stands for Decentralized Autonomous Organization. You can think of DAOs as analogous to companies in the real world. Essentially, DAOs allow for members to create and vote on governance decisions.

In traditional companies, when a decision needs to be made, the board of directors or executives of the company are in charge of making that decision. In a DAO, however, this process is democratized, and any member can create a proposal, and all other members can vote on it. Each proposal created has a deadline for voting, and after the deadline the decision is made in favour of the voting outcome (YES or NO).

Membership in DAOs is typically restricted either by ownership of ERC20 tokens, or by ownership of NFTs. Examples of DAOs where membership and voting power is proportional to how many tokens you own include Uniswap and ENS. Examples of DAOs where they are based on NFTs include Meebits DAO.

Building our DAO
You want to launch a DAO for holders of your CryptoDevs NFTs. From the ETH that was gained through the ICO, you built up a DAO Treasury. The DAO now has a lot of ETH, but currently does nothing with it.

You want to allow your NFT holders to create and vote on proposals to use that ETH for purchasing other NFTs from an NFT marketplace, and speculate on price. Maybe in the future when you sell the NFT back, you split the profits among all members of the DAO.

Requirements
Anyone with a CryptoDevs NFT can create a proposal to purchase a different NFT from an NFT marketplace
Everyone with a CryptoDevs NFT can vote for or against the active proposals
Each NFT counts as one vote for each proposal
Voter cannot vote multiple times on the same proposal with the same NFT
If majority of the voters vote for the proposal by the deadline, the NFT purchase is automatically executed
What we will make
To be able to purchase NFTs automatically when a proposal is passed, you need an on-chain NFT marketplace that you can call a purchase() function on. There exist a lot of NFT marketplaces out there, but to avoid overcomplicating things, we will create a simplified fake NFT marketplace for this tutorial as the focus is on the DAO.
We will also make the actual DAO smart contract using Hardhat.
We will make the website using Next.js to allow users to create and vote on proposals
Prerequisites
You have completed the NFT-Collection Tutorial
You must have some ETH to give to the DAO Treasury
