# new-EIP918

## A PROPOSAL FOR A REORGANIZED EIP 918  

### Author: Rick Park, ceo@xbdao.io  

The current revision of the EIP918 standard suffers of some usability problems related to: some incongruences in naming convention in the various sections, apparent definition of externally visible variables and not of the methods used to access them (even if in the most case some their implicit getter is implied), huge technical material not perfectly congruent in the various sections, and so on. As a result of the actual situation, the use of the specification is somehow difficult for the mean skilled programmer.
The proposed revision aim is to have a part organized using the so called 'lawyer paradigm', where what is not specified is permitted and any word of the specification RESTRICTS the possible implementations to the proposed standard. Suitable examples of this approach in the Ethereum field can be found in the ERC20 specification. The proposal have a first part (here below described) mandatory, where all the new proposed minable tokens as per the proposed standard are asked to precisely follow in any aspect. There is a second part which recommends some not mandatory aspect, which are suitable to simplify and rationalize the internal structure of the contract.
A suitable backwards compatibility section is presented, where already existing token, if implementing at least that interface, should be declared compliant to EIP918-B because substantially EIP918 compliant, but for some naming convention.
For the sake of simplicity, a suitable EIP918 interface file ('IEIP918.sol') is presented to be included in the source code for compatibility assurance by means of inheritance and local overloading, while an Abstract Contract file ('AEIP918.sol') suited to guarantee both EIP918 and EIP918B compatibility is presented for possible inclusion.
All the huge technical material present in the previous draft of this EIP should be reorganized under the section 'Implementation notes and examples'.
Is to be evaluated the needing and opportunity to include the merge mining and delegate mining definition at this level: probably it can be treated in the recommended practice section only, being a very particular case.
