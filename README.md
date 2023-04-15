# Strings
## _Programma C# per lo studio delle stringhe_
La consegna richiede la creazione di un programma che tratti la **manipolazione delle stringhe in MAUI**, ~~senza~~ usufruire di alcune utlity, tra le quali:
  * ToUpper()
  * ToLower()
  * Count()
  * Lenght()
  * Replace()
  * IsLetter()
  * IsNumber()
  * StringBuilder

In particolare, il programma dovrà eseguire diverse operazioni sulla chiesta inserita input:

* Trasformarla nella sua versione in caps lock
* Trasformarla nella sua versione minuscola
* Controllare se contiene solo caratteri alfabetici
* Controllare di quante lettere è formata
* Controllare se contiene solo caratteri alfanumerici
* Rovesciarla (esempio: ciao / oaic)



# Esempi di metodi creati per il realizzamento del programma

## Funzioni usata per replicare *ToUpper()*

```
char ToUpper(char c)
	{
		if (c >= 'a' && c <= 'z')
		{
			int x = (int)c & 0xDF;
			return (char)x;
		}
		return c;
	}
  ```




## Funzione utilizzata per replicare *IsLetter()*

```
bool IsLetter(char c)
	{
		if ((c >= 'a' && c <= 'z'))
			return true;
		if ((c >= 'A' && c <= 'Z'))
			return true;
		else
			return false;
	}
```
