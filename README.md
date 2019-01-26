# OAs

Here Spark with Python is used. Rule data is stored in 4 RDDs, for (inbound, tcp), (inbound, udp), (outbound, tcp), (outbound, udp). Rule data (port) is transformed to two intergers indicating upper-bound and lower-bound . Rule data (ip address) is transformed to two strings indicating upper-bound and lower-bound . Thus, in the 4 RDDs of rule data, every item includes 4 things: upper-bound and lower-bound of both port and ip address. If it is not a range appeared in the rule data of port or ip address, upper-bound and lower-bound will be the same. To compare the input data with the rules, we just need to compare the port and address with each item after making sure which RDD does it "belongs to".

Unfortunately, I did not have time to complete this task perfectly due to the system crash (actually I spent an hour to deal with the environment of Spark and finally failed). So I did not test it either. If I could have the chance to test the code,I would generate a large csv file using Python with data randomly chosen (and maybe repeatedly).

In addition, I accidently uploaded to a private repository and found this mistake after a while, which also made a lateness.

Thanks for your watching and I look forward to your advice for a better solution.


P.S. I am interested in data team since I am currently enrolled in a master program of data informatics. Though I do not have background of this area during my bachelor degree, I am actively learning about it this year and seeking for an opportunity to have experience on this area.
