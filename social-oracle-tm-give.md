---
description: >-
  Information about Coordinape GIVE on Base Chain via an EAS schema, generated
  from rich GIVE actions taken in CoLinks, Farcaster, and GIVE.party.
cover: >-
  https://images.unsplash.com/photo-1621508654686-809f23efdabc?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxjcnlzdGFsJTIwYmFsbHxlbnwwfHx8fDE3MTgzMTk3MDV8MA&ixlib=rb-4.0.3&q=85
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 🔮 Social Oracle™️ GIVE

## Find Social Oracle on EAS

[https://base.easscan.org/schema/view/0x82c2ec8ec89cf1d13022ff0867744f1cecf932faa4fe334aa1bb443edbfee3fa](https://base.easscan.org/schema/view/0x82c2ec8ec89cf1d13022ff0867744f1cecf932faa4fe334aa1bb443edbfee3fa)

## What is the Social Oracle?

Coordinape's recognition and reputation primitive [GIVE ](colinks/give.md)is ONCHAIN! \
GIVE is a Permissionless Public Good reputation primitive that creates a valuable and trusted Social Oracle of connections and attestations from peer to peer about skills and experiences.

\
GIVEs created in [Farcaster](https://www.farcaster.xyz/), [CoLinks](https://colinks.coordinape.com/info), and [GIVE.party](https://colinks.coordinape.com/giveparty) now get written to [Base Chain](https://base.org) via attestations created with[ Ethereum Attestation Service (EAS)](https://attest.org/).  We've built GIVE as a reputation primitive and brought it onchain to make it universally accessible and integratable. &#x20;

## How can I use it?

### Integrate the Social Oracle

Coordinape creates attestations on behalf of authenticated users when they create and give GIVEs to other users. Therefore GIVEs "From" `onchain.coordinape.eth` are highly trustworthy. \
\
You can query any EAS Schema using the EAS GraphQL API. [Learn more here.](https://docs.attest.org/docs/developer-tools/api)

#### **Some of the possible ways to integrate the Social Oracle**

* **Resume or CV** - GIVE can act as an endorsement that a given person has a skill. The more GIVE about the skill, the more trusted the person is likely to be about that skill.&#x20;
* **Social and professional Discovery** - The network of GIVEs reveals much rich data about people and relationships. It's extremely easy to get leads for people who have specific skills or qualities using the Social Oracle.
* **Gating/Eligibility/qualification -** Since GIVE is on [BASE](https://base.org) , it's easily possible to gate web3 organizations, events, groups, and more by simply requiring that participants have enough onchain GIVE or GIVE from a particular source or GIVE of a particular skill. There a many possibilities!
* **Humanity Scoring** - Given the social oracle data, it's easy to create or add to formulas that can add to or even guarantee the likelihood that a user is actually a human.&#x20;

### Issue GIVE attestations

Anyone can openly use the [GIVE Schema](https://base.easscan.org/schema/view/0x82c2ec8ec89cf1d13022ff0867744f1cecf932faa4fe334aa1bb443edbfee3fa) to create GIVE attestations.&#x20;

Use the [GIVE Schema](https://base.easscan.org/schema/view/0x82c2ec8ec89cf1d13022ff0867744f1cecf932faa4fe334aa1bb443edbfee3fa) to issue GIVE attestations from your trusted organization to add more trusted data to the Social Oracle.\
_\*If your org/project plans to do this, feel free to reach out to us in our_ [_Discord_](https://discord.gg/GFASZtq6Sw) _and we may be interested to integrate your GIVE data into our use of the Social Oracle._ \


## GIVE EAS Schema:&#x20;

[https://base.easscan.org/schema/view/0x82c2ec8ec89cf1d13022ff0867744f1cecf932faa4fe334aa1bb443edbfee3fa](https://base.easscan.org/schema/view/0x82c2ec8ec89cf1d13022ff0867744f1cecf932faa4fe334aa1bb443edbfee3fa)

| Field      | Type      | Purpose                                                          | Example(s)                                                                                      |
| ---------- | --------- | ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `from`     | `address` | Ethereum address                                                 | "0xd8da6bf26964af9d7eed9e03e53415d37aa96045"                                                    |
| `amount`   | `uint16`  | number representing amount of GIVE                               | "1"                                                                                             |
| `platform` | `string`  | app or platform the GIVE occurred on                             | "CoLinks", "GIVE.party", "Farcaster"                                                            |
| `url`      | `string`  | url for GIVE reference                                           | [https://warpcast.com/crabsinger.eth/0x6c2c498](https://warpcast.com/crabsinger.eth/0x6c2c4981) |
| `context`  | `string`  | text field for any desired purpose                               | "GIVE related to the Women in Web3 IRL event at ETH Denver 2024"                                |
| `skill`    | `string`  | a skill that this GIVE is endorsing for the reciever of the GIVE | "Community Management"                                                                          |
| `tag`      | `string`  | a tag that this GIVE is about                                    | "First Class"                                                                                   |
| `note`     | `string`  | a note from the GIVE sender to the receiver                      | "Your contributions to the project are unmatched! Thank you for making this project a reality!" |
| `weight`   | `uint16`  | number representing the quality of this GIVE                     | "300"                                                                                           |



<details>

<summary>EAS SDK GIVE example <br><a href="https://base.easscan.org/schema/view/0x82c2ec8ec89cf1d13022ff0867744f1cecf932faa4fe334aa1bb443edbfee3fa">This example comes from the GIVE Schema on EAS utilizing the EAS SDK. </a></summary>

{% code fullWidth="false" %}
```javascript
import  { EAS, SchemaEncoder }  from "@ethereum-attestation-service/eas-sdk";
const easContractAddress = "0x4200000000000000000000000000000000000021";
const schemaUID = "0x82c2ec8ec89cf1d13022ff0867744f1cecf932faa4fe334aa1bb443edbfee3fa";
const eas = new EAS(easContractAddress);
// Signer must be an ethers-like signer.
await eas.connect(signer);
// Initialize SchemaEncoder with the schema string
const schemaEncoder = new SchemaEncoder("address from,uint16 amount,string platform,string url,string context,string skill,string tag,string note,uint16 weight");
const encodedData = schemaEncoder.encodeData([
	{ name: "from", value: "0x0000000000000000000000000000000000000000", type: "address" }
	{ name: "amount", value: "0", type: "uint16" }
	{ name: "platform", value: "", type: "string" }
	{ name: "url", value: "", type: "string" }
	{ name: "context", value: "", type: "string" }
	{ name: "skill", value: "", type: "string" }
	{ name: "tag", value: "", type: "string" }
	{ name: "note", value: "", type: "string" }
	{ name: "weight", value: "0", type: "uint16" }
]);
const tx = await eas.attest({
	schema: schemaUID,
	data: {
		recipient: "0x0000000000000000000000000000000000000000",
		expirationTime: 0,
		revocable: true, // Be aware that if your schema is not revocable, this MUST be false
		data: encodedData,
	},
});
const newAttestationUID = await tx.wait();
console.log("New attestation UID:", newAttestationUID);
```
{% endcode %}

</details>
