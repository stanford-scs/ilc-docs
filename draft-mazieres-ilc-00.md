% Title = "ILC: Internet-level consensus"
% abbrev = "ilc"
% category = "exp"
% docName = "draft-mazieres-ilc-00"
% ipr= "trust200902"
% area = "Internet"
% workgroup = ""
% keyword = ["tcp", "encryption"]
%
% date = 2017-02-13T00:00:00Z
%
% [[author]]
% initials="S."
% surname="Fleckenstein"
% fullname="Scott Fleckenstein"
% #role="editor"
% organization = "Stellar"
%   [author.address]
%   email = "scott@stellar.org"
%   [author.address.postal]
%   street = "170 Capp St., Suite A"
%   city = "San Francisco, CA"
%   code = "94110"
%   country = "US"
%
% [[author]]
% initials="D."
% surname="Mazieres"
% fullname="David Mazieres"
% #role="editor"
% organization = "Stanford University"
%   [author.address]
%   email = "dm@uun.org"
%   [author.address.postal]
%   street = "353 Serra Mall, Room 290"
%   city = "Stanford, CA"
%   code = "94305"
%   country = "US"
%
% [[author]]
% initials="J."
% surname="McCaleb"
% fullname="Jed McCaleb"
% #role="editor"
% organization = "Stellar"
%   [author.address]
%   email = "jed@stellar.org"
%   [author.address.postal]
%   street = "170 Capp St., Suite A"
%   city = "San Francisco, CA"
%   code = "94110"
%   country = "US"
%
% [[author]]
% initials="M."
% surname="Shore"
% fullname="Melinda Short"
% #role="editor"
% organization = "Fastly"
%   [author.address]
%   email = "mshore@fastly.com"
%   [author.address.postal]
%   street = "PO Box 16271"
%   city = "Two Rivers, AK"
%   code = "99716"
%   country = "US"
%
% [[author]]
% initials="D."
% surname="Steffan"
% fullname="Deian Stefan"
% #role="editor"
% organization = "UCSD"
%   [author.address]
%   email = "???"
%   [author.address.postal]
%   street = "???"
%   city = "San Diego, CA"
%   code = "9????"
%   country = "US"

.# Abstract

An Internet-level consensus mechanism is one that accommodates the
decentralized nature of the Internet to agree on values without
relying on a centralized authority for configuration.  Specifically,
the goal is to achieve consensus in settings where there may be
Internet-wide benefit from agreement, yet the security concerns of
participants and the multi-national nature of the network preclude any
globally-acceptable consortium in which to concentrate trust.

{mainmatter}

# Introduction

# Threat model and feasible guarantees

# Applications

## Payments

## Package management

## Certificate transparency

Certificate Transparency (CT) is a mechanism, developed by Google and undergoing standardization at the IETF, which brings accountability to certification authorities (CAs) by providing the means to log and audit certificate issuance, and consequently to detect certificate misissuance, certificate leakage, and some other problems related to PKI operations on the public internet.  Issued certificates are logged to public servers, where they are stored in cryptographically signed public logs.  

The CT trust model depends on the integrity of the log.  That is to say, while CT inclusion proofs are used to verify that a given log includes a particular certificate, and that the parties to whom certificates have been issued are authorized to have them, there is nothing inherent to the CT mechanism that can be used to detect a misbehaving log.  One primary class of log misbehavior would be to give different view of the log to different viewers, or what is known as a partitioning attack.

The IETF Public Notary Transparency (trans) working group is responsible for standardizing CT.  They are in the process of specifying three experimental mechanisms for gossiping CT data, with the intent of detecting a non-conforming log, but these have not yet been implemented.

## End-user identification and key certification

# Protocols

# Security considerations

# Acknowledgments


{backmatter}
