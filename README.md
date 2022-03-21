 <h1>Flux set up at home hardware </h1>
 <br> Watch this <a href="https://youtu.be/jH-M3MAMTV8" target="_blank">Video</a> & set up your Flux Node &
 Make sure to <a href="http://bit.ly/Simplyeverythingcrypto" target="_blank">subscribe</a>
 <br> Note, you will need to have at least 100 confirmation on your collateral read Part 5.
 <br> <h3>Requirements</h3>
 <br> 1. At least 1,000 Flux to get started, Buy Flux on <a href="https://bit.ly/SignUpKucoinToday" target="_blank">Kucoin</a> or <a href="https://accounts.binance.com/en/register?ref=TQG402UF" target="_blank">Binance</a>
 <br> 2. Your own hardware depending on which tier you go for <a href="https://runonflux.io/flux-nodes.html" target="_blank">Read Here</a> / A VPS
 <br>--Hardware For Tiers
 <br>-Cumulus NUC - https://amzn.to/3trk1EC
 <br>-Nimbus NUC Barebone - https://amzn.to/3KXASVx 
 <br>-NUC 32gb Ram - https://amzn.to/3Ir04lu
 <br>-500GB NVMe - https://amzn.to/3JujZl5
 <br> <a href="https://home.runonflux.io/dashboard/economics" target="_blank">Check Out How Much You Can Make?</a>

<h2> Part 1 Getting Ubuntu Server</h2>
 <br>a. Download the <a href="https://ubuntu.com/download/server" target="_blank">latest ubuntu Server</a>
 <br>b. Wait 5mins ~ 60 mins depending on your internet speed.
 <br>c. After download is finish flash the downloaded ISO to a 16~32gb Thumbdrive / sd card using <a href="https://www.balena.io/etcher/" target="_blank">balenaEtcher</a>
 <br>d. Plug it into your hardware that you want to set the flux node on.
 <br>
 <br><h2>Part 2 Bios Settings </h2>
 <br>a. Depending on your motherboard
 <br>On keyboard press your BIOS key set by your manufacturer which could be <b>F10, F2, F12, F1, or DEL.</b> else, <a href="https://presearch.org/signup?rid=3735748" target="_blank">Presearch It</a>
 <br>b. You should search for <b>"Restore AC Power Loss"</b> which will be under Chipset / Advance / Power Management depending on how the manufacturer named it.
 Should look something like <a href="https://drive.google.com/file/d/1dqNsKvEd8qJWNWX48IEsu9Y08lgLYBlq/view?usp=sharing" target="_blank">this</a>
 <br>c. After enabling, On Bios go to <b>"Save & Exit"</b> <a href="https://drive.google.com/file/d/1vAOsOGmS53zlxy0QDAwn_KarKXmgoEJx/view?usp=sharing" target="_blank">[Reference]</a>
 <br> Save changes & select the your flashed SD Card / Thumbdrive on step "1c" under Boot Override. 
 
 <br><h2>Part 3 Setting Ubuntu Server Up</h2>
 <br>a. Select Install Ubuntu Server and wait
 <br>b. Select your langugage 
 <br>c. Select your keyboard layout 
 <br>d. Select your network, <b>If you're not connected via ethernet you might need to do this step.</b>
 <br>-If it's wireless select wlan <a href="https://drive.google.com/file/d/13vZlen7zu3luiGvFFy6huE6l7IIdefvs/view?usp=sharing" target="_blank">[Reference]</a> & edit WiFi then select choose a visible network & enter your wifi password.
 <br>e. Configure Proxy, Just leave blank and select <b>"Done".</b>
 <br>f. Configure Ubuntu archive Mirror, leave it as default and select <b>"Done".</b>
 <br>g. Guided Storage Configuration
 <br><b>Important</b>, Unselect "Set Up this disk as an LVM group" & select <b>"Done".</b> <a href="https://drive.google.com/file/d/1jNh_tSOvw2VvCtbO8WD_c-JG7CKnP00o/view?usp=sharing" target="_blank">[Reference]</a>
 <br>h. Storage configuration - Leave it as default and select <b>"Done".</b> Then confirm destrutive action "<b>"Continue".</b>
 <br>i. Profile Setup - Fill up the details 
<br>-Your name = just ur profile name on the linux server not username.
<br>-Server's name = is how you want the server to be called, will be shown on your router as input. 
<br>-Username = to use when logging into the server
<br>-Password = to log into the server.
<br>j. SSH Setup enable "Install OpenSSH server" & <b>"Done".</b>
<br>k. Featured Server Snaps leave it as default & <b>"Done".</b>
<br><b>Finally Install complete!</b>
<br>-You will see <b>"Cancel update and reboot"</b> but wait till you see <b>"Reboot Now"</b> option and select it
<br>-Once reboot you will see <b>"[FAILED] Failed unmounting/cdrom. blah blah blah.</b> 
<br>-Just unplug your flash drive you did on "2d." then press enter on keyboard & let it load till you see the login page.
<br>L. enter the username & password done on step "3i." 
<br><h3>Option Steps for web view & terminal for easy install of Flux Node</h3>
<br>a. Copy down the IPv4 password shown on the page after login.
<br>b. type in <b>"sudo apt install cockpit"</b> & enter your password on step "3L." then wait for it to complete installing.

<h2>Part 4 Router Portforwarding / DMZ</h2>
<br>a. Log in to your router
<br>b. Search For DHCP Server / Reservation Under "Lan" mostly depending on your router manufacturer.
Search for your Hardware Mac Address on your router and assign them the default IP given.
<br>c. If Portforward range use this
<br>-Port 16124 - 16128 | TCP & UDP | Your Device IP
<br>-Port 30000 - 39999 | TCP & UDP | Your Device IP
<br>d. If DMZ
<br>-Enable DMZ on router and enter the IP of your device.
<br>
 <br><h2>Part 5 Installing Flux Node! </h2>
 
 <br>a. If you installed cockpit on optional step you can just login by entering the IPv4 you copied on step "Option Steps a." on browser with :9090 e.g "192.168.1.241:9090" and login else go to "5b."
 <br>b. Go to ZelCore wallet | <a href="https://zelcore.io/" target="_blank">[Download]</a> if you haven't
 <br>c. Send fund of 1,000 / 12,500 / 40,000 Flux exactly in a Single Transaction for collateral to either wallet shown on ZelCore and wait for 100 confirmations. 
 <br> If you send funds via exchanges, funds will not be exactly due to the fees they charge or send to many address, You have to an internal transfer from your ZelCore Wallet to another internally.
 <br> On ZelCore select the wallet you sent Flux to and choose <b>Flux</b> > Menu page <b>"More"</b> > Select <b>FluxNodes.</b> 
 <br>d. you will see under <b>"My FluxNodes"</b> the node will show the tier depending on how much Flux you sent on a single transaction for collateral. Open it up and select <b>"edit"</b>, You will find the Identity Key, Collateral TX ID & Output Index, remember this step you will need them. 
 <br>e. Go back to your server / web terminal and type in <b>"sudo apt install  npm -y"</b> and wait.
 <br>f. Type <b>"sudo su"</b> enter password if needed.
 <br>g. Enter command <b>"bash -i <(curl -s https://raw.githubusercontent.com/RunOnFlux/fluxnode-multitool/master/multitoolbox.sh)"</b>
 <br>h. Install Docker by selecting option 1 and "Enter" then input the username you used to set up the server on Part 3i.
 <br> After installing docker it will prompt you "Would you like to switch account" choose yes by entering "y".
 <br>i. Enter command <b>"bash -i <(curl -s https://raw.githubusercontent.com/RunOnFlux/fluxnode-multitool/master/multitoolbox.sh)"</b>
 <br>j. Install FluxNode by selecting option 2 & wait.
 <br> -You might be prompted "Detected you are using 22 for SSH is this correct?" Select "yes" if prompted else skip this.
 <br> -You will be prompted to enter your FluxNode PrivKey Generated by your Zelcore go back to "5d." to retrieve and paste it and select "ok"
 <br> -You will be asked for FluxNode Collateral txid go to "5d." retreive and paste it and select "ok"
 <br> -You will be asked for FluxNode Collateral Output index, go to 5d. retrieve it and paste it and select "ok"
 <br> -You will be asked to download bootstrap file, Select option "1" and select "ok" wait for 10 ~ 120 mins depending on your internet speed.
 <br> -After the bootstrap file is installed you will be prompted to "remove bootstrap archive file?" Just select "Yes" and go to your ZEL ID from ZelCore(Apps -> Zel ID (Click QR Code)) and paste the copied QR Code and click "ok"
 <br> -If you are nimbus and above you will be prompted to enter Kadena address, find it on your ZelCore that Account starting with K not Public key.
 <br> -If you are nimbus and above you will be prompted to enter your Kadena chainid, enter "0" and select "ok" 
 <br> --Optional you will be prompted asking if you would like to "enable alert?" Select Yes or No and fill in the details if you selected yes, for this guide it will be "no".
 <br> -Countinue waiting until you see <a href="https://drive.google.com/file/d/1_mFy7_DYg6uoBIIGiOqtzmOjjduMwyFL/view?usp=sharing" target="_blank">[This]</a> Copy the IP shown highlighed in red.
 <br>k. Go to your zelcore wallet and find your fluxnode ref "5d." edit your FluxNode and enter the public IP you copied and <br>"start"</br> your fluxnode
 <h3>-Congrats you are running your fluxnode!</h3>
 
 <br>--Optional step for those who enable the web interface on Part3 After L. 
 <br> -on terminal enter <b>"sudo ufw enable"</b>
 <br> -enter <b>"sudo ufw allow 9090"</b>
 <br> -to check if it's allowed type <b>"sudo ufw status"</b>
 
 <br><br>
 <br>Feel free to some milk powder on Flux - "t1fM5bjG4ximyDgAhRnFmqf8zhQ7xfBwanh"
 <br>Or you wan 
 via BSC/ETH/Polygon - "0xE9E129aD58108B99c432AB00A92a82fC68bc2a90"
 <br>Or some digital gold BTC - "35qUZ5urRiVqJRvj8CuAN3cMxNMurFvHz3"
