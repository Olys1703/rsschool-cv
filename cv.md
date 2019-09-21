# Sergey Lysenko
***
##### Adress:
46, Revolucionnaya Street,
Samara, Russia, 443086
##### Phone number:
+79228283226
##### Career Objective: 
Interested to work as a Java Programmer in your esteemed organization skills where I can show my skills in programming to help the organization grow.
##### Key Skills:
* Ability to create simple but effective prorgramms management softwares using Java
* Expert in the general usage of С++ and Java
* Superior database management skills
* In depth knowledge of different procedures to be followed for data recovery in case of some crisis
* Good knowledge of connection between C++ and different softwares.
##### Languages
Russian (native), English (fluent)
##### Education:
Samara State Aerospace University, Samara, Russia, 2014-2018,
Robotic Process Automation
##### Professional Experience:
1. SCADA laboratory assistant, 2015-2018, [Samara State Aerospace University](https://ssau.ru/)
1. Conveyor programmer, 2018-2019, [Nestle](https://www.nestle.ru/)
1. STL, SCL, Assemler, VBA, Visual C++ Programmer, 2019, [SMS](http://www.sms-automation.ru/)
##### Code example:
         

```
FOR i:=1 TO n DO
	IF Pointers_to_DI_handler[i]<>0 THEN
		alar_ack:=alar_ack OR Pointers_to_DI_handler[i]^.State_Alarm_ACK;
		war_ack:=war_ack OR Pointers_to_DI_handler[i]^.State_Warning_ack;
		alar:=alar OR Pointers_to_DI_handler[i]^.State_alarm;
		war:=war OR Pointers_to_DI_handler[i]^.State_Warning;
		Simulation_Exist:=Simulation_Exist OR Pointers_to_DI_handler[i]^.data^.Simulation_Mod;
	END_IF
	IF Pointers_to_aI_handler[i]<>0 THEN
		alar_ack:=alar_ack OR Pointers_to_aI_handler[i]^.state_ack_HH OR Pointers_to_aI_handler[i]^.state_ack_ll OR ( Pointers_to_aI_handler[i]^.state_ack_oos AND Pointers_to_aI_handler[i]^.data^.alarm_on_oos);
		war_ack:=war_ack  OR Pointers_to_aI_handler[i]^.state_ack_H OR Pointers_to_aI_handler[i]^.state_ack_l OR ( Pointers_to_aI_handler[i]^.state_ack_oos AND Pointers_to_aI_handler[i]^.data^.warning_on_oos);
	
		alar:=alar OR Pointers_to_aI_handler[i]^.state_HH OR Pointers_to_aI_handler[i]^.state_ll OR ( Pointers_to_aI_handler[i]^.state_oos AND Pointers_to_aI_handler[i]^.data^.alarm_on_oos);
		war:=war  OR Pointers_to_aI_handler[i]^.state_H OR Pointers_to_aI_handler[i]^.state_l OR ( Pointers_to_aI_handler[i]^.state_oos AND Pointers_to_aI_handler[i]^.data^.warning_on_oos);
		
		Simulation_Exist:=Simulation_Exist OR (Pointers_to_AI_handler[i]^.data^.Sim_mod<>0);
	END_IF
	IF Pointers_to_DO_handler[i]<>0 THEN
		Simulation_Exist:=Simulation_Exist OR Pointers_to_Do_handler[i]^.data^.Simulation_Mod;
	END_IF
END_FOR
```