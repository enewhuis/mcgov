# mcgov
MCGov - EVM-based (Ethereum) Multi-class Governance Tokens

## ABSTRACT

Currently there is no standard for DAO voting power weighted by token class e.g. having distinct founder, preferred, dev, and common shares, etc. with the same equity implications but distinct voting power.

Current ERC20-based governance solutions assume a single voting class where voting power equals ERC20 token balance.

ERC1155 improves the situation for managing a set of related tokens from a single contract, however, it does not provide an aggregate view of the non-weighted equity share.

MCGov will extend Open Zeppelin governance to support an opinionated ERC1155/ERC20 hybrid enabling classes of distinct voting power, provide an ERC20 view of account equity, and host a web app to deploy custom multi-class DAO tokens for use with governance UI/UX e.g. withtally.com.

## BACKGROUND

* DAO - Distributed Autonomous Organization
* ERC20 - widespread standard for single-class tokens on Ethereum.
* ERC1155 - emerging standard for fungibility-agnostic token sets.
* Open Zeppelin - popular well-audited and robust framework for Solidity smart contract development.
* Governance - DAO system of voting whereby functions may be proposed, voted, and executed through smart contracts.
* Voting Power - the weight of an account-cast vote based on a token balance.
* WithTally.com - popular user interface to standardized governance contracts.

## OPPORTUNITY

Many DAO founders are looking for a multi-class solution they can customize for their particular project.  The current governance systems based on voting with a flat voting power distribution are not the most general solutions nor the best solution for many use cases attempting to achieve a balance of founder, expert, and common vote governance.

Example:

Loci Global DAO (LG) tokens represent voting power held by Loci associates for on-chain governance of mutual property assets.  The DAO distributes two classes of voting power--350,000 LGY founder shares with 35% of voting power and 440,650,000 LG common shares with 65% of voting power.

    440,650,000 LG  as ERC1155 65% voting power
        350,000 LGY as ERC1155 35% voting power
    -----------
    441,000,000 LG  as ERC20

LG intends to deploy a single smart contract that will allow holders to hold either token class while at the same time providing ERC20 semantics for standard online wallets.  Holders from both classes may issue proposals for governance via UI such as withtally.com and their respective voting power will be determined based on the particular classes held in their accounts.

## SOLUTION OVERVIEW

1. Juicebox DAO Token Raise
2. Website with Static Project Details
3. MCGov Multi-class Base Contract
4. MCGov Multi-class Token Deployer Contract
5. Website extended with Token Deployer App (app)
6. LG Contract Example Use Case
7. MCGov-based MCGov DAO Token (replaces Juicebox DAO Token)
8. MCGov DAO governance of future maintenance and development 

## VERSION 1 DRAFT PROJECT PLAN

- Develop prototype 0 base ERC1155_ERC20_Votes contract in Solidity on Rinkeby. [$6000]
- Develop prototype 0 LG contract based on ERC1155_ERC20_Votes and deploy on Rinkeby. [$3000]
- Initial Testing, Enhancements, and Fixes on Rinkeby. [$3000]
- Develop static project website. [$2500]
- Head hunt 5-member technical review board (recruiter search fees) [$5000]
- MCGov Customer Development (Marketing, Influencers, etc.). [$36,000]
- Design MCGov token deployer contracts and UI/UX. [$12,000]
- Review Board Introduction meeting [$2500]
- Review Board Iteration planning meeting 1 [$2500]
- Develop and deploy contracts, app, and LG governance prototype 1 on Rinkeby [$12,000]
- Review Board Iteration planning meeting 2 [$2500]
- Develop and deploy contracts, app, and LG governance prototype 2 on Rinkeby [$12,000]
- Community Test Round 1 (recruit, lead, collect, and report) [$6000]
- Audit (e.g. Code4rena) ERC1155_ERC20_Votes and related contracts. [$50,000]
- Review Board Iteration planning meeting 3 [$2500]
- Develop and deploy contracts, app, and LG governance prototype 3 final. [$12,000]
- Community Test Round 2 (lead, collect, and report) [$4000]
- Review Board Iteration planning meeting 4 [$2500]
- Implement final versions of MCGov contracts, app, and LG governance example. [$6000]
- Deploy LG and LG Governance contracts via token deployer web app on Mainnet. [$2000]
- Deploy MCGOV Governance token with review board members as founders shares. [$2000]
- Juicebox -> MCGOV token conversion (web app and community education). [$3000]
- MCGov WithTally.com listing [$3000]
- Initial Community Support [$6000]
- Legal and Accounting Fees [$6000]
- "18%" Overrun Buffer / initial web app maintenance budget [$39,600]


## TOTAL STARTUP COSTS

Seeking $244,800 in funding via Juicebox.money
