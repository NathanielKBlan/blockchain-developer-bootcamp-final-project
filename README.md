# LeadChain
A salesforce app to track leads/opportunities and recommend leads to prioritize

## Need
Throughout life (either personal or professional) we are presented with a wide variety of opportunities.
Each opportunity (or lead) gives us a chance at furthering our own goals, however it is also good to note that
because an opportunity presents itself, it doesn't mean that we always take it. This is because we subconciously
know that each lead caries a cost, be it monetary, time, or even the chance to pursue another lead. Consiously 
though we also consider the potential benefits of pursuing a lead, such as (but not limited to): monetary benefits,
social benefits, potential to generate further leads, etc. More often than not however we can either loose track of
our leads (especially when working solo or with a small team), forget about some, or be indecisive about what lead
to persue. Salesforce already does a great job at providing tools to track leads, but LeadChain goes one step further
and provides robustness, security, and recommendations when it comes to leads.

## Need for a Blockchain Solution
Before I go into what LeedChain is, I want to explain why a blockchain solution is an optimal one here.
It really comes down to a simple checklist, such as this one:
[Is a Blockchain Necessary?](https://github.com/NathanielKBlan/blockchain-developer-bootcamp-final-project/blob/main/readme-resources/poc/blockchain-checklist.png?raw=true) [^1]

By going down this list I'll explain why a blockchain solution is a good choice for the task LeedChain is trying to accomplish.

### Do you need to store state
Yes, in order for LeadChain to be able to provide it's recommendation it relies on data, and with leads new data is always coming in
and with taken leads we also want to record any measurable outcomes into our state.

### Are there multiple writers
Yes, LeadChain is meant to be used as an "enterprise" application as multiple leads will present themselves to multiple people
in the organization and we want them to all be able to record the leads they have at hand, which they've undertaken, and what
the outcomes were.

### Can you use an always online trusted third party
No, in this case it's best not to trust third parties with tracking your leads or determining which to undertake. No one will care
as much as you about YOUR leads!

### Are all writers known
Yes, in this case you will want to know who all the writers so that one can be sure that any writer present is part of the organization.

### Are all writers trusted
No, each person in the organization would want to persue their own lead due to bias or some benefit.

### Is public verifiability required
No, nodes running the verification process on the blockchain network must belong to the organization.

### End result
The solution (LeadChain) requires a private permissioned blockchain.


[^1]: Wust, K., &amp; Gervais, A. (2018). Do you need a blockchain? 2018 Crypto Valley Conference on Blockchain Technology (CVCBT). https://doi.org/10.1109/cvcbt.2018.00011 
