## Smart Contracts

#### CRONOS:

##### TOKENS: 
SH33P:  `0x0694c9bf930b7456712cEde98bE770e110212B38`<br />
xSH33P: `0x6241C0616178322398465a4fBEbBE98F14cAa7C1`<br />
eSH33P2: `0xc0758b10CC2660320C3A67Df228608130C7d7419`<br />

SH33P is the primary token of the ecosystem, xSH33P is the staked variant and eSH33P2 is the internal mechanics token.
<hr />

##### MARKET GENERATION:
Event: `0x8e69618dcEdDC5a625A05a29c3a6312E97e6ad56`<br />
Distribution: `0x05A5FEF2CBd09e32B501Ce3a0B130Ef3BC1e51a4`<br />

The event collects user contributions over a set time, the distribution sends tokens to contributors.
<hr />

##### DISTRIBUTORS:
Oneshot: `0xe6d2f10901ed6e7224151944bca9E4061AA44F47`<br />
Multi: `0x92049BA6E3f5bf0415C64c015f813e391821a0d6`<br />

Oneshot was used to break initial amounts of CRO between system contracts and team members. Multi is used to distribute payments to team wallets.
<hr />

##### FLOOR CALCULATORS:
floorcalc: `0x9D210f0d18136E04f92d15C885ec6e695560dd39`<br />
floorcalcV1: `0xc3431D208f009E70Dc7D52A726d2C8DA5C31e870`<br />

These calculators are used in configuration at deployment time and in production, to help calculate available reusable wrapped base.
<hr />

##### ECOSYSTEM CORE:
feeSplitter: `0xb1d7681557C4395dA470272E4233Bf473B093A49`<br />
transferGate: `0x314fBACCd79Ef847A8A223667066C718d80fB9ea`<br />
liquidityController: `0xCA2EE70Bc4A10214af392E5210db1230A7E5A0FD`<br />

FeeSplitter redistributes collected fees between set contracts and addresses of the SH33P ecosystem. TransferGate regulates fees and the handling of fee configuration. LiquidityController enables the project team to manage locked liquidity of the protocol.
<hr />

##### FUNDING BREAK-OFFS:
burnPit: `0x8Fb20C603e728aB081fcD9856A4d400ADcce344f`<br />
stockpile: `0x7146e93f9bc1D8A0d080e46559EaA8A8A04b0776`<br />
vegasparty: `0xE994941704bDF486C447F23E881B5C76Cb6E7de1`<br />
marketing: `0xC118813fe95F1A4d8E7ff7D4CD3341F9740Cc7D2`<br />

BurnPit is permanently burned tokens - they can never be retrieved. This enables more tokens to have their value extracted by elite mechanics - scarcity is directly responsive to volume of the protocol. Stockpile is a holding of SH33P token collected from fees, to be distributed to Degen NFT holders via the NFT Fee Splitter.

VegasParty is tokens to be sold, to aid in the funding of the annual Degen Protocol meetup, held in Las Vegas and hosted by Degen Protocol team / board members. Marketing is a stack of tokens distributable for marketing purposes (airdrops, bounty payouts, hiring, freelance contributions, etc etc).
<hr />

##### VAULT AND BOOSTER:
Vault: `0xdda37d90Fa3C2E6B81a8B48685edF19342E7B230`<br />
Booster: `0x121b80bD65D88c82e19A3D4Bb02CDFBD62FAbDB3`<br />

The Vault contract is based on Bankroll Stack, with minor modifications to suit distribution of the 10% deposit and withdraw fees. From the FeeSplitter contract, the Booster contract receives SH33P, which is converted to xSH33P and added to the 'drip pool' component of the Vault contract.
