# My Analysis of tcpdump log

I checked the tcpdump logs given in the course.

What I found:

1.  First my pc asked dns.google for yummyrecipesforme.com IP. It gave 203.0.113.22. This is DNS.

2.  Then 3-way handshake happened - S, S-ACK, ACK. Means TCP connection was made.

3.  Then my pc did GET / HTTP/1.1 request. Means it asked for homepage. Here the hack happened and file download prompt came.

4.  After downloading file, my pc again asked dns for greatrecipesforme.com. It got 192.0.2.17. I never typed this second website. So this is suspicious.

5.  Again same handshake and GET request happened but for the second website. So user was redirected.

Conclusion:
Protocols used are DNS, TCP, HTTP. This log shows how attacker redirected user from real site to fake site.

This is what I learned from this activity.
