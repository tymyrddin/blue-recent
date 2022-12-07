# Solar, exploiting log4j

On December 9th, 2021, the world was made aware of a new vulnerability identified as 
[CVE-2021-44228](https://nvd.nist.gov/vuln/detail/CVE-2021-44228), affecting the Java logging package `log4j`. 
This vulnerability earned a severity score of 10.0 (the most critical designation) and offers remote code trivial 
remote code execution on hosts engaging with software that utilizes this `log4j` version. This attack has been dubbed 
`Log4Shell`

Today, `log4j` versions are available which have this vulnerability patched (JNDI is fully disabled, support for 
Message Lookups is removed, and the DoS vulnerability [CVE-2021-45046](https://nvd.nist.gov/vuln/detail/CVE-2021-45046) 
is not present).

The danger of this vulnerability (and reason for including it here) is due to how ubiquitous the logging package is. 
Millions of applications as well as software providers use this package as a dependency in their own code. While 
you may be able to patch your own codebase using log4j, other vendors and manufacturers will still need to push 
their own security updates downstream. Many security researchers have likened this vulnerability to that of 
`Shellshock` by the nature of its enormous attack surface. We will see this vulnerability for years to come.
 
## Further reading

* [Critical RCE Vulnerability: log4j - CVE-2021-44228](https://www.huntress.com/blog/rapid-response-critical-rce-vulnerability-is-affecting-java)
* [Huntress Log4Shell Vulnerability Tester](https://log4shell.huntress.com/)
* [YouTube: CVE-2021-44228 - Log4j - MINECRAFT VULNERABLE! (and SO MUCH MORE)](https://www.youtube.com/watch?v=7qoPDq41xhQ)


