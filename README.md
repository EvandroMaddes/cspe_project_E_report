# cspe_project_E_report
A three tier web application is comp osed by a web server, an application
server and a DB: services are called in sequence. Each server is replicated
resp ectively in CWS, CAS and CDB instances, each one running on a different
machine that shares a common queue of finite capacity KWS, KAS and KDB.
Three types of requests populate the system: NU user requests (characterised
by a think time ZU), NS remote procedure call software agents, and NB batch
elaboration programs. Each type of request requires a different amount of
time from each resource, according to an exponential distribution following
the average shown in the table below. Requests arriving at a full station are
blocked after they are served.
We want to determine the minimum number of replica CWS, CAS and
CDB for each server such that requests are served on the average in less than
2 sec.
