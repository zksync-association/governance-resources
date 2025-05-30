# Token Program Multisig Guidelines

## Purpose

These guidelines advise the setup and management of all multisig wallets that have access to the ZK token or other assets affiliated with a ZKsync Token Program approved by the Token Assembly. These multisigs protect the authority to mint ZK and distribute assets. These accounts should adhere to necessary security standards to protect ZK token supply authorized by the Token Assembly.

## ZKsync Token Program Multisig Guidelines

Any multisig wallets that have access to the ZK token or other assets affiliated with a ZKsync Token Program should follow the guidelines below.

Each multisig must configure their Execution Threshold based on its risk profile. The risk profile is primarily defined based on assets under control (e.g. ZK, USDC or ETH), yet should also take into consideration code and contracts the multisig influences.

| **Risk Profile** | **Approximate USD Value** | **Execution Threshold**  |
| --- | --- | --- |
| Low / Tactical | <$1M | 3/5 Minimum |
| Medium / Operational | ~$1-$10M | 3/5 Minimum |
| High / Strategic | >$10M | 5/7 Minimum or Governor Admin |

In addition, each multisig must follow industry standard best-practices, such as those listed below:

### **Multisig Set-Up and Maintenance Checklist**

- The multisig structure, participation, and change policy is communicated publicly. For example, it is outlined in the related Token Program Proposal.
    - Only participants included in the communication hold keys.
    - High-risk multisigs include at least one representative from an external oversight entity, either Security Council or ZKsync Foundation.
        - The identity of high-risk signers may remain **confidential** and known only to the following parties:
            
            a) ZKsync Association; and 
            
            b) ZK GPS [LINK]; and 
            
            c) other members of the same multisig.
            
        - Signers must confirm key control via onchain message upon creation of multisig.
- Changes to multisig participation are communicated publicly on the governance forum for all Token Programs.
    - Changes to multisig signers do not lower the absolute number of signers below Token Proposal approved one or lower the threshold below Token Proposal approved one.
    - Changes to multisig participation, including number of signers and thresholds, for high-risk multisigs are approved via an onchain vote, as defined in the approved proposal.
- The multisig is verified onchain.
- The multisig is closed-down (i.e. passed to the burn address) once all related contracts are not necessary or the Token Program is complete. Multisigs and public keys are not reused.
- The multisig set-up is reviewed by at least on external security team within the Security Council or vetted security organization.
- Multisig address for admin of a Token Program primary capped minter is shared in onchain proposal.

### **Signer Guidelines Checklist**

- Signers use a secure hardware wallet (e.g. Ledger, Trezor).
- Signers control only one private key per multisig.
- Keys are not reused across multisigs.
- Keys are not used for any unrelated on-chain activity.
- Lost or compromised devices are reported immediately, and affected keys replaced.
- Passive signers, such as a backup signer, do not meet the threshold on any multisig.
- For high-risk multisigs, here are some additional measures to consider:
    - The threshold of signers is never present in a single physical location (e.g., conference, retreat)
    - Signers must define internal verification method for transactions >1M ZK, such as video call, secret pass phrase, and/or verification through two independent communication channels.

### Industry References

- [How to multisig](https://howtomultisig.com/)

### Document Update Process
The ZKsync Association will review the risk profiles and security requirements once per year based on industry standards and governance requirements.

</aside>
