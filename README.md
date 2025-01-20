Experiment 1.2: Start and Stop IBM SDS instances
Aim: To understand and demonstrate the process of starting and stopping IBM SDS (Security Directory
Server) instances using command-line operations to manage LDAP services effectively.

Objective:
➢ Learn how to start and stop SDS instances (idsldap1 and idsldap2) using the ibmslapd
command.
➢ Understand how to verify the successful startup and shutdown of the instances.
➢ Practice managing multiple SDS instances to ensure proper functioning of directory services in a
secure environment.

Steps:
Step1 : Open Terminal from Desktop.
Step2 : Start the newly created SDS instance idsldap1 using below command:
/opt/ibm/ldap/V6.4/sbin/ibmslapd -I idsldap1 -n -t .
Note: Here in the command -I is instance name -n is to start -t to tail log
You can see the server is started.
Step3: To start the idsldap2 instance, use the command:
/opt/ibm/ldap/V6.4/sbin/ibmslapd -I idsldap2 -n -t.
Note: Here in the command -I is instance name -n is to start -t to tail log.
You can see the server is started.
Step4: To stop the idsldap1 instance, use the command /opt/ibm/ldap/V6.4/sbin/ibmslapd -I idsldap1 -
k. This command sends a signal to gracefully shut down the idsldap1 directory server instance, ensuring
that it stops properly without disrupting other services.
Step5 : To stop the idsldap2 instance, use the command /opt/ibm/ldap/V6.4/sbin/ibmslapd -I idsldap2 -
k. This sends a stop signal to the idsldap2 server, gracefully shutting it down while ensuring all processes
are properly terminated.
Note : Start and Stop SDS instances using above commands for all the exercises
below.

Learning Outcomes :
➢ Understand IBM SDS architecture and functionality.
➢ Gain command-line proficiency for starting/stopping instances.
➢ Learn how to manage IBM SDS instances (start, stop, restart).
➢ Develop troubleshooting skills for instance management.
➢ Build foundational knowledge in IBM LDAP server administration.
➢ Familiarize with automating instance start/stop processes.
