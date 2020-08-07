## Open procurement procedures
---

### One-stage competitive procedure (Micro, RPQ, Open)

Depending on the type of procedure, method of procurement, geography and the legal basis, the attribute composition of the model can be adjusted, but its general logic remains unchanged for all types of procedures.
The contracting process based on competitive procedure is commonly carried out in the following sequence:

#### Business Process Diagram (go to https://goo.gl/bdUhh6)
Announce a tender
Creating a tender, CA determines key fields of the yet-to-be announced procurement, uploads tender documentation, with the requirements to the procurement object indicated as that which determines winner evaluation criteria.
Scoring function implementation
To achieve MEAT, Procuring Entity can use a scoring function by defining together with a regular common information a set of criteria, its available options and coefficients of such options to determine the total available weight of all components of bid and background of evaluation. 
Criteria
Set of criteria may include different types of requirements, used in different ways and for different reasons. Moreover, some used criteria may be prescribed by the legal basis “by default” (exclusion grounds of ESPD or particular chapters of selection grounds from ESPD, like General yearly turnover). 
Read more about criteria under scoring function


Conversions
Where scoring function to be applied, a set of verifiable conversions needed for future ranking and evaluation. 
Read more about conversions for scoring function

Evaluation panel 
Set of Procuring Entity evaluation pannel could be announced or updated (if some changes or replacements took place since PN for this contracting process was published and evaluation panel was expressed there). 
Read more about PEs' evaluation committee



Clarification period
Clarification period is separately distinguished in the procurement procedure during which participants can ask questions regarding the procurement requirements, demand issue resolution, and submit a claims, while CA can provide answers to questions and introduce changes into the procurement conditions (according to the rules and limitations below). The duration of the clarification period and offer submission is determined by CA but in any case can not be less than those prescribed by Law.
Suspending of procedure
Any accepted enquiries which have no relevant clarification provided by CA before ‘enquiryPeriod.endDate’ suspend the start of next phase of contracting process - submission period.
Unsuspending of procedure
After the publication of the CAs’ clarifications, procedure is unsuspended automatically with prolongation of ‘enquiryPeriod’ according to the rules, prescribed by Law.
Future steps
In addition to existing opportunity to ask questions about the procurement procedure, any user in the system (except Procuring entity) can contact Procuring entity and make a Violation elimination claim about the tender conditions. The Procuring entity has prescribed period to review the claim and make a decision on it. During this period the Procuring entity must publish a response to the claim and (in the case of complaint satisfaction) amend the appropriate procurement conditions or awarding procedure results.
Complaint submission 
Complaints on conditions received during clarification period transfer to the official Review body. After the complaint submission, a representative of the Review Body checks whether all requirements are fulfilled and carried out. If so, complaint is accepted for review. Otherwise, it is rejected. 
Complaint withdrawal 
At any time before the publication of the Review body’s decision, the complainant can withdraw his complaint.
Standstill period
The duration of the applicable standstill period following a challenge or complaint of tenders’ conditions or actions taken by the Procuring Entity that are allegedly not in compliance with the provisions of the Law. 
Reviewing
To indicate the results of review of accepted complaint, representative of Review Body must specify the results via changing of status of reviewed complaint together with contribution of additional needed information. 
If the complaint was dismissed by Review body, standstill period of such complaint ends
If the complaint was satisfied by Review body, the Procuring entity carries out the decision under its own responsibility, there are no additional automatic control means. Carried out decision marked with ‘satisfied’ state by CA himself indicates that prescribed judgments of Review Body are satisfied and complaint is complete.

Amendments or additional information
The Public Sector Directive in its introduction regulates the circumstances where modifications to a contract notice while it is being carried out are possible without a requirement to start a new tender process.
Introduction 82:
It should be clarified that the need to ensure that economic operators have sufficient time in which to draw up responsive tenders may entail that the time limits which were set initially may have to be extended. This would, in particular, be the case where significant changes are made to the procurement documents. It should also be specified that, in that case, significant changes should be understood as covering changes, in particular to the technical specifications, in respect of which economic operators would need additional time in order to understand and respond appropriately. It should, however, be clarified that such changes should not be so substantial that the admission of candidates other than those initially selected would have been allowed for or additional participants in the procurement procedure would have been attracted. That could, in particular, be the case where the changes render the contract or framework agreement materially different in character from the one initially set out in the procurement documents.

Permitted or non-significant modifications of contract notice during their term – then new procurement procedure is not required
To be provided
Prohibited or substantial modifications of contract notice during their term – new procurement procedure required    
To be provided    
How to handle contract modifications    
To be provided            

Submission of the offers
Once the clarification period is over the CA can no longer introduce changes into the Contract Notice. Economic Operators submit offers that are confidential. 
Requirement responses for automated ranking and evaluation 
Having a set of requirements defined by Procuring Entity and a number of values available, tenderers by preparing their offers, include a values for each requirement, reflecting the substance of the offer and fulfilling general corporate profiles’ data requested by Procuring Entity or required by the Legal Framework of particular jurisdiction. While submitting their proposal tenderers also fill the non-price parameters — values for specific verifiable tenderer attributes of the offer. 
Read more about structured bids

Modifications
An Economic Operator may modify its electronic bid by submitting online within submission deadlines a new information regarding previously submitted offer in accordance to the electronic submission procedures. 
Withdrawal
An Economic Operator may withdraw his electronic bid by submitting online within submission deadlines a request for cancellation of previously submitted offer.
Substitution 
An Economic Operator may substitute his electronic bid by submitting online within submission deadlines a request for cancellation of previously submitted offer and the new electronic bid in accordance to the electronic submission procedures.



Reverse Auction
Single unique link for each scheduled electronic auction will be available in Public Point. Depending on access-mode (with or without token) this link might work as:
individual link of the participant, who accesses his personal page via this link and participates in the auction.
public link to the auction which can be published anywhere for viewers, who use this link to observe.
Preparation of the auction
Date and time of the auction are determined by the BPE automatically, once the Contract Notice is published. Platforms have to inform their users about the upcoming auction beginning date. If no participant is registered (or only one bid received) after the end of the tender period, the system automatically changes the process status to ‘unsuccessful’. 
Note that electronic auctions (if included) are held for each lot separately


If more than one participant is registered, the system activates the e-Auction module. Those participants who registered their offers for this particular procurement can participate in the auction. All the other users, including the CA of this process, can observe how the auction develops. Once the Auction is established, the NEPPs are granted access to the auction web-page for participant access provision to the auction. 
Then the auction-phase ends
Once all established under single submission stage electronic auctions end partially disclosure of all the Information on tenderers and their bids occur. Such partially disclosed information includes all the data except financial offer digitalization (financial envelope). This granularity will be disclosed only for single qualified offer during the evaluation process.
Information disclosure on tenderers occurs once the last auction in this process is completed


Evaluation and identification of the procurement winner
Once the submission period is over and participants can no longer submit or update their bids, the system will disclose all submitted bids. 
In case if after submission period end there is nothing to disclose (no bids were submitted) or all submitted bids failed, the system will automatically change this specific lot of this contracting process to status “unsuccessful”. 
Where enough number of bids received during the tendering period, the system will generate a set of qualification envelopes (awards) and launch the awarding period for this contracting process.
Eligibility check
Automated check
System will automatically verify eligibility (based on data available via external bus) of each tenderer whose bid was disclosed according to rules of dispatch under the current procurement method. 
Read more about automated eligibility check


Manual check
Where automated check is not available, Procuring entity shall provide an eligibility check manually. Depending on award criteria applied, the system will disclose either eligibility documents only or full package of documents submitted by EOs within their bids. 
Read more about envelopes disclosure rules


System will allow PE to check eligibility of the candidates against initially announced criteria in any order.
The financial part of bids of those candidates who passed eligibility check will go to the technical evaluation. All the others who failed eligibility check are excluded from evaluation.
Initial ranking for evaluation
Depending on award criteria applied system will rank eligible bids and suggest them in order of admissibility: from the most to the least acceptable by applicable criteria. This automated ranking is undertaken using a set of criteria and the relevant conversions applied by PE for each available value of each applied requirement and published in a Contract Notice on one hand. And the requirement responses submitted by each EO against published criteria on another hand.
Read more about initial ranking according to the scoring function

Technical evaluation 
CA sequentially reviews bids that are eligible starting with declaration of non conflict of interest beginning with first ranked by the system.
Declaration of non-conflict of interests
Due to requirements of declaration of non conflict of interest by evaluation panel members against each tenderer for each bid to be evaluated, the system will generate relevant requests for each evaluation panel member declared by Procuring Entity within Contact Notice. 
Each initial or new (in case of replacement) member of the evaluation panel shall submit relevant responses in order to  confirm an absence of conflict of interest for each tenderer (legal entity) in each bid received for evaluation by panel. 
Since this is a declaration following Open Government Principles, this action does not block the evaluation process. It means that technically Procuring Entity can pass this stage and start the evaluation without declarations by evaluation panel members. But this PEs decision will be reflected in the system and published for public access. 

Technical consideration
Evaluation panel considers technical compliance according to the award criteria methodology applied and a scoring function (where included). If the most acceptable bid is in compliance with the CA’s technical requirements, PE determines this offer as a qualified and goes to the next step - financial evaluation. If it is not, PE confirms his decision to disqualify the participant and declines such an offer. Then the system suggests to qualify the next offer from the acceptance perspective.
Financial consideration
Evaluation panel considers financial compliance according to the award criteria methodology applied and a scoring function (where included). If a qualified offer is in compliance with the CA’s financial requirements, PE determines this offer as a winner. If it is not in compliance, CA confirms his decision to disqualify the offer on this (evaluation) stage, and declines such an offer. Then the system suggests to qualify the next offer from the acceptance perspective.
If all the offers were declined by PE either on qualification step or on evaluation and upon the completion of complaining process (review period) this specific lot of this contracting process automatically changes to ‘unsuccessful’.
Evaluation Protocol
Once a winner is selected for each lot, CA submits the evaluation protocol which, in its turn, indicates the end of the awarding process. As a result of submission of evaluation protocol, the system will automatically generate a set of Contract Award Notices for each awarded lot, change evaluation stage to ‘awarded’ and launch the complaining process - review period.
Tender/lot cancellation
According to Public procurement standard forms guidance 2017-06-23 (version 1.1) Corrigendum is no longer used to inform about cancelled* (i.e. incomplete or unsuccessful) procedures. This is done by using the contract award notice, where non-award can be indicated, per lot, in section V.1. 
If contracting bodies wish to inform the market about their plan to cancel a procedure beforehand then they can advertise this at EU level using a сorrigendum notice. In this case, they should add a text announcing the intent to cancel ("The contracting authority or entity intends to repeal this notice.") in the "Other additional information field" (VII.2) and explain the reasons. After the standstill period has elapsed, they should announce the formal cancelation through the contract award notice as usual (with possibly repeating the reasons for the cancellation in the "Additional information field" (VI.3)).
CA can cancel either procedure or separate lot anytime before its completion 


Review period
Review period is a time-slot during which the decision of the procuring entity to award a contract or cancel competition under separate lot or all the contracting process can be challenged. All the tenderers whose offers were reviewed by PE are able to claim on such made decisions. This review period is the same for all the  tenderers. 
Future steps
If any complaints were received and accepted for review during the review period, the system automatically establishes standstill period for each received complaint separately.
Complaint submission
Complaints on made decisions received during the review period transfer to the official Review body. After the complaint submission, a representative of the Review Body checks whether all requirements are fulfilled and carried out. If so, complaint is accepted for review. Otherwise, it is rejected. 
Complaint withdrawal 
At any time before the publication of the Review body’s decision, the complainant can withdraw his complaint.
Suspending of procedure
Such accepted complaints block the opportunity to run contracting step (publish a contract with the winner) and suspend all evaluation stage via establishing of special time-slot: system automatically establishes standstill period for each complaint received and accepted for review.
Standstill period
The duration of the applicable standstill period following a challenge or complaint of decisions or actions taken by the Procuring Entity that are allegedly not in compliance with the provisions of the Law. 
Reviewing
To indicate the results of review of accepted complaint, representative of Review Body must specify the results via changing of status of reviewed complaint together with contribution of additional needed information. 
If the complaint was dismissed by Review body, standstill period of such complaint ends
If the complaint was satisfied by Review body, the Procuring entity carries out the decision under its own responsibility, there are no additional automatic control means. Carried out decision marked with ‘satisfied’ state by CA himself indicates that prescribed judgments of Review Body are satisfied and complaint is complete.
Unsuspending of procedure
After the publication of the Review body’s decision with the status “dismissed” procedure is unsuspended automatically. Satisfied complaints should be changed by CA to ‘complete’ state.

Concluding an agreement
As soon as either review period or all established standstill periods expired, CA will prepare and publish the concluded agreement for signing and verification. 
Preparation
Once review period ends, the system automatically generates a set of drafts of future awarded contracts (AC) - separate draft for each determined winner. CA updates these drafts with actual needed data (required according to local rules) and, once all such updates are done, CA indicates this contract is fully prepared for signing. System automatically generates PDF of needed contract based on received data and standardized template. Such pdf-document will be put to the ‘documents’ section of specific contract and all this contract will be switched to  ‘ready for signing’ state. Thereafter, signing and validation process starts
Signing

Validation 
Activation
At this point, the awarding process is completed, and no further actions are required. The evaluation phase goes to ‘complete’ state and all the contracting process goes to ‘execution’.
Future steps
Implementation
To be provided
Transactions
To be provided


