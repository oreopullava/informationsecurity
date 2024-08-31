<h1>Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains</h1>
https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf

- traditional methods address only known vulnerabilities and reacts only after attack -> not really affective against ATPs
- ATPs =  Advanced Persistent Threats
- ATPs are highly skilled attackers that attacks sensitive information 
- using kill chain model to anticipate, detect, and disrupt 

- military operations (find, fix, track, target, engage, assess)
- models are adapted in information security, such as the ABSAC framework, which aligns countermeasures to attack phases
- exploitation life cycle” focuses on post-compromise actions but is lacking early defensive strategies, that are crucial when thinking about ATPs

- Intelligence-Driven CND focuses on understanding attackers and their behavior to create a defense. Viewed as a series of phases, and disrupting any phase in the "kill chain" can stop the attacker.
Indicators:
- Atomic: basic details like IP addresses
- Computed: Data derived from incidents
- Behavioral: Patterns combining different clues
-  Indicators are constantly analyzed and updated to improve defense

  <h4>Intrusion kill chain</h4>
1. Reconnaissance: Attacker gathers info on targets
2. Weaponization: Prepares the attack (creating malware)
3. Delivery: Sends the attack (email, website, USB)
4. Exploitation: Attack is triggered (exploits a vulnerability)
5. Installation: Installs malware to maintain access
6. Command and Control: Attacker gains control of the system
7. Actions on Objectives: Attacker achieves their goals

- intrusion kill chain helps defenders create actionable intelligence by matching their security measures with the steps attackers use to target their organization.
- course of action matrix utilize actions like detect, deny, disrupt, degrade, deceive, and destroy from DoD doctrine to address different phases of an attack, incorporating tools like HIDS, NIDS, and firewall ACLs
- Defender Resiliency focuses on building resiliency by using available indicators to force adversaries to make adjustments, rather than solely focusing on zero-day exploits
- track defensive performance with metrics, showing how defenses react to multiple intrusion attempts
- Defensive Adaptation, continuously update and layer defenses

 
  - Kill chain analysis is a guide for analysts to understand what information is
  - To mitigate future attacks, defenders must analyze and understand all phases not just the current one
  - Analyzing multiple intrusion kill chains over time helps spot shared indicators and patterns
  - By understanding repeated tactics defenders can reduce the likelihood of successful attacks over time.
    
  



*
*
*
*
*
*
*
*
*
*






<h1>Installing Debian</h1>

First step was to install current Debian ISO image. I found them in https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/
After I found the correct one I started the downloading.

<img width="936" alt="image" src="https://github.com/user-attachments/assets/ca77a476-ac48-4bee-8810-b05f6bd94fc6">

The correct way to choose the right image was by these rules:

- live - Can boot from image and use Linux even without installing. Some Linux distributions call live images desktop images.
- 12.x.x - The distribution version, which locks major versions of most software, while providing security updates.
- amd64 - Most regular desktops, laptops and servers are amd64. Also Intel processors use amd64 architecture.
- xfce - my favourite desktop environment. Obvious and simple, but also easy to configure if you want. The other ones work fine, too.
  rules taken from https://terokarvinen.com/2021/install-debian-on-virtualbox/


After that I had to download the VirtualBox since I didn't have it beforehand. I found it easily from here: https://www.virtualbox.org/wiki/Downloads
<img width="395" alt="image" src="https://github.com/user-attachments/assets/922cd35b-871a-484a-a0cb-66835f5b1b2f">
<img width="542" alt="image" src="https://github.com/user-attachments/assets/475941f6-094d-4a0f-ab2a-b1d7ced3e9e8">

Now that I had downloaded the VirtualBox. I had to set it up. After that it opened the VirtualBox manager. There I had to create a new Virtual Machine with these steps:
1. Machine -> new
2. Named the machine
3. Changed the memory to 4000 MB
4. Created a new virtual hard disk, sized 60 GB
5. "Create"

Now that I had my Virtual Machine created I had to insert my Debian ISO image that I had downloaded earlier. It was quick with these steps:
1. Settings
2. Storage
3. Under Controller IDE choose "EMPTY"
4. "Optical Drive" then open the menu
5. Selected the ISO disk image



this should be the outcome:



<img width="671" alt="image" src="https://github.com/user-attachments/assets/a75af958-bb87-44a0-a2e1-6953e380a503">



Then I booted the machine
<img width="331" alt="image" src="https://github.com/user-attachments/assets/cee4fc8e-471b-4ac0-8405-dc60b551f4be">
<img width="401" alt="image" src="https://github.com/user-attachments/assets/211f1468-83e1-4db8-925c-7967e809865d">



For me to test mouse, keyboard, network and display I opened Firefox 
<img width="397" alt="image" src="https://github.com/user-attachments/assets/2fbcb063-52c6-4af9-a7cb-6d9ceb9e89c4">

<h3>Running the installer</h3>

In the desktop there was "Install Debian" that I clicked. For me to install it I had to go through these steps first:
1. Change the language to American English
2. Set my location to Finland
3. Choose the keyboard (Finnish)
4. Erase disk
5. Did not encrypt
6. Fill in user info, my name, log in name, naming computer and set a strong password
7. Then clicked install


   <img width="398" alt="image" src="https://github.com/user-attachments/assets/6a5c8498-b324-4218-8399-503302a2d187">


   Then it rebooted and I was greeted with log in screen. In the steps before I had to create log in name and password so they were the ones I used for log in. After I was in I opened the Firefox to test everything works just fine. Then I opened Applications: Terminal Emulator. I wrote the command "sudo apt-get update" to update and then put another command "sudo apt-get -y dist-upgrade" for it to upgrade everything. It took a few minutes. Here is photo below of the upgrade process:

   <img width="398" alt="image" src="https://github.com/user-attachments/assets/87f6be45-2d57-44f5-967c-7ccdf94a6ca5">


Then I had to install a firewall and turn it on with these commands "sudo apt-get -y install ufw" "sudo ufw enable"
Now we had to restart and log in again, and we were all set!


