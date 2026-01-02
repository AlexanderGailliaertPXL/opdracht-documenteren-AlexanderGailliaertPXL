# opdracht-documenteren-AlexanderGailliaertPXL
dit is een repositorie voor het uploaden van een config van een router voor deze opdracht. 
deze config is gemaakt voor de opdracht van een netwerk te creeren voor het bedrijf technova solutions. ik heb hiervoor gekozen voor als dns TNS te nemen.  



      Current configuration : 986 bytes
!
version 15.4  
no service timestamps log datetime msec  
no service timestamps debug datetime msec  
service password-encryption  
!  
hostname centrale-router  
!  
!  
!  
enable secret 5 $1$mERr$c1R7/kACskPU7sBJd8FM3.  
!  
!  
!  
!  
!  
!  
ip cef  
no ipv6 cef  
!  
!  
!  
username alexander secret 5 $1$mERr$QcKZwc/9KtAbi2gWlEpcP.  
!  
!  
!  
!  
!  
!  
!  
!  
!    
!  
ip domain-name TNS  
!  
!  
spanning-tree mode pvst  
!  
!  
!  
!  
!  
!  
interface GigabitEthernet0/0/0  
 ip address 192.168.1.1 255.255.255.224  
 duplex auto  
 speed auto  
!  
interface GigabitEthernet0/0/1  
 ip address 192.168.2.1 255.255.255.240  
 duplex auto  
 speed auto  
!  
interface Vlan1  
 no ip address  
!  
ip classless  
!  
ip flow-export version 9  
!  
!  
!  
banner motd ^Cauthorized personal only^C  
!  
!  
!  
!  
line con 0  
 password 7 082243401A160912020A1F173D24362C  
 login  
!  
line aux 0  
!  
line vty 0 4  
 exec-timeout 30 0  
 password 7 083758571918160405041E00  
 login  
 transport input ssh  
line vty 5 15  
 exec-timeout 30 0  
 password 7 083758571918160405041E00  
 login  
 transport input ssh  
!  
!  
!  
end  






    hierbij de configuratie voor de centrale router voor dit kleine bedrijfje.
