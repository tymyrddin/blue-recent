# Follina MSDT

The MSDT exploit is not really something new. A [bachelor’s thesis](https://benjamin-altpeter.de/doc/thesis-electron.pdf) 
was published August 2020 with techniques on how to use MSDT for code execution. 

Almost two years after that initial publication, pieces of evidence of MSDT exploitation 
as well as code execution via Office URIs has triggered several independent researchers to file separate reports to 
[MSRC](https://msrc-blog.microsoft.com/)

It’s not until the discovery of nao_sec, which was made public in twitter, that attacks using this particular vector 
is actively being made in the wild. This was picked up by Kevin Beaumont who publicly identified it as a zero-day 
that Microsoft [EDR products](blue-edr:index) are failing to detect, and then later classified by Microsoft as a 
zero-day with the vulnerability name [CVE-2022-30190](https://nvd.nist.gov/vuln/detail/cve-2022-30190).

## Further reading

* [Follina — a Microsoft Office code execution vulnerability | by Kevin Beaumont | May, 2022 | DoublePulsar](https://doublepulsar.com/follina-a-microsoft-office-code-execution-vulnerability-1a47fce5629e) - Full timeline, early details regarding the vulnerability, and “Follina” namesake courtesy of Kevin Beaumont
* [Rapid Response: Microsoft Office RCE - Follina MSDT Attack (huntress.com)](https://www.huntress.com/blog/microsoft-office-remote-code-execution-follina-msdt-bug)

