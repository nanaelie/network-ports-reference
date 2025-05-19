
# What Are TCP and UDP Ports Used For?

TCP and UDP protocols enable communication between two devices over the Internet or a network. To properly deliver data, the system uses ports, which are digital “entry points” identified by numbers ranging from 0 to 65,535.

# How Ports Work:

Each data packet contains two port numbers: one for the sender and one for the receiver.

The operating system dynamically opens ports to route data to the appropriate application.

Port numbers help the system identify which program should receive the incoming data.

## Types of Ports:

- Well-known ports (0–1023): Reserved for standardized services (e.g., HTTP, FTP, SSH).
- Registered ports (1024–49151): Assigned to applications by organizations or developers via the IANA.
- Dynamic/private ports (49152–65535): Temporarily used by applications (e.g., web browsers during a session).

## Note:

Some ports are dedicated to either TCP or UDP, while others can be used for both. A few ports, although not officially registered, have become widely adopted as de facto standards.

---

# Well-known ports

<table>
    <thead>
        <tr>
            <th>Port</th>
            <th>TCP</th>
            <th>UDP</th>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead> 
    <tbody> 
        <tr>
            <td>1</td>
            <td>true</td> 
            <td>true</td>
            <td>tcpmux</td>
            <td>TCP Port Multiplexer (service de multiplexage de TCP port)</td>
        </tr> 
        <tr>
            <td>5</td>
            <td>true</td>
			<td>true</td>
			<td> rje </td>
			<td> Remote Job Entry (saisie de tâche à distance) </td>
		</tr>
		<tr>
			<td> 7 </td>
			<td>true</td>
			<td>true</td>
			<td> echo </td>
			<td> Service d’écho </td>
		</tr>
		<tr>
			<td> 9 </td>
			<td>true</td>
			<td>true</td>
			<td> discard </td>
			<td> Service zéro à des fins de test </td>
		</tr>
		<tr>
			<td> 11 </td>
			<td>true</td>
			<td>true</td>
			<td> systat </td>
			<td> Informations système </td>
		</tr>
		<tr>
			<td> 13 </td>
			<td>true</td>
			<td>true</td>
			<td> daytime </td>
			<td> Saisie de la date et de l’heure </td>
		</tr>
		<tr>
			<td> 17 </td>
			<td>true</td>
			<td>true</td>
			<td> qotd </td>
			<td> Envoie la citation du jour </td>
		</tr>
		<tr>
			<td> 18 </td>
			<td>true</td>
			<td>true</td>
			<td> msp </td>
			<td> Transfère des SMS </td>
		</tr>
		<tr>
			<td> 19 </td>
			<td>true</td>
			<td>true</td>
			<td> chargen </td>
			<td> Envoie une séquence de caractères infinie </td>
		</tr>
		<tr>
			<td> 20 </td>
			<td>true</td>
			<td>false</td>
			<td> ftp-data </td>
			<td> Transmission de données&nbsp;FTP </td>
		</tr>
		<tr>
			<td> 21 </td>
			<td>true</td>
			<td>true</td>
			<td> ftp </td>
			<td> Connexion&nbsp;FTP </td>
		</tr>
		<tr>
			<td> 22 </td>
			<td>true</td>
			<td>true</td>
			<td> ssh </td>
			<td> Service Secure Shell </td>
		</tr>
		<tr>
			<td> 23 </td>
			<td>true</td>
			<td>false</td>
			<td> telnet </td>
			<td> Service Telnet </td>
		</tr>
		<tr>
			<td> 25 </td>
			<td>true</td>
			<td>false</td>
			<td> smtp </td>
			<td> Simple Mail Transfer Protocol (protocole simple de transfert de courrier) </td>
		</tr>
		<tr>
			<td> 37 </td>
			<td>true</td>
			<td>true</td>
			<td> time </td>
			<td> Protocole temporel lisible par un ordinateur </td>
		</tr>
		<tr>
			<td> 39 </td>
			<td>true</td>
			<td>true</td>
			<td> rlp </td>
			<td> Resource Location Protocol (protocole de localisation des ressources) </td>
		</tr>
		<tr>
			<td> 42 </td>
			<td>true</td>
			<td>true</td>
			<td> nameserver </td>
			<td> Service de noms </td>
		</tr>
		<tr>
			<td> 43 </td>
			<td>true</td>
			<td>false</td>
			<td> nicname </td>
			<td> Service d’annuaire&nbsp;WHOIS </td>
		</tr>
		<tr>
			<td> 49 </td>
			<td>true</td>
			<td>true</td>
			<td> tacacs </td>
			<td> Terminal Access Controller Access Control System (protocole d’authentification à distance) </td>
		</tr>
		<tr>
			<td> 50 </td>
			<td>true</td>
			<td>true</td>
			<td> re-mail-ck </td>
			<td> Remote Mail Checking (consultation de messagerie à distance) </td>
		</tr>
		<tr>
			<td> 53 </td>
			<td>true</td>
			<td>true</td>
			<td> domain </td>
			<td> Résolution de nom par DNS </td>
		</tr>
		<tr>
			<td> 67 </td>
			<td>false</td>
			<td>true</td>
			<td> bootps </td>
			<td> Services Bootstrap Protocol </td>
		</tr>
		<tr>
			<td> 68 </td>
			<td>false</td>
			<td>true</td>
			<td> bootpc </td>
			<td> Bootstrap Client </td>
		</tr>
		<tr>
			<td> 69 </td>
			<td>false</td>
			<td>true</td>
			<td> tftp </td>
			<td> Trivial File Transfer Protocol (protocole simplifié de transfert de fichiers) </td>
		</tr>
		<tr>
			<td> 70 </td>
			<td>true</td>
			<td>false</td>
			<td> gopher </td>
			<td> Recherche de document </td>
		</tr>
		<tr>
			<td> 71 </td>
			<td>true</td>
			<td>false</td>
			<td> genius </td>
			<td> Protocole&nbsp;Genius </td>
		</tr>
		<tr>
			<td> 79 </td>
			<td>true</td>
			<td>false</td>
			<td> finger </td>
			<td> Transmet les coordonnées des utilisateurs </td>
		</tr>
		<tr>
			<td> 80 </td>
			<td>true</td>
			<td>false</td>
			<td> http </td>
			<td> Hypertext Transfer Protocol (protocole de transfert hypertexte) </td>
		</tr>
		<tr>
			<td> 81 </td>
			<td>true</td>
			<td>false</td>
			<td>false</td>
			<td> Torpark&nbsp;: Onion-Routing (non officiel - routage en oignon) </td>
		</tr>
		<tr>
			<td> 82 </td>
			<td>false</td>
			<td>true</td>
			<td>false</td>
			<td> Torpark&nbsp;: Control (non officiel) </td>
		</tr>
		<tr>
			<td> 88 </td>
			<td>true</td>
			<td>true</td>
			<td> kerberos </td>
			<td> Système d’authentification de réseau </td>
		</tr>
		<tr>
			<td> 101 </td>
			<td>true</td>
			<td>false</td>
			<td> hostname </td>
			<td> NIC Host Name (nom d’hôte&nbsp;NIC) </td>
		</tr>
		<tr>
			<td> 102 </td>
			<td>true</td>
			<td>false</td>
			<td> Iso-tsap </td>
			<td> ISO-TSAP-Protocol (protocole&nbsp;ISO&nbsp;TSAP) </td>
		</tr>
		<tr>
			<td> 105 </td>
			<td>true</td>
			<td>true</td>
			<td> csnet-ns </td>
			<td> Mailbox-Mailserver (serveur de messagerie électronique) </td>
		</tr>
		<tr>
			<td> 107 </td>
			<td>true</td>
			<td>false</td>
			<td> rtelnet </td>
			<td> Remote Telnet (Telnet à distance) </td>
		</tr>
		<tr>
			<td> 109 </td>
			<td>true</td>
			<td>false</td>
			<td> pop2 </td>
			<td> Post Office Protocol v2 (protocole de bureau de poste&nbsp;v2) pour la communication par e-mail </td>
		</tr>
		<tr>
			<td> 110 </td>
			<td>true</td>
			<td>false</td>
			<td> pop3 </td>
			<td> Post Office Protocol v3 (protocole de bureau de poste&nbsp;v3) pour la communication par e-mail </td>
		</tr>
		<tr>
			<td> 111 </td>
			<td>true</td>
			<td>true</td>
			<td> sunrpc </td>
			<td> Protocole&nbsp;RPC pour NFS </td>
		</tr>
		<tr>
			<td> 113 </td>
			<td>false</td>
			<td>true</td>
			<td> auth </td>
			<td> Service d’authentification </td>
		</tr>
		<tr>
			<td> 115 </td>
			<td>true</td>
			<td>false</td>
			<td> sftp </td>
			<td> Simple File Transfer Protocol (version simplifiée de FTP) </td>
		</tr>
		<tr>
			<td> 117 </td>
			<td>true</td>
			<td>false</td>
			<td> uucp-path </td>
			<td> Transmission de fichiers entre systèmes&nbsp;Unix </td>
		</tr>
		<tr>
			<td> 119 </td>
			<td>true</td>
			<td>false</td>
			<td> nntp </td>
			<td> Transmission de fichiers au sein de groupes de discussion </td>
		</tr>
		<tr>
			<td> 123 </td>
			<td>false</td>
			<td>true</td>
			<td> ntp </td>
			<td> Service de synchronisation temporelle </td>
		</tr>
		<tr>
			<td> 137 </td>
			<td>true</td>
			<td>true</td>
			<td> netbios-ns </td>
			<td> Service de noms&nbsp;NETBIOS </td>
		</tr>
		<tr>
			<td> 138 </td>
			<td>true</td>
			<td>true</td>
			<td> netbios-dgm </td>
			<td> NETBIOS Datagram Service (service de datagramme&nbsp;NETBIOS) </td>
		</tr>
		<tr>
			<td> 139 </td>
			<td>true</td>
			<td>true</td>
			<td> netbios-ssn </td>
			<td> NETBIOS Session Service (service de session&nbsp;NETBIOS) </td>
		</tr>
		<tr>
			<td> 143 </td>
			<td>true</td>
			<td>true</td>
			<td> imap </td>
			<td> Internet Message Access Protocol (protocole d’accès aux messages électroniques) pour communication par e-mail </td>
		</tr>
		<tr>
			<td> 161 </td>
			<td>false</td>
			<td>true</td>
			<td> snmp </td>
			<td> Simple Network Management Protocol (protocole simple de gestion de réseau) </td>
		</tr>
		<tr>
			<td> 162 </td>
			<td>true</td>
			<td>true</td>
			<td> snmptrap </td>
			<td> Simple Network Management Protocol Trap (Trap de protocole simple de gestion de réseau) </td>
		</tr>
		<tr>
			<td> 177 </td>
			<td>true</td>
			<td>true</td>
			<td> xdmcp </td>
			<td> X Display Manager (gestionnaire d’affichage&nbsp;X) </td>
		</tr>
		<tr>
			<td> 179 </td>
			<td>true</td>
			<td>false</td>
			<td> bgp </td>
			<td> Border Gateway Protocol (protocole d’échange de route) </td>
		</tr>
		<tr>
			<td> 194 </td>
			<td>true</td>
			<td>true</td>
			<td> irc </td>
			<td> Internet Relay Chat (discussion relayée par Internet) </td>
		</tr>
		<tr>
			<td> 199 </td>
			<td>true</td>
			<td>true</td>
			<td> smux </td>
			<td> SNMP UNIX Multiplexer (service de multiplexage&nbsp;UNIX&nbsp;SNMP) </td>
		</tr>
		<tr>
			<td> 201 </td>
			<td>true</td>
			<td>true</td>
			<td> at-rtmp </td>
			<td> AppleTalk Routing (routage d’AppleTalk) </td>
		</tr>
		<tr>
			<td> 209 </td>
			<td>true</td>
			<td>true</td>
			<td> qmtp </td>
			<td> Quick Mail Transfer Protocol (protocole de transfert de courrier rapide) </td>
		</tr>
		<tr>
			<td> 210 </td>
			<td>true</td>
			<td>true</td>
			<td> z39.50 </td>
			<td> Système d’informations bibliographiques </td>
		</tr>
		<tr>
			<td> 213 </td>
			<td>true</td>
			<td>true</td>
			<td> ipx </td>
			<td> Internetwork Packet Exchange </td>
		</tr>
		<tr>
			<td> 220 </td>
			<td>true</td>
			<td>true</td>
			<td> imap3 </td>
			<td> IMAP&nbsp;v3 pour la communication par e-mail </td>
		</tr>
		<tr>
			<td> 369 </td>
			<td>true</td>
			<td>true</td>
			<td> rpc2portmap </td>
			<td> Coda Filesystem Portmapper (portmapper de systèmes de fichiers&nbsp;Coda) </td>
		</tr>
		<tr>
			<td> 370 </td>
			<td>true</td>
			<td>true</td>
			<td> codaauth2 </td>
			<td> Coda Filesystem Authentication Service (service d’authentification de systèmes de fichiers&nbsp;Coda) </td>
		</tr>
		<tr>
			<td> 389 </td>
			<td>true</td>
			<td>true</td>
			<td> ldap </td>
			<td> Lightweight Directory Access Protocol (protocole&nbsp;DAP version allégée) </td>
		</tr>
		<tr>
			<td> 427 </td>
			<td>true</td>
			<td>true</td>
			<td> svrloc </td>
			<td> Service Location Protocol (protocole de découverte de services) </td>
		</tr>
		<tr>
			<td> 443 </td>
			<td>true</td>
			<td>false</td>
			<td> https </td>
			<td> HTTPS (HTTP via SSL/TLS) </td>
		</tr>
		<tr>
			<td> 444 </td>
			<td>true</td>
			<td>true</td>
			<td> snpp </td>
			<td> Simple Network Paging Protocol (protocole simple d’appel de réseau) </td>
		</tr>
		<tr>
			<td> 445 </td>
			<td>true</td>
			<td>false</td>
			<td> microsoft-ds </td>
			<td> SMB via TCP/IP </td>
		</tr>
		<tr>
			<td> 464 </td>
			<td>true</td>
			<td>true</td>
			<td> kpasswd </td>
			<td> Modification de mot de passe pour Kerberos </td>
		</tr>
		<tr>
			<td> 500 </td>
			<td>false</td>
			<td>true</td>
			<td> isakmp </td>
			<td> Protocole de sécurité </td>
		</tr>
		<tr>
			<td> 512 </td>
			<td>true</td>
			<td>false</td>
			<td> exec </td>
			<td> Remote Process Execution (exécution de processus à distance) </td>
		</tr>
		<tr>
			<td> 512 </td>
			<td>false</td>
			<td>true</td>
			<td> comsat/biff </td>
			<td> Client et serveur de messagerie </td>
		</tr>
		<tr>
			<td> 513 </td>
			<td>true</td>
			<td>false</td>
			<td> login </td>
			<td> Connexion à l’ordinateur à distance </td>
		</tr>
		<tr>
			<td> 513 </td>
			<td>false</td>
			<td>true</td>
			<td> who </td>
			<td> Whod User Logging Daemon </td>
		</tr>
		<tr>
			<td> 514 </td>
			<td>true</td>
			<td>false</td>
			<td> shell </td>
			<td> Remote Shell </td>
		</tr>
		<tr>
			<td> 514 </td>
			<td>false</td>
			<td>true</td>
			<td> syslog </td>
			<td> Unix System Logging Service (service de connexion au système&nbsp;Unix) </td>
		</tr>
		<tr>
			<td> 515 </td>
			<td>true</td>
			<td>false</td>
			<td> printer </td>
			<td> Services d’impression&nbsp;: Line Printer Daemon </td>
		</tr>
		<tr>
			<td> 517 </td>
			<td>false</td>
			<td>true</td>
			<td> talk </td>
			<td> Talk Remote Calling (appel à distance) </td>
		</tr>
		<tr>
			<td> 518 </td>
			<td>false</td>
			<td>true</td>
			<td> ntalk </td>
			<td> Network Talk (discussion en réseau) </td>
		</tr>
		<tr>
			<td> 520 </td>
			<td>true</td>
			<td>false</td>
			<td> efs </td>
			<td> Extended Filename Server (serveur de noms de fichiers étendu) </td>
		</tr>
		<tr>
			<td> 520 </td>
			<td>false</td>
			<td>true</td>
			<td> router </td>
			<td> Routing Information Protocol (protocole d’information de routage) </td>
		</tr>
		<tr>
			<td> 521 </td>
			<td>false</td>
			<td>true</td>
			<td> ripng </td>
			<td> Routing Information Protocol (protocole d’information de routage) pour IPv6 </td>
		</tr>
		<tr>
			<td> 525 </td>
			<td>false</td>
			<td>true</td>
			<td> timed </td>
			<td> Serveur de temps </td>
		</tr>
		<tr>
			<td> 530 </td>
			<td>true</td>
			<td>true</td>
			<td> courier </td>
			<td> Courier Remote Procedure Call (appel de procédure à distance&nbsp;Courier) </td>
		</tr>
		<tr>
			<td> 531 </td>
			<td>true</td>
			<td>true</td>
			<td> conference </td>
			<td> Discussion via AIM et IRC </td>
		</tr>
		<tr>
			<td> 532 </td>
			<td>true</td>
			<td>false</td>
			<td> netnews </td>
			<td> Netnews Newsgroup Service (service d’actualités&nbsp;Netnews) </td>
		</tr>
		<tr>
			<td> 533 </td>
			<td>false</td>
			<td>true</td>
			<td> netwall </td>
			<td> Diffusions d’urgence </td>
		</tr>
		<tr>
			<td> 540 </td>
			<td>true</td>
			<td>false</td>
			<td> uucp </td>
			<td> Unix-to-Unix Copy Protocol (protocole de copie&nbsp;Unix vers Unix) </td>
		</tr>
		<tr>
			<td> 543 </td>
			<td>true</td>
			<td>false</td>
			<td> klogin </td>
			<td> Kerberos v5 Remote Login (connexion à distance&nbsp;Kerberos&nbsp;v5) </td>
		</tr>
		<tr>
			<td> 544 </td>
			<td>true</td>
			<td>false</td>
			<td> kshell </td>
			<td> Kerberos v5 Remote Shell (Shell à distance&nbsp;Kerberos&nbsp;v5) </td>
		</tr>
		<tr>
			<td> 546 </td>
			<td>true</td>
			<td>true</td>
			<td> dhcpv6-client </td>
			<td> DHCP v6 Client </td>
		</tr>
		<tr>
			<td> 547 </td>
			<td>true</td>
			<td>true</td>
			<td> dhcpv6-server </td>
			<td> DHCP v6 Server </td>
		</tr>
		<tr>
			<td> 548 </td>
			<td>true</td>
			<td>false</td>
			<td> afpovertcp </td>
			<td> Apple Filing Protocol (protocole&nbsp;AppleShare) via TCP </td>
		</tr>
		<tr>
			<td> 554 </td>
			<td>true</td>
			<td>true</td>
			<td> rtsp </td>
			<td> Commande de flux </td>
		</tr>
		<tr>
			<td> 556 </td>
			<td>true</td>
			<td>false</td>
			<td> remotefs </td>
			<td> Remote Filesystem (système de fichiers à distance) </td>
		</tr>
		<tr>
			<td> 563 </td>
			<td>true</td>
			<td>true</td>
			<td> nntps </td>
			<td> NNTP via SSL/TLS </td>
		</tr>
		<tr>
			<td> 587 </td>
			<td>true</td>
			<td>false</td>
			<td> submission </td>
			<td> Message Submission Agent (agent de soumission de message) </td>
		</tr>
		<tr>
			<td> 631 </td>
			<td>true</td>
			<td>true</td>
			<td> ipp </td>
			<td> Internet Printing Protocol (protocole d’impression internet) </td>
		</tr>
		<tr>
			<td> 631 </td>
			<td>true</td>
			<td>true</td>
			<td>false</td>
			<td> Common Unix Printing System (non officiel - système d’impression&nbsp;Unix commun) </td>
		</tr>
		<tr>
			<td> 636 </td>
			<td>true</td>
			<td>true</td>
			<td> ldaps </td>
			<td> LDAP via SSL/TLS </td>
		</tr>
		<tr>
			<td> 674 </td>
			<td>true</td>
			<td>false</td>
			<td> acap </td>
			<td> Application Configuration Access Protocol (protocole d’accès à la configuration d’applications) </td>
		</tr>
		<tr>
			<td> 694 </td>
			<td>true</td>
			<td>true</td>
			<td> ha-cluster </td>
			<td> Service&nbsp;Heartbeat </td>
		</tr>
		<tr>
			<td> 749 </td>
			<td>true</td>
			<td>true</td>
			<td> kerberos-adm </td>
			<td> Administration&nbsp;Kerberos&nbsp;v5 </td>
		</tr>
		<tr>
			<td> 750 </td>
			<td>false</td>
			<td>true</td>
			<td> kerberos-iv </td>
			<td> Services&nbsp;Kerberos&nbsp;v4 </td>
		</tr>
		<tr>
			<td> 873 </td>
			<td>true</td>
			<td>false</td>
			<td> rsync </td>
			<td> Services de transfert de fichiers&nbsp;rsync </td>
		</tr>
		<tr>
			<td> 992 </td>
			<td>true</td>
			<td>true</td>
			<td> telnets </td>
			<td> Telnet via SSL/TLS </td>
		</tr>
		<tr>
			<td> 993 </td>
			<td>true</td>
			<td>false</td>
			<td> imaps </td>
			<td> IMAP via SSL/TLS </td>
		</tr>
		<tr>
			<td> 995 </td>
			<td>true</td>
			<td>false</td>
			<td> pop3s </td>
			<td> POP3 via SSL/TLS </td>
		</tr>
    </tbody>
</table>




# Registered Ports



<table>
    <thead>
        <tr>
            <th>Port</th>
            <th>TCP</th>
            <th>UDP</th>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead> 
    <tbody>
        <tr>
            <td>1080</td>
            <td>true</td>
            <td>false</td> 
            <td>socks</td> 
            <td>Proxy&nbsp;SOCKS</td> 
        </tr> 
        <tr> 
            <td>1433</td> 
            <td>true</td> 
            <td>false</td> 
            <td>ms-sql-s</td> 
            <td>Serveur&nbsp;Microsoft&nbsp;SQL</td> 
        </tr> 
        <tr> 
            <td>1434</td> 
            <td>true</td>
			<td>true</td>
			<td> ms-sql-m </td>
			<td> Moniteur Microsoft SQL </td>
		</tr>
		<tr>
			<td> 1494 </td>
			<td>true</td>
			<td>false</td>
			<td> ica </td>
			<td> Client Citrix ICA </td>
		</tr>
		<tr>
			<td> 1512 </td>
			<td>true</td>
			<td>true</td>
			<td> wins </td>
			<td> Windows Internet Name Service </td>
		</tr>
		<tr>
			<td> 1524 </td>
			<td>true</td>
			<td>true</td>
			<td> ingreslock </td>
			<td> Ingres DBMS </td>
		</tr>
		<tr>
			<td> 1701 </td>
			<td>false</td>
			<td>true</td>
			<td> l2tp </td>
			<td> Protocole de tunnelisation de niveau&nbsp;2/transfert de couche&nbsp;2 </td>
		</tr>
		<tr>
			<td> 1719 </td>
			<td>false</td>
			<td>true</td>
			<td> h323gatestat </td>
			<td> H.323 </td>
		</tr>
		<tr>
			<td> 1720 </td>
			<td>true</td>
			<td>false</td>
			<td> h323hostcall </td>
			<td> H.323 </td>
		</tr>
		<tr>
			<td> 1812 </td>
			<td>true</td>
			<td>true</td>
			<td> radius </td>
			<td> Authentification&nbsp;RADIUS </td>
		</tr>
		<tr>
			<td> 1813 </td>
			<td>true</td>
			<td>true</td>
			<td> radius-acct </td>
			<td> Accès&nbsp;RADIUS </td>
		</tr>
		<tr>
			<td> 1985 </td>
			<td>false</td>
			<td>true</td>
			<td> hsrp </td>
			<td> Cisco HSRP </td>
		</tr>
		<tr>
			<td> 2008 </td>
			<td>true</td>
			<td>false</td>
			<td>false</td>
			<td> Teamspeak 3 Accounting (non officiel) </td>
		</tr>
		<tr>
			<td> 2010 </td>
			<td>false</td>
			<td>true</td>
			<td>false</td>
			<td> Teamspeak 3 Weblist (non officiel) </td>
		</tr>
		<tr>
			<td> 2049 </td>
			<td>true</td>
			<td>true</td>
			<td> nfs </td>
			<td> Système de fichiers en réseau </td>
		</tr>
		<tr>
			<td> 2102 </td>
			<td>true</td>
			<td>true</td>
			<td> zephyr-srv </td>
			<td> Serveur&nbsp;Zephyr </td>
		</tr>
		<tr>
			<td> 2103 </td>
			<td>true</td>
			<td>true</td>
			<td> zephyr-clt </td>
			<td> Client&nbsp;Zephyr </td>
		</tr>
		<tr>
			<td> 2104 </td>
			<td>true</td>
			<td>true</td>
			<td> zephyr-hm </td>
			<td> Gestionnaire d’hôte&nbsp;Zephyr </td>
		</tr>
		<tr>
			<td> 2401 </td>
			<td>true</td>
			<td>false</td>
			<td> cvspserver </td>
			<td> Concurrent Versions System (système de gestion de versions) </td>
		</tr>
		<tr>
			<td> 2809 </td>
			<td>true</td>
			<td>true</td>
			<td> corbaloc </td>
			<td> Common Object Request Broker Architecture (architecture logicielle pour le développement de composants et d’object requests) </td>
		</tr>
		<tr>
			<td> 3306 </td>
			<td>true</td>
			<td>true</td>
			<td> mysql </td>
			<td> Service de base de données&nbsp;MySQL (pour MariaDB également) </td>
		</tr>
		<tr>
			<td> 4321 </td>
			<td>true</td>
			<td>false</td>
			<td> rwhois </td>
			<td> Remote Whois Service (service&nbsp;Whois à distance) </td>
		</tr>
		<tr>
			<td> 5999 </td>
			<td>true</td>
			<td>false</td>
			<td> cvsup </td>
			<td> CVSup </td>
		</tr>
		<tr>
			<td> 6000 </td>
			<td>true</td>
			<td>false</td>
			<td> X11 </td>
			<td> X Windows System Services (services système pour Windows&nbsp;X) </td>
		</tr>
		<tr>
			<td> 11371 </td>
			<td>true</td>
			<td>false</td>
			<td> pgpkeyserver </td>
			<td> Serveur de clés publiques pour PGP </td>
		</tr>
		<tr>
			<td> 13720 </td>
			<td>true</td>
			<td>true</td>
			<td> bprd </td>
			<td> Symantec/Veritas NetBackup </td>
		</tr>
		<tr>
			<td> 13721 </td>
			<td>true</td>
			<td>true</td>
			<td> bpdbm </td>
			<td> Symantec/Veritas Database Manager </td>
		</tr>
		<tr>
			<td> 13724 </td>
			<td>true</td>
			<td>true</td>
			<td> vnetd </td>
			<td> Symantec/Veritas Network Utility </td>
		</tr>
		<tr>
			<td> 13782 </td>
			<td>true</td>
			<td>true</td>
			<td> bpcd </td>
			<td> Symantec/Veritas NetBackup </td>
		</tr>
		<tr>
			<td> 13783 </td>
			<td>true</td>
			<td>true</td>
			<td> vopied </td>
			<td> Symantec/Veritas VOPIE </td>
		</tr>
		<tr>
			<td> 22273 </td>
			<td>true</td>
			<td>true</td>
			<td> wnn6 </td>
			<td> Conversion&nbsp;Kana/Kanji </td>
		</tr>
		<tr>
			<td> 23399 </td>
			<td>false</td>
			<td>false</td>
			<td>false</td>
			<td> Skype (non officiel) </td>
		</tr>
		<tr>
			<td> 25565 </td>
			<td>true</td>
			<td>false</td>
			<td>false</td>
			<td> Minecraft </td>
		</tr>
		<tr>
			<td> 26000 </td>
			<td>true</td>
			<td>true</td>
			<td> quake </td>
			<td> Quake et autres jeux multijoueurs </td>
		</tr>
		<tr>
			<td> 27017 </td>
			<td>false</td>
			<td>false</td>
			<td>false</td>
			<td> MongoDB </td>
		</tr>
		<tr>
			<td> 33434 </td>
			<td>true</td>
			<td>true</td>
			<td> traceroute </td>
			<td> Suivi de réseau </td>
		</tr> 
    </tbody> 
</table>
