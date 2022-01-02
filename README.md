# mcgov
MCGov - EVM-based (Ethereum) Multi-class Governance Tokens

MCGov - Ethereum Multi-class on-chain governance tokens.


ABSTRACT

Currently there is no standard for DAO voting power weighted by token class e.g. having distinct founder, preferred, dev, and common shares, etc. with the same equity implications but distinct voting power.

Current ERC20 solutions assume a single voting class where voting power equals ERC20 token balance.

ERC1155 improves the situation for managing a set of related tokens from a single contract, however, it does not provide an aggregate view of the non-weighted equity share.

MCGov will extend Open Zeppelin governance to support an opinionated ERC1155/ERC20 hybrid enabling classes of distinct voting power, provide an ERC20 view of account equity, and host a web app to deploy custom multi-class DAO tokens for use with governance UI/UX e.g. withtally.com.


BACKGROUND

ERC20 - widespread standard for single-class tokens on Ethereum.
ERC1155 - emerging standard for fungibility-agnostic token sets.
Open Zeppelin - popular well-audited and robust framework for Solidity smart contract development.
On-Chain Governance - DAO system whereby smart contract functions may be proposed, voted, and executed with public UI ecosystem, timelocked controllers, and other purposes.
Voting Power - the weight of an account-cast vote based on a token balance.


OPPORTUNITY

Many DAO founders are looking for a multi-class solution they can customize for their particular project.

Example:

Loci Global DAO (LG) tokens represent voting power held by Loci associates for on-chain governance of mutual property assets.  The DAO distributes two classes of voting power--350,000 LGY founder shares with 35% of voting power and 440,650,000 LG common shares with 65% of voting power.

    440,650,000 LG  as ERC1155 65% voting power
        350,000 LGY as ERC1155 35% voting power
    -----------
    441,000,000 LG  as ERC20

LG intends to deploy a single smart contract that will allow holders to hold either token class while at the same time providing ERC20 semantics for standard online wallets.  Holders from both classes may issue proposals for governance via UI such as withtally.com and their respective voting power will be determined based on the particular classes held in their accounts.


VERSION 1 DRAFT PROJECT PLAN

- Develop prototype 0 base ERC1155_ERC20_Votes contract in Solidity. [$8,000]
- Develop prototype 0 LG contract based on ERC1155_ERC20_Votes contract and deploy on Rinkeby for testing. [$4,000]
- Develop static project website. [$3,000]
- Assemble 5-member technical review board [$2,500]
- Develop "MCGov.App" dynamic multi-class token deployer web app. [$12,000]
- "MCGov.App" Customer Development (Marketing, Influencers, etc.). [$36,000]
- Review Board Introduction meeting [$500]
- Review Board Iteration planning meeting 1, implement/deploy prototype 1, LG governance example 1 [$6,000]
- Review Board Iteration planning meeting 2, implement/deploy prototype 2, LG governance example 2 [$6,000]
- Community Test Round 1 [$6,000]
- Audit (Code4rena) ERC1155_ERC20_Votes and related contracts. [$50,000]
- Review Board Iteration planning meeting 3, implement/deploy prototype 3 final. [$6,000]
- Community Test Round 2 [$6,000]
- Review Board Iteration planning meeting 4, implement final version. [$6,000]
- Review Board Remuneration [$30,000]
- Deploy LG and LG Governance contracts via token deployer web app on Mainnet [$2000]
- Deploy MCGOV Governance token with review board members as founders shares. [$2000]
- Juicebox -> MCGOV token conversion (web app and community education). [$3,000]
- MCGOV WithTally.com listing. [$3,000]
- Initial Community Support [$6,000]
- "18%" Overrun Buffer / initial web app maintenance budget [$50,000]


TOTAL PROJECT COST

Seeking $259,000 in funding via Juicebox.money
