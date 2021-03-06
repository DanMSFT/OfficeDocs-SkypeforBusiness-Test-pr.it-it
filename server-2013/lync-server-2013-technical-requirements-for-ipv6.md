﻿---
title: 'Lync Server 2013: Requisiti tecnici per IPv6'
TOCTitle: Requisiti tecnici per IPv6
ms:assetid: caff0123-ce41-4a62-87a0-00b1d118b72b
ms:mtpsurl: https://technet.microsoft.com/it-it/library/JJ205278(v=OCS.15)
ms:contentKeyID: 49301965
ms.date: 08/24/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Requisiti tecnici per IPv6 in Lync Server 2013

 

_**Ultima modifica dell'argomento:** 2012-10-30_

Se si prevede di configurare Lync Server 2013 per IPv6, tenere conto dei requisiti seguenti:

  - Per utilizzare gli indirizzi IPv6 con Lync Server, è necessario creare record DNS (Domain Name System) per i record che devono essere individuati e risolti in un indirizzo IPv6. Il DNS IPv6 utilizza record AAAA (A quadrupla) dell'host. Se si utilizzano entrambi gli indirizzamenti IPv4 e IPv6 nella distribuzione, è consigliabile configurare e gestire sia i record A dell'host per IPv4 che i record AAAA dell'host per IPv6. Anche in caso di transizione completa della distribuzione a IPv6, è possibile che siano comunque necessari record dell'host DNS IPv4 per gli utenti esterni che continuano a utilizzare IPv4.
    
    È possibile distribuire record DNS IPv6 prima di iniziare a utilizzare IPv6. Se il client o il server non utilizza IPv6, il record non verrà utilizzato come riferimento. Le tecnologie transitorie sceglieranno quale record utilizzare in base alla configurazione e ai criteri della tecnologia.

  - Ogni indirizzo IPv6 prevede un ambito. I tre ambiti che è possibile utilizzare per l'indirizzamento IPv6 sono gli indirizzi globali IPv6 (simili agli indirizzi IPv4 pubblici), gli indirizzi locali univoci IPv6 (simili agli intervalli di indirizzi IPv4 privati) e gli indirizzi IPv6 locali rispetto al collegamento (simili agli indirizzi IP privati automatici in Windows Server per IPv4). Tutti i server di un pool devono disporre di indirizzi IPv6 con lo stesso ambito.

<table>
<thead>
<tr class="header">
<th><img src="images/Gg412908.important(OCS.15).gif" title="important" alt="important" />Importante:</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>IPv6 è un argomento complesso che richiede una pianificazione accurata con il team di rete e il provider Internet affinché gli indirizzi assegnati a livello di Windows Server e di Lync Server 2013 funzionino come previsto. Vedere i collegamenti alla fine dell'argomento per risorse aggiuntive sull'indirizzamento IPv6 e la pianificazione.</td>
</tr>
</tbody>
</table>


## Vedere anche

#### Ulteriori risorse

[Architettura dell'indirizzamento IP versione 6](http://tools.ietf.org/html/rfc4291)  
[Formato degli indirizzi unicast globali IPv6](http://tools.ietf.org/html/rfc3587)  
[Indirizzi unicast IPv6 locali univoci](http://tools.ietf.org/html/rfc4193)

