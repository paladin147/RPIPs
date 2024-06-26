---
layout: other-content
title: Glossary of Terms
nav-title: Part 5 - Glossary of Terms
description: Defines some of the common terminology present in the other explainers.
author: Valdorff (@Valdorff), Paladin (@Paladin147)
custom-next: none
custom-prev: /tokenomics-explainers/004-rework-support
depth: Intermediate
---

{% assign cPrev=site.pages | where:"url", page.custom-prev | first %}
{% assign cNext=site.pages | where:"url", page.custom-next | first %}

<div class="prev-next-container">
{%if cPrev %}<a href="{{cPrev.url|relative_url}}">Previous - {{cPrev.title}}</a>{%else%}<span>Previous</span>{% endif %}
{%if cNext %}<a href="{{cNext.url|relative_url}}">Next - {{cNext.title}}</a>{%else%}<span>Next</span>{% endif %}
</div>

**Bonded ETH:** The portion of a validator’s ETH that is provided by the Node Operator. Sometimes called NO ETH or nETH.

**Borrowed ETH:** The portion of a validator’s ETH that is provided by the protocol (ultimately from rETH holders). Sometimes called protocol ETH or pETH.

**Cliff:** Description of RPL rewards going suddenly to 0 (as opposed to gradually declining) when you fall below 10% borrowed ETH worth of staked RPL. Aka RPL reward threshold.

**Forced Validator Exit:** The ability for the protocol to exit a validator (eg, for bad behavior, such as MEV theft). Currently only the node operator can trigger an exit, or the Ethereum protocol itself, which it does when the validator balance reaches 16 ETH.

**LEB, or x-ETH Bond:** Originally minipools used a 16 ETH Bond. As a result, smaller bonds were referred to as  “Lower ETH Bond” minipools, or LEBs. The Atlas release introduced LEB8s. The new proposal suggests 4-ETH bond validators and 1.5-ETH bond validators.

**LP:** Liquidity Provder. An LP deposit two tokens to a liquidity pool. The ratio of the sides determines the price. For example, a pool with 1 ETH and / 170 RPL gives an RPL price of .0058 ETH ($22 @ $3800 ETH/USD). Adding .1 ETH and 0 RPL to the pool would result in 1.1 ETH / 170 RPL = .0064 ($24.58 @ 3800 ETH/USD). In reality, much of that change would be 'arbitraged away', but in the meantime it has provided additional liqudity for RPL buys/sells and exerted upwards pressure on the RPL/ETH price.

**Megapools:** A single RP contract serving as the withdrawal address for multiple validators.

**MEV Theft:** When a node operator steals execution-layer rewards for profit. This requires a sophisticated, unethical, and lucky operator. See Node Level Penalties.

**Node Level Penalties:** The ability to penalize a Megapool in order to disincentivize MEV theft. The ability to penalize across validators means a malicious node operator can only profit when an opportunity is larger than their total bond across validators, rather than just their bond on one validator.

**NO:** Node Operator

**Top off:** To (buy and) stake more RPL to keep above the RPL reward threshold. (See Cliff).

**rETH TVL:** Total value locked in rETH. Consider it the “size” of the liquid staking token.

**Sock Puppet or Sybil:** A single entity creating and controlling multiple identities (sock puppets), usually for an attack or to gain influence. An example in Rocketpool is voting, as multiple fake identiies with the same number of RPL has greater voting power than a single identity due to quadratic voting, which incentivizes sock puppets/sybil attacks.

**Solo staking APY:** The yield for staking on a full 32-ETH validator (inclusive of consensus rewards, tips, and MEV rewards)


<div class="prev-next-container">
{%if cPrev %}<a href="{{cPrev.url|relative_url}}">Previous - {{cPrev.title}}</a>{%else%}<span>Previous</span>{% endif %}
{%if cNext %}<a href="{{cNext.url|relative_url}}">Next - {{cNext.title}}</a>{%else%}<span>Next</span>{% endif %}
</div>