![[Pasted image 20240420214102.png]]Normalmente em uma virtual machine, como o [[virtualBox]] são criados novos sistemas operacionais em cima do sistema operacional host, isso é um problema pois isso implica em satisfazer todas as necessidades de um sistema operacional, como o boot

Com containers, nos é permitido, graças ao container engine, instanciar serviços, e esses serviços estarão separados, sem a interferência de agentes externos.

Isso acontece poiso linux disponibiliza desde 2007, 2 recursos muito uteis do linux
- namespaces
	- ele isola processos que estão com o mesmo namespaces dos demais processos
-  cgroups
	- Permite o controle granular de alocação recursos, como memoria, ou processamento

A junção desses 2 recursos, resultou na criação do docker em 2013
![[Pasted image 20240420214719.png]]
*PID namespace é o nome da ferramenta que permitiu o docker existir*