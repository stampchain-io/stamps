<h1>STAMP VAULT</h1>
<p><strong>A method of permanently securing Ordinal Sats within a Bitcoin Stamp vault</strong></p>

<p><strong>Authors:</strong> Arwyn, Kevin, B0B Smith and Mike In Space</p>

<p><strong>Introduction:</strong> Ordinals introduced a novel method of instantiating individual "Satoshis" when viewed through the lens of "Ordinal theory". However, these atomized "Sats" have proven to be quite fragile in that they can easily be spent by mistake. This is due to their very nature of being tied to specific UTXOs which the Bitcoin protocol has no awareness of. Ordinal theory is an overlay "metaprotocol" that operates by its own rules, but relies on lower-level transfer of UTXOs at the base layer. In contrast, Counterparty assets utilize an account-balance model wherby the ruleset operates independantly of specific UTXOs.</p>

<p>Bitcoin Stamps added a novel twist to the traditonal Counterparty approach by adopting the account-balance model but opting to store data within transaction outputs rather than OP_RETURN messages. What this means is that Ordinal theory utilizes UTXOs to determine ownership while Bitcoin Stamps utilizes UTXOs for data storage. It also presents a unique opportunity to leverage aspects of both protocols in order to provide a robust method of permanently storing Ordinals within Bitcoin Stamp vaults.</p>

<p>Bitcoin Stamps (OLGA-encoding) places the Counterparty OP_RETURN message (used to control transfer of ownership) in Position 2 (vout:1). This provides an opportunity for the first output to be reserved for an inbound "Sat" which is compliant with Ordinal theory.</p>

<p>In this way, a Sat tracked by Ordinal theory can be secured within a Bitcoin Stamps' first output and then subsequently stored or transferred using the account-based model of Bitcoin Stamps. This adds a layer of resilience and cannot accidently be spent.</p>

<p><strong>Consequences of this approach:</strong> Stamp Vault should be recognized as a one-way peg from Ordinals to Stamps, similar to "Teleburn" which is utilized by Ordinals.</p>

<p><br><img src="https://i.imgur.com/KfuXNvz.png"></p>





