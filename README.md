# Hardware Hacking Tools and Techniques

## Introduction
Increasingly Embedded Systems and the Internet of Things are forming part of the infrastructure that we use everyday. Failure of this infrastructure could result in serious social and economic damage, and in certain cases the failure of this infrastructure could result in loss of life. To limit this potential damage we need to perform Hardware Vulnerability Assessments so as to ensure that the devices that form this infrastructure are fit for purpose. In order to answer this question was must first define what a vulnerability is. 

The ISO 27001 standard for ISO Information Security Management Systems defines a vulnerability as "$a weakness of an asset or control that could potentially be exploited by one or more threats.}” Additionally, ISO further defines a threat as any “$potential cause of an unwanted incident, which may result in harm to a system or organisation.$”

Typically, vulnerability assessments (aka penetration tests) are used either to identify the level of technical risk emanating from a set of vulnerabilities, or to assess the efficacy of tamper resistance. Exactly what techniques are used, what targets are allowed, how much knowledge of the system is given to the testers beforehand and how much knowledge of the test is given to stakeholders can vary within the assessments regime. Hence the role of a Hardware Vulnerability Assessment is to identify, validate and document a set of vulnerabilities on the Target of Evaluation (ToE) in a scientifically reproducible manner. 

A stakeholder, or set of stakeholders, functions to define the scope and scale of the test, and these stakeholders can include regulators as well as risk owners. Stakeholders wish to reduce/minimise the risks that they face, and the level to which they wish to do this is dependant on their risk appetite. To that end, a Hardware Security Assessment can function to demonstrate compliance with a risk reduction policy, as well as adherence to a set of legal, business, social, moral and ethical requirements. It is critical to note that all Hardware Security Assessment must operate within the confines of the law. 

Any given threat agent will have a set of amplifiers, and inhibitors, that function to promote or reduce the likelihood of an attack. The goal of an HVA is to identify a set of counter-measures and inhibitors that will reduce the risk of a successful attack against a target of evaluation to its lowest level.

When conducting a security assessment the assessor will function as a threat agent and perform a set of threat actions against a target of evaluation to try and compromise it. These actions are documented over the course of a Security Assessment and their results function to give a picture of the security state of an asset. Then from the security state of the asset the assessor can derive a set of countermeasures and recommendations as to how the security state of the asset can be improved.

Types of tests that can be carried out by testers armed with varying amounts of information about your hardware/embedded system include the following:\\

* $White-Box Testing$ - Full disclosure about the target of evaluation  (ToE) is shared with the testers; this can include design documents and schematics as well as source code and compiled binaries. This type of testing confirms the efficacy of internal vulnerability assessment and management controls by identifying the existence of known vulnerabilities and common misconfigurations. White-Box testing can also include code-reviews. \\

* $Grey-Box Testing$ - Partial disclosure about the target of evaluation  (ToE) is shared with the testers; this can include some (but not all) design documents and schematics as well as source code and compiled binaries. This type of testing confirms the efficacy of internal vulnerability assessment and management controls by identifying the existence of known vulnerabilities and common misconfigurations. However, due to only partial disclosure of information relating to the Target of Evaluation (ToE) it can also result in vulnerabilities remaining undiscovered.\\

* $Black-box testing$ - No information is shared with the testers about the internals of the  target of evaluation  (ToE). This type of test more accurately models the risk faced from attackers. However, the lack of information can also result in vulnerabilities remaining undiscovered in the time allocated for 

When developing a testing strategy to use in a hardware security assessment we can make use of the following:\\
\begin{itemize}
\item Vulnerability identification in bespoke or niche hardware. \\
\item Scenario driven testing aimed at identifying vulnerabilities.\\
\end{itemize}

The role of a Hardware Security Assessment is to identify and document vulnerabilities on the target system (Target of Evaluation). Testing on the target can be non-invasive or invasive and functions to simulate a set of cyber attacks. A Hardware Security Assessment is a method for gaining assurance on the security of an hardware/embedded system by attempting to breach some or all of that system's level of security, using the same tools and techniques as an adversary might use, and consists of a number of distinct iterative phases. Figure 1 illustrates the phases associated with  Hardware Security Assessment.\\
\begin{figure}[]
\includegraphics[width=100mm]{Images/Process.png}
\centering
\label{Figure-2}
\caption{The Process Model} 
\end{figure}

Figure 2 defines the key elements in the Hardware Vulnerability Assessment (HVA) Process. A key element to note about this process is its iterative nature. Unlike other process models this model allows for a security tester to move between elements in the process model based upon the results of a specific element. These processes can be defined and documented using standards such as ISO9000 and IS17025. We can also measure the maturity of the HVA processes via a standard five level maturity model.
%%
%%
%%
%%
%%

\section{Threat Modelling and Threat Intelligence}
The goal of threat modelling is to define the set of capabilities associated with a specific threat actor. The type of threat actors that can be simulated in a HVA are depicted in Figure 3. All of the threat agents depicted in Figure 3 will have elements in common as well as elements that are unique. Each threat agent will also have a set inhibitors and amplifiers that directly impact on the likelihood of an attack.Threat agents can include: Nation States, Employees, Terrorists, Empowered Small Agents (ESA), Organised Crime and Corporations \\
\begin{figure}
\includegraphics[width=120mm]{Images/threat.png}
\centering
\label{Figure-3}
\caption{Threat Actors}
\end{figure}
\begin{itemize}
\item \textbf{Nation States}. \\
\begin{itemize}
\item These are groups of individuals, or organisations, resourced and backed by a nation state to achieve a particular objective. Due to the backing by a nation state these treat agents will be well resourced, well trained and well educated. Nation states are typically motivated by economic factors and focus on the theft of intellectual property.\\
\end{itemize}
\item \textbf{Employees}. \\
\begin{itemize}
\item These threat agents are individuals that work within an organisation and thus have physical and remote access to infrastructure of an organisation. Employees are typically motivated by Ideology, Ego or Revenge. They can also be coerced into performing actions via bribery or blackmail. \\
\end{itemize}
\item \textbf{Terrorists}. \\
\begin{itemize}
\item These threat agents are individuals or groups of individuals that seek to influence behaviour of a person, group of people or nation state via the creation terror through illegal acts. These types of threat agents are typically ideologically motivated and can be well resourced. \\
\end{itemize}
\item \textbf{Empowered Small Agents}. \\
\begin{itemize}
\item Empowered Small Agents is a broad group of threat agents covering the press, hacktivists and individual/groups of hackers. Their motivations motivations and capabilities will vary.\\
\end{itemize}
\item \textbf{Organised Crime}. \\
\begin{itemize}
\item This type of threat agent is concerned with making money and will typically focus on blackmailing an organisations to via the threat of publication of its intellectual property. To achieve their goals Organised Crime typically works through proxies such as employees via bribery or blackmail, and/or empowered small agents (EMA). Typically these types of threat agents are well motivated via financial rewards.\\
\end{itemize}
\item \textbf{Corporations}. \\
\begin{itemize}
\item These are commercial organisations that are motivated by economic forces and focus on the theft of intellectual property. To achieve their goals they can make use of employees via bribery or blackmail, and/or empowered small agents (EMA). Typically these types of threat agents are well financially resourced.
\end{itemize}
\end{itemize}

When specifying a Hardware Vulnerability Assessment (HVA) we need to define a set of threat actors that the assessment will simulate along with a set of capabilities for each simulated threat actor. When specifying the capabilities of a threat actor for a hardware vulnerability test there are a number of methods that we can use.   The simulated attacks for each threat actor are specified via an attack scenario and an attack tree. The attack scenario defines the goals, content and limitations of the attack while the attack graph specifies the attack in greater detail. As part of specifying the capabilities of a threat actor in an attack scenario we should also specify their:\\
\begin{itemize}
\item Limitations in terms of technical access, education and technical resources.\\
\item Actions that may amplify their willingness to perform an attack.\\
\item Inhibitors that may diminish the likelihood of an attack.\\
\end{itemize}
We can specify the actions of a threat agent by using a set of attack graph. This is a graphical representation of the steps that a threat actor would perform to achieve a desired impact. Attack graphs are charts that display the paths that attacks can take in a system. These charts display attack goals as a root with possible paths as branches to a desired outcome. When creating an attack graph for threat modelling, multiple graphs are created for a single system, one for each attacker goal. Attacks are very similar to fault trees used in the development and testing of safety critical systems - See Figure 4.\\
\begin{figure}[]
\includegraphics[width=100mm]{Images/ATTACKTREE.png}
\centering
\label{Figure-3}
\caption{Simple Attack Tree}
\end{figure}

In Figure 4 we can see that the goal $Modify Firmware$ is broken down into two sub-goals that are further decompose into three possible attack vectors. We can also make use of threat modelling method to represent the actions, and desired outcomes of an attack.The most common and well know threat modelling method is called STRIDE, and it standards for:
\begin{itemize}
\item \textbf{Spoofing}\\
\begin{itemize}
\item An attacker can spoof or impersonate a process, machine, electrical component or an electrical interface. When spoofing an electrical interface the attack is creating fake signals to elicit a response from an integrate circuit/device.\\
\end{itemize}
\item \textbf{Tampering}\\
\begin{itemize}
\item This involves modifying something on memory, disk, PCB, or somewhere else, which violates integrity. Example of tampering can include creating false access points on a PCB to allow for signals to be accessed.\\
\end{itemize}
\item \textbf{Repudiation}\\
\begin{itemize}
\item Repudiation involves claiming that you didn’t do something or were not involved or making it impossible to link an action back to you\\.
\end{itemize}
\item \textbf{Information Disclosure}\\
\begin{itemize}
\item This involves disclosing information to an authorised user. From a Hardware Vulnerability Assessment perspective this can include assessing the firmware via an SPI/JTAG interface or using a Debug Interface to access the internals of a core processor.\\
\end{itemize}
\item \textbf{Denial of Service}\\
\begin{itemize}
\item This involves exhausting resources required to offer services. For example, by pulling a input pin high or low is it possible to stop the embedded system from booting correctly.\\
\end{itemize}
\item \textbf{Escalation of Privileges}\\
\begin{itemize}
\item This involves allowing someone to do what they are unauthorised to do, which violates authorisation. For example, on an embedded system running a Real Time Operating System (RTOS, is it possible to boot the operating system into single user mode.\\
\end{itemize}
\end{itemize}
Other threat modelling methods includes Process for Attack Simulation and Threat Analysis (PASTA). ASTA is an attacker-centric methodology with seven steps. It is designed to correlate business objectives with technical requirements. PASTA’s steps guide teams to dynamically identify, count, and prioritise threats.\\
\begin{itemize}
\item Define business objectives.\\
\item Define the technical scope of assets and components.\\
\item Application decomposition and identify application controls.\\
\item Threat analysis based on threat intelligence.\\
\item Vulnerability detection.\\
\item Attack enumeration and modelling.\\
\item Risk analysis and development of countermeasures.\\
\end{itemize}
%%
%%
%%
%%
%%

\section{Tamper Resistance}
%%
%%
%%
%%
%%
To mitigate the actions of a threat agent a stakeholder will implement a set of counter-measures. While software counter measures include encryption, hardware based counter measures include tamper resistance. There are four basic types of tamper resistance:\\
\begin{itemize}
\item \textbf{Resistance}. The goal of tamper resistance is to ensure that any physical tampering is difficult. A side benefit of a good tamper resistance strategy is that it is often also tamper evident.\\
\item \textbf{Evidence}. The goal of tamper evidence as a resistance strategy is to ensure that any attempt to modify a device can be clearly seen. \\
\item \textbf{Detection}. The goal of tamper detection is to allow devices to be aware of tampering. This can include magnetic switches and pressure contacts as well as radiation sensors.\\
\item \textbf{Response}. The goal of tamper response is to allow devices to respond to an attack once it is detected. Types of response can include actions such as erasure and physical destruction.\\
\end{itemize}
%%
%%
%%
%%
%%

\section{Hardware Vulnerability Assessment}
As we can see in Figure 2 a Hardware Vulnerability Assessment consists of a set of distinct, but iterative, process elements. In this section we are going to explore each of these process elements in more detail. When conducting any test it is important that we recognise the difference between success and failure. To do this we need to ensure that all the tools and techniques we are going to use are correctly calibrated. From a scientific perspective it is this calibration that allows us to have confidence in our findings. Calibration allows us to identify the difference between success and failure when conducting a test. When performing a Hardware Vulnerability Assessment we need to understand that at each layer of abstraction there will be different interfaces that we can use for debugging.  These interfaces are placed there by the designers so that they can performing testing
\begin{itemize}
\item Chip/ASIC designers.\\
\item PCB/layout designers.\\
\item Embedded software developers.\\
\end{itemize}
Each layer of abstraction may require different debug interfaces. Each bringing their own nuances and common design practices that influence the physical layout and look of the device to be tested. From a hardware perspective we need to ensure that we have the following with known and documented outputs:
\begin{itemize}
\item Test board for UART. \\
\item Test Boards for SPI and I2C.\\
\item Test Boards for JTAG.\\
\item Test Boards for USB2 and USB3.\\
\item Test Boards for WiFi, RFIDI and ZigBee.\\
\item Software API interfaces into the firmware.\\
\end{itemize}
We also need to ensure that all software and manuals are kept patched and up-to-date. We should also have documented methods for testing the test boards to ensure that the software is functioning correctly and that the tests are traceable. It is critical that these documented tests define both success and failure conditions. In defining the calibration process a key standard that we can use is ISO 17025. The calibration process should also define all units of measures (volts, amps, etc) with reference to international standards.\\

\subsection{The Stakeholders}
The stakeholders are people and organisations responsible for defining and owning the requirements for the Hardware Vulnerability Assessment. They are also responsible for defining the acceptance criteria for the report and performing the evaluation/acceptance of the report. Stakeholders are responsible for defining the following:\\
\begin{itemize}
\item The aims, objectives and purpose of the Hardware Vulnerability Assessment.\\
\item The scope of the test (what is in bounds and out of bounds).\\
\item Time scales and costs of Hardware Vulnerability Assessment.\\
\item Identification of other key stakeholders.\\
\item List of deliverables and desired outcomes.\\
\item Target of evaluation of the Hardware Vulnerability Assessment.\\
\item Legal and Regulator requirements.\\
\item Capability statement for the threat agent/actor to be simulated.\\
\end{itemize}
These requirements are expressed in a language and form the scope of engagement for the test. All requirements are owned by stakeholders.\\

\subsection{Requirements}
\begin{quotation}
“\emph{If you cannot say what you mean, your Majesty you will never mean what you say and a gentleman should alaways mean what he says}” ― Peter O'Toole\\  
\end{quotation}

The requirements define the scope, scale and structure of the test. They function to define the type of test to be executed and how the test is to be conducted and reported, as well as the legal and ethical framework for the test. Scoping a penetration test should include the following activities:\\
\begin{itemize}
\item All relevant risk owners should outline any areas of special concern.\\
\item Technical boundaries and elements of the Target of Evaluation that are in/out-of scope.\\
\item Technical description of the threat actor's capabilities to be emulated during the test.\\
\item Reporting standards and nomenclature to be used for reporting/documenting vulnerabilities.\\
\end{itemize}

The requirements should also include a plan of action that defines the structure of the assessment. Key elements include:
\begin{itemize}
\item The technical boundaries of the assessment and the types of specific tests expected.\\
\item The timeframe and the amount of effort necessary to deliver the assessment.\\
\item Depending on the type of approach agreed, this document may also contain a number of scenarios or specific 'use cases' to test.\\
\item Any compliance or legislative requirements that the testing plan must meet.\\
\item Any specific reporting requirements.\\
\end{itemize}

When expressing the requirements care needs to be taken to ensure that the requirements is achievable and expressed in a common language. \\

While a common language allows for concepts to be expressed, it is the application of structure to the use of that language that allows for understanding to be developed and validated. Thus when expressing a requirement it is not sufficient to simply state the requirement, but rather we need to express how the requirement can be decomposed and ultimately measured. As we can see in Figure 5 each requirement should be associated with a test/metric.\\
\begin{figure}[]
\includegraphics[width=90mm]{Images/Requirement.png}
\centering
\label{Figure-5}
\caption{Structuring Requirements}
\end{figure}

When constructing a test it is important to notes that the test should be \textbf{SMART}:\\
\begin{itemize}
\item \textbf{Specific} - Well defined, clear, and unambiguous.\\
\item \textbf{Measurable} - With specific criteria that measure your progress toward the accomplishment of the goal.\\
\item \textbf{Achievable} - Attainable and not impossible to achieve.\\
\item \textbf{Realistic} -  Within reach, realistic, relevant to your project and reachable given the time and resources.\\
\item \textbf{Timely} - With a clearly defined timeline, including a starting date and a target date. The purpose is to create urgency.\\
\end{itemize}
\subsection{The Report}
The report documents the result of the security assessment from both a business and technical perspective. It will define the tests that were conducted and their results. It should be noted that no security assessment is ever complete; it is simply a set of tests and their documented results. It can never test for all possible vulnerabilities as this set is infinite. It is therefore critical that the stakeholder and the security assessor collaborate to define the scope and scale of the test. The test report should include:

\begin{itemize}
\item Any security issues and vulnerabilities uncovered during the execution of the attack scenarios.\\
\item An assessment by the test team as to the level of risk that each vulnerability exposes the target of evaluation (ToE) to.\\
\item A technical, social or legal method of resolving each issue found.\\
\item Advice on how to improve your internal vulnerability assessment process.\\
\end{itemize}
A debriefing can also be useful. At this meeting the test team run through their findings and you can request further information or clarification of any issues.\\

\subsection{Attack Surface Analysis}
The attack surface is the set of methods/tests that we can use to exploit items of the Target of Evaluation (ToE) during a Hardware Vulnerability Assessment (HVA). Typically these will be specified in the attack scenarios for a threat actor. For a HVA an attack surface can include the following:
\begin{itemize}
\item Printed Circuit Board (PCB) analysis.\\
\item Identification of all I/O points on the ToE.\\
\item Identification of all Test/Debug points on the ToE, such as JTAG, SPI, SWD, I2C etc.\\
\item Identification of all application interface points such as UART, WiFi, etc.\\
\item Identification of individual technical components, such as Integrated Circuits on the device to be tested i.e., The Target of Evaluation.\\
\item Reverse Engineering of extracted data from the Target of Evaluation.\\
\item Exploitation of software extracted from Target of Evaluation.\\
\end{itemize}
The analysis of the attack surface is the process of a) identifying what methods/tests are in scope for the test, b) what further information is required to facilitate the success of a methods/tests. For complex tests it can also include the definition of an attack tree. An attack tree functions to define the methods/tests that need to be performed to achieve a specific goal. 

\subsection{Open Source Intelligence and Analysis}
Open source analysis is the use of publicly available information sources to derive information about a specific subject/object. This information is derived from the synthesis, analysis and validation of data that is in the public domain. Key types of open source intelligence that we are looking for a technical documentation, and data-sheets that define the functionality of the protect and the components used to make the product. Types of Open Source information can include:
\begin{itemize}
\item User documentation provided with product.\\
\item The use of search engines.\\
\item Product review sites.\\
\item Product vendor site and suppler sites.\\
\item Data sheets on integrated circuits and other components.\\
\item Books and other online educational material.\\
\item Regulator and patent sites.\\
\end{itemize}
Other types of open source intelligence that are specifically useful for analysis of embedded systems include:
\begin{itemize}
\item Federal Communications Commission.\\
\begin{itemize}
\item https://apps.fcc.gov/oetcf/tcb/reports/TCBSearch.cfm\\
\end{itemize}
\item Chip and data sheet web sites such as https://www.findchips.com \\
\item Integrated Circuit Designers, such as\\
\begin{itemize}
\item ARM, intel, AMD.\\
\end{itemize}
\item Integrated Circuit Vendors/Manufactures\\
\begin{itemize}
\item NXP, intel, Micron, Toshiba\\
\item Winbond, Spartan, Broadcom\\
\item Texas Instruments, Samsung.\\
\end{itemize}
\item Search Engines such as Google, Yahoo, Bing, Ecosia, etc.\\
\item Security sites such as: CERT and UK-CERT, \\
\begin{itemize}
\item https://www.us-cert.gov\\
\end{itemize}
\item Patent information such as: patents.google.com \\
\item Academic Conference and Journals.\\
\begin{itemize}
\item ACM Digital Library - https://dl.acm.org\\
\item IEEExplore - https://ieeexplore.ieee.org\\
\item Elsivier E-Library - https://www.elsevier.com/en-gb/solutions/eLibrary\\
\item Springer - https://link.springer.com\\
\end{itemize}
\end{itemize}
The synthesis of information involves the fusion of data so as to prove, or disprove, a given hypothesis. Analysis of information so as to derive intelligence is the process of determining what information falls within scope and if that information has been validated. The validation of intelligence is typically done through experimentation. For example, Open Source Intelligence may tell us that a specific set of pins on an integrated circuit can be used for debugging via JTAG, but it is not until we try to use these pins for JTAG debugging that we know if that information is correct. We only know if the experiment is correct if we have calibrated it correctly so that we know what success and fail look like. 
\subsection{Exploitation}
Exploitation is the process of executing a specific test derived from the attack surface analysis. Prior to the execution of a test we will need to calibrate the test so as to understand the criteria for success or failure. The execution of the test may involve the following:
\begin{itemize}
\item Physical access to the Target of Evaluation so as to solder on test pins and then connect the test pins to an adaptor.\\
\item The  creation of a test rig where components are placed on a test PCB and then that test PCB is connected to the Target of Evaluation.\\
\item The use of protocols such as WiFi, RFID, ZigBee and TCP/IP to access the device.\\
\item Analysis of extract information, such searching for possible passwords from extracted firmware.\\
\item Removing components, such as Integrated Circuits, from the device and analysing them individually. This type of attack is often called a Chip-Off attack.\\
\item Exploitation of software interfaces on software executing on ToE.
\end{itemize}
Prior to the execution, during the execution and post execution of a test, detailed notes must be taken, analysed and retained for later reference. Also, each test must be structured along strict scientific principles so as to ensure reproducibility. Once we have completed a test we should reflect upon its results so as to see if further open source analysis is required. We should also link the results of the test into the attack surface analysis as the test's result may open up, or close down, areas of the attack surface. 
%%
%%
%%
%%
%%
\section{Standards}
When defining and implementing as process model for Hardware Vulnerability Assessments (HVA) there are a number of standards that we can make use of these include:
\begin{itemize}
\item \textbf{ISO 17025} is the general requirements for the competence of testing and calibration laboratories is the main ISO standard used by testing  laboratories. The key elements ISO 17025 are:\\
\begin{itemize}
\item \emph{Capacity}\\
\begin{itemize}
\item Is the concept that a laboratory has the resources (People with the required skills and knowledge, the Environment with the required facilities and equipment, the Quality Controls (Such as ISO 9000), and the Procedures \& Process Maturity) in order to undertake the work and produce competent results.\\
\end{itemize}
\item \emph{Exercise of Responsibility}\\
\begin{itemize}
\item Is the concept that persons in the organisation have the authority to execute specific functions within the overall scope of work – and that the organisation can demonstrate governance and responsibility for the results of the work.\\
\end{itemize}
\item \emph{Scientific Method}\\
\begin{itemize}
\item Is the concept that the work carried out by the organisation is based on accepted scientific approaches, preferably consensus-based, and that any deviations from accepted scientific approaches can be substantiated in a manner considered generally acceptable by experts in that field.\\
\end{itemize}
\item \emph{Objectivity of Measurement}\\
\begin{itemize}
\item Is the concept that the results produced within the scope of work of the organisation, are mainly based on internationally recognised measurable quantities.\\
\end{itemize}
\item \emph{Objectivity of Results}\\
\begin{itemize}
\item Is the concept that subjective test results are produced only by persons deemed qualified to do so and that such results are noted as being subjective, or are known by experts in that field of testing to be mainly subjective.\\
\end{itemize}
\item \emph{Impartiality of Conduct}\\
\begin{itemize}
\item Is the concept that the pursuit of competent results through the use of generally accepted scientific approaches is the primary and overriding influence on the work of persons executing tests - all other influences being considered secondary and not permitted to take precedence.\\
\end{itemize}
\item \emph{Traceability of Measurement}\\
\begin{itemize}
\item Is the concept that the results produced, within the scope of work of the laboratory, are based on a recognised system of measurement that derives from international accepted known standards of measurement.\\
\item Is the concept that the chain of comparison of measurement between these accepted known quantities and the device providing the objective result, is unbroken for the transfer of measurement characteristics for the whole of the measurement and analysis chain.\\
\end{itemize}
\item \emph{Repeatability of Test}\\
\begin{itemize}
\item Is the concept that the test which produced the objective results, will produce the same results, within accepted deviations during subsequent testing, and within the constraints of using the same procedures, equipment and persons used during a previous execution of the test.\\
\end{itemize}
\item \emph{Transparency of Process}\\
\begin{itemize}
\item Concept that the processes existent within the laboratory producing the objective results, are open to internal and external scrutiny, so that factors which may adversely affect the laboratory's pursuit of objective results based on scientific method, can be readily identified and mitigated.\\
\end{itemize}
\end{itemize}
\end{itemize}




\begin{itemize}
\item \textbf{ISO 9000} is defined as a set of international standards on quality management and quality assurance developed to help companies effectively document the quality system elements needed to maintain an efficient quality system. They are not specific to any one industry and can be applied to organisations of any size. Key elements of ISO 9000 are:\\
\begin{itemize}
\item \emph{Principle 1 – Customer Focus}\\
\begin{itemize}
\item Organisations depend on their customers and therefore should understand current and future customer needs, should meet customer requirements and strive to exceed customer expectations.\\
\end{itemize}
\item \emph{Principle 2 – Leadership}\\
\begin{itemize}
\item Leaders establish unity of purpose and direction of the organisation. They should create and maintain the internal environment in which people can become fully involved in achieving the organisation's objectives.\\
\end{itemize}
\item \emph{Principle 3 – Engagement of people}\\
\begin{itemize}
\item People at all levels are the essence of an organisation and their full involvement enables their abilities to be used for the organisation's benefit.\\
\end{itemize}
\item \emph{Principle 4 – Process Approach}\\
\begin{itemize}
\item A desired result is achieved more efficiently when activities and related resources are managed as a process.\\
\end{itemize}
\item \emph{Principle 5 – Improvement}\\
\begin{itemize}
\item Improvement of the organisation's overall performance should be a permanent objective of the organisation. This can be  linked into defined process maturity levels.\\
\end{itemize}
\item \emph{Principle 6 – Evidence-based decision making}\\
\begin{itemize}
\item Effective decisions are based on the analysis of data and information.\\
\end{itemize}
\item \emph{Principle 7 – Relationship Management}\\
\begin{itemize}
\item An organisation and its external providers (suppliers, contractors, service providers) are interdependent and a mutually beneficial relationship enhances the ability of both to create value.\\
\end{itemize}
\end{itemize}
\end{itemize}
%%
%%
%%
%%
%%
## Process Maturity
Process maturity for Hardware Vulnerability Assessment can be achieved via a Maturity Model:
* Level 1 – Initial}
  * At this level an organisation is using ad hoc methods for testing, so results are not repeatable and there is no quality standard.

* Level 2 – Definition
  * At this level testing is defined as a process, so there might be test strategies, test plans, test cases, based on requirements. Testing does not start until products are completed, so the aim of testing is to compare products against requirements.

* Level 3 – Integration
  * At this level testing is integrated into an Assessment cycle. The need for testing is based on risk management, and the testing is carried out with some independence from the development area.

* Level 4 – Management and Measurement
  * At this level testing activities take place at all stages of the life cycle, including reviews of requirements and designs. Quality criteria are agreed for all products of an organisation (internal and external).

* Level 5 – Optimization
  * At this level the testing process itself is tested and improved at each iteration. This is typically achieved with tool support, and also introduces aims such as defect prevention through the life cycle, rather than defect detection (zero defects).\\


## Summary and Conclusions
In this document we have sought to define what a Hardware Vulnerability Assessment (HVA) is and how we specify, execute and report upon it. The process the we have created to perform a Hardware Vulnerability Assessment is iterative in nature and seeks to allow the tester maximum flexibility when executing a HVA. The process also defines the role that stakeholder play along with key elements required when defining a Hardware Vulnerability Assessment.

## Contact Details
For further information and questions please contact Dr Andrew Blyth, PhD. <ajcblyth@snowcapcyber.com>
