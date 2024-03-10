The KQL query in ServerAgentsAssessment returns the versions of the Arc, AMA, MMA and MDE software components running on the Windows and Linux servers.
It requires MDE running on those servers (the software inventory is done by its MDVM component). The query can be launched in the Advanced Hunting page of the Microsoft Defender XDR portal.
Please note that I wasn't able to find a way to get the version of the AMA agent running on Windows Servers. I'm able to get the version of the AMA "extension" associated to the related VMs/Arc enabled servers by using a KQL query in Azure Resource Graph Explorer but I would have preferred to get everything in MDVM... Any better idea to get this result is welcome.

Acronyms:
Arc -> It's just Azure Arc
AMA -> Azure Monitoring Agent
MMA -> Microsoft Monitoring Agent
MDE -> Microsoft Defender for Endpoint
MDVM -> Microsoft Defender Vulnerability Management
XDR -> eXtended Detection and Response

Refereces of the versions of these components: 
* MMA for Windows Server: https://learn.microsoft.com/en-us/azure/virtual-machines/extensions/oms-windows#agent-and-vm-extension-version
* MMA for Linux: https://learn.microsoft.com/en-us/azure/virtual-machines/extensions/oms-linux
* AMA for Windows Server  and Linux: https://learn.microsoft.com/en-us/azure/azure-monitor/agents/azure-monitor-agent-extension-versions
* MDE for Windows Server: https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/windows-whatsnew?view=o365-worldwide
* MDE for Linux: https://learn.microsoft.com/en-us/microsoft-365/security/defender-endpoint/linux-whatsnew?view=o365-worldwide
* Arc for Windows Server and Linux: https://learn.microsoft.com/en-us/azure/azure-arc/servers/agent-release-notes

