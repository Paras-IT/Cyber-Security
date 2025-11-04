# Task A - I have listen a podcast from darknetdiaries.com (espisode 103) and summarize as below:
- Fabio Viggiani, an Incident responder from Truesec company was asked to investigate a potential security breach at a large Swedish company.
- The Swedish Security Service informed the company that one of its servers was in communication with a known command-and-control (C2) server associated with a foreign state actor. The server in question was utilized as a jump server by a Managed Service Provider (MSP) to remotely oversee the company's infrastructure.
- Fabio requested a disk image and memory dump for the jump server. In a matter of minutes, he found thehostingoftheserver.mimikatz.hash, a file in the transient folder that proved credentials had been extracted using Mimikatz. The file contains around 100 plaintext login credentials, including Active Directory domain admin accounts.
- The finding led to a significant incident response, which included the creation of a war room and the participation of business leadership. The team began a forensic timeline analysis to establish a connection between file alterations and C2 communication periods. The malware used DLL side-loading to infiltrate reliable applications like Vba32 AntiRootkit Scanner. Malicious DLLs were in strange folders, including C:\Windows\Web, and loaded encrypted payloads into memory. Several instances of this method, each connecting to a distinct C2 server, were found over the period of several weeks.
- Memory analysis showed an odd, embedded message along with active malware: “Have your bosses given you the space to try to be a hacker? Come on man, don’t kill me.” This was probably a request or a taunt from the perpetrator. The attacker logged in via Remote Desktop using valid credentials; no exploit was utilized. This suggested that credentials had already been taken, either via Mimikatz or phishing. The infection has been active for over a month prior to its discovery.
- The attack was part of the Cloud Hopper campaign, which was executed by APT10, a Chinese state-sponsored group. Cloud Hopper targeted MSPs worldwide, using them as a doorway to the networks of their clients. The incident highlighted the risks associated with outsourcing IT infrastructure and the importance of monitoring third-party access.

# Task B - I have summarize this blog, https://www.schneier.com/blog/archives/2025/11/ai-summarization-optimization.html
- These days, AI systems record meetings and rank spoken material, turning the minutes into unbiased evidence. 
- Attendees speak early, reiterate ideas, and employ phrases like "key takeaway" and "action item" to influence what AI highlights in summaries. 
- Similar to search engine optimization, AISO modifies speech for algorithmic preferences, mirroring techniques used in LLM and generative engine optimization. 
- Identifying and preventing manipulation is the aim of organizational governance, social backlash, and technical countermeasures (such as prompt filtering and content sanitization).
- AISO subtly alters the dynamics of the workplace by providing strategic communicators with an edge and raising AI fluency to the level of an executive skill. 

# Task C - Here are some links that i found interesting
- https://www.researchgate.net/profile/Huiyao-Dong/publication/389138418_Cybersecurity_in_the_AI_era_analyzing_the_impact_of_machine_learning_on_intrusion_detection/links/67c74395461fb56424f10d43/Cybersecurity-in-the-AI-era-analyzing-the-impact-of-machine-learning-on-intrusion-detection.pdf
- https://darknetdiaries.com/episode/99/
- https://www.schneier.com/blog/archives/2025/10/first-wap-a-surveillance-computer-youve-never-heard-of.html
