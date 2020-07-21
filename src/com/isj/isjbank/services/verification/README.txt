Le service implemente la fonction verification
	verification(String check, int age, int salaire, int montant_pret, String cni, String numero_compte, int montant_retrait)

------------------------------------------------------TEST--------------------------------------------------------

Verifier si un client exit
----------> verification("client", 0 , 0, 0, "123456789", "0" ,0)
check="client" et cni="123456789" et le reste=0 ou "0"


Verifier si le compte existe pour supprimer
----------> verification("delete", 0 , 0, 0, "0", "COMP12345" ,0)


Verifier le droit de pret
----------> verification("pret", 30 , 250000, 1500000, "0", "0" ,0)


Verifier le solde
----------> verification("solde", 0 , 0, 0, "0", "COMP12345" ,340000)


Elle retourne un boolean.

