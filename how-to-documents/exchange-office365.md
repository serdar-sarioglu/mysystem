## Exchange & Office 365 Goodies

#### Junk Mail & Safe Senders Bulk (New)

Connect Exchange PowerShell Console: 

>Get-Mailbox | Set-MailboxJunkEmailConfiguration  -BlockedSendersAndDomains "bad-sender.com" -TrustedSendersAndDomains "john@good-sender.com" 

#### To Check Policy is applied

>Get-MailboxJunkEmailConfiguration -Identity <serdar@mysystem.org>

Update Existing Policy

>$Temp = Get-MailboxJunkEmailConfiguration <serdar@mysystem.org>

>$Temp.BlockedSendersAndDomains += "<bad-sender>.com","<user>@<bad-sender>.com","..."

>$Temp.TrustedSendersAndDomains += "<good-sender>.com","<user>@<good-sender>.com","..."

>Set-MailboxJunkEmailConfiguration -Identity <user@contoso.com> -BlockedSendersAndDomains  $Temp.BlockedSendersAndDomains -TrustedSendersAndDomains $Temp.TrustedSendersAndDomains 



##
This Document has been written By Serdar Sarioglu - 2015

KeyWords: `Exchange` `Office 365` `PowerShell` `Commands`

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/badge/Visit-mysite-green.svg"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate-me-red.svg"></a>
<a href="mailto:serdar.sarioglu@mysystem.org" title="Email"><img src="https://img.shields.io/badge/Email-me-blue.svg"></a>
<a href="https://www.linkedin.com/in/serdarsarioglu/" title="Linkedin"><img src="https://img.shields.io/badge/Linkedin-me-orange.svg"></a>
