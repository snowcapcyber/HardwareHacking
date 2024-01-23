# Hardware Hacking Tools and Techniques

Increasingly Embedded Systems and the Internet of Things are forming part of the infrastructure that we use everyday. Failure of this infrastructure could result in serious social and economic damage, and in certain cases the failure of this infrastructure could result in loss of life. To limit this potential damage we need to perform Hardware Vulnerability Assessments so as to ensure that the devices that form this infrastructure are fit for purpose. In order to answer this question was must first define what a vulnerability is. 

The ISO 27001 standard for ISO Information Security Management Systems defines a vulnerability as “a weakness of an asset or control that could potentially be exploited by one or more threats.” Additionally, ISO further defines a threat as any “potential cause of an unwanted incident, which may result in harm to a system or organisation.”

Typically, vulnerability assessments (aka penetration tests) are used either to identify the level of technical risk emanating from a set of vulnerabilities, or to assess the efficacy of tamper resistance. Exactly what techniques are used, what targets are allowed, how much knowledge of the system is given to the testers beforehand and how much knowledge of the test is given to stakeholders can vary within the assessments regime. Hence the role of a Hardware Vulnerability Assessment is to identify, validate and document a set of vulnerabilities on the Target of Evaluation (ToE) in a scientifically reproducible manner. 

A stakeholder, or set of stakeholders, functions to define the scope and scale of the test, and these stakeholders can include regulators as well as risk owners. Stakeholders wish to reduce/minimise the risks that they face, and the level to which they wish to do this is dependant on their risk appetite. To that end, a Hardware Security Assessment can function to demonstrate compliance with a risk reduction policy, as well as adherence to a set of legal, business, social, moral and ethical requirements. It is critical to note that all Hardware Security Assessment must operate within the confines of the law. \\

The key concepts for a Hardware Vulnerability Assessment are depicted in Figure 1. Any given threat agent will have a set of amplifiers, and inhibitors, that function to promote or reduce the likelihood of an attack. The goal of an HVA is to identify a set of counter-measures and inhibitors that will reduce the risk of a successful attack against a target of evaluation to its lowest level.

When conducting a security assessment the assessor will function as a threat agent and perform a set of threat actions against a target of evaluation to try and compromise it. These actions are documented over the course of a Security Assessment and their results function to give a picture of the security state of an asset. Then from the security state of the asset the assessor can derive a set of countermeasures and recommendations as to how the security state of the asset can be improved.

Types of tests that can be carried out by testers armed with varying amounts of information about your hardware/embedded system include the following:\\

* White-Box Testing - Full disclosure about the target of evaluation  (ToE) is shared with the testers; this can include design documents and schematics as well as source code and compiled binaries. This type of testing confirms the efficacy of internal vulnerability assessment and management controls by identifying the existence of known vulnerabilities and common misconfigurations. White-Box testing can also include code-reviews. 

* Grey-Box Testing - Partial disclosure about the target of evaluation  (ToE) is shared with the testers; this can include some (but not all) design documents and schematics as well as source code and compiled binaries. This type of testing confirms the efficacy of internal vulnerability assessment and management controls by identifying the existence of known vulnerabilities and common misconfigurations. However, due to only partial disclosure of information relating to the Target of Evaluation (ToE) it can also result in vulnerabilities remaining undiscovered.

* Black-box testing - No information is shared with the testers about the internals of the  target of evaluation  (ToE). This type of test more accurately models the risk faced from attackers. However, the lack of information can also result in vulnerabilities remaining undiscovered in the time allocated for 

When developing a testing strategy to use in a hardware security assessment we can make use of the following:

* Vulnerability identification in bespoke or niche hardware.
  
* Scenario driven testing aimed at identifying vulnerabilities.

The role of a Hardware Security Assessment is to identify and document vulnerabilities on the target system (Target of Evaluation). Testing on the target can be non-invasive or invasive and functions to simulate a set of cyber attacks. A Hardware Security Assessment is a method for gaining assurance on the security of an hardware/embedded system by attempting to breach some or all of that system's level of security, using the same tools and techniques as an adversary might use, and consists of a number of distinct iterative phases. Figure 1 illustrates the phases associated with  Hardware Security Assessment.

The above figure defines the key elements in the Hardware Vulnerability Assessment (HVA) Process. A key element to note about this process is its iterative nature. Unlike other process models this model allows for a security tester to move between elements in the process model based upon the results of a specific element. These processes can be defined and documented using standards such as ISO9000 and IS17025. We can also measure the maturity of the HVA processes via a standard five level maturity model.

## Contact Details

For further information and questions please contact Dr Andrew Blyth, PhD. <ajcblyth@snowcapcyber.com>
