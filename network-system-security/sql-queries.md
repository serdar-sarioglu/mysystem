## How to trunk a Log file & Shrink DB

How to trunk ms sql logs:


>ALTER DATABASE [SampleDb] set recovery simple

>GO

>CHECKPOINT

>GO

>DBCC SHRINKFILE (SampleDb_log_file,1)

>GO

>ALTER DATABASE [SampleDb] set recovery full

>GO

Second Step to Shrink:

>USE [SampleDb];

>GO

>DBCC SHRINKFILE (SampleDb_log_file, 8);

>GO

##
This Document has been written By Serdar Sarioglu - 2015

KeyWords: `SQL` `Trunk` `Logs` `MS`

<a href="https://mysystem.org" title="Mysystem.org"><img src="https://img.shields.io/badge/Visit-mysite-green.svg"></a>
<a href="https://www.paypal.me/ssarioglu" title="Support project"><img src="https://img.shields.io/badge/Donate-me-red.svg"></a>
<a href="mailto:serdar.sarioglu@mysystem.org" title="Email"><img src="https://img.shields.io/badge/Email-me-blue.svg"></a>
<a href="https://www.linkedin.com/in/serdarsarioglu/" title="Linkedin"><img src="https://img.shields.io/badge/Linkedin-me-orange.svg"></a>
