Threat modeling Manifesto https://www.threatmodelingmanifesto.org/
- highlighting concerns about security, privacy and safety
- starting with thinking what can go wrong with our system
- Threat modeling is something everyone can do

  World shortest threat modeling course https://www.youtube.com/playlist?list=PLCVhBqLDKoOOZqKt74QI4pbDUnXSQo0nf
  - Four questions:
    1. What are we working on?
       - sketching
       - collaboration
       - data flow diagrams
       - learning about systems we are working on
    2.What can go wrong?
       - pay attention to answers
       - STRIDE model
3. What are we going to do about it?
   - tracking our work
   - develompent items
   - accept or transfer the risk
   - risk management
  
4. Did we do a good enough job?
   - would you recommend the threat modeling to colleague
  
       Darknet Diaries Podcast: EP 142 Axact
  - Very interesting episode
  - Talking about compant Axact that builds fake university websites and sell courses. The diplomas are fake and they are scamming people for money.
  - People worked with these diplomas, only line the company did have was not to sell medical diplomes since they can cause harm to people
  - Axact faced some lawsuits and 23 workers went to jail but not for too long.
  - The business never ended
  - Business owner has power and has connections so he is not in jail


   a) security hygiene
   - strong and different passwords for each site
   - two-Factor Authentication
   - not click on suspicios links
   - check where you put your info into
   - update softwares
   - data backup
   - locking devices

b) Threat model: LuxuryForAll

LuxuryForAll is a designer clothing rental company. Everyone can rent clothes and accesories through mobile app. We have everything for every occasion, whether it is for special event or just everyday wear.

1. What are we working on
   - customers personal and payment information
   - Inventory system
   - Mobile app platform
   - contracts with suppliers/customers
   - deliviery systems
  
   - customer trust, we need to have effortless bsuiness plan where customers can easily rent clothes with this we can ensure that customers comes back to use our services again
   - easy delivery/return process or pickup/dropout
   - customer support


2. What can go wrong?

Spoofing: Attack against customer or supplier to gain acces to information or accounts
Tampering: rental orders, inventory data, or payment details.
Repudiation: Customers or attackers could deny placing orders or making payment
Information Disclosure: access to personal, payment, or supplier contract information.
Denial of Service: disturbing access to mobile app
Elevation of Privilege: Gaining higher access within the system, potentially getting access to sensitive data or system functionality.

Largest risk:
Data breach of customers personal and payment info.
Could lead to identity theft, fraud, loss of customer trust and legal action

Cybercriminals: Interested in stealing personal and payment information for financial gain.

3. What are we going to do about it?
- Encrypting data
- strict access control
- updating the app
- firewall
- securing payment information
- only collect the minimum data needed
- backup systems
- multiple servers
- incident response plan
- eliminating unnecessary data
- accepting minor risks

4. Did we do good enough job?
   - regular security check-ins
   - penetration tests
   - updating the threat model
   - providing right training for employees
   - ask enough feedback from customers

