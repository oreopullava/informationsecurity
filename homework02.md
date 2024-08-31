<h1>Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains</h1>








<h1>Installing debian</h1>

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







