# Notatki
## 1. DSADD – tworzenie grup
-   `dsadd group` – tworzenie grupy
-   `CN` – nazwa grupy    
-   `OU` – jednostka organizacyjna    
-   `DC` – domena    
-   `-secgrp yes` – grupa zabezpieczeń    
-   `-scope g` – grupa globalna    
-   `-scope L` – grupa lokalna domenowa    
-   `-samid` – nazwa logowania grupy
## 2. CSVDE – import grup
-   `-i` – import    
-   `-f` – nazwa pliku 
-   `-k` – pomijanie określonych błędów
## 3. LDIFDE – import grup
-   `-i` – import   
-   `-f` – plik    
-   `-k` – pomijanie określonych błędów
-   `changetype: modify` – modyfikacja    
-   `add: member` – dodanie członka    
-   `-` – koniec operacji
## 4. DSMOD – modyfikowanie grup
-   `-addmbr` – dodaje członka    
-   `-rmmbr` – usuwa członka
## 5. DSGET – pobieranie informacji
-   `dsget group` – informacje o grupie    
-   `-members` – wyświetla członków
## 6. DSMOVE – przenoszenie i zmiana nazwy
-   `-newname` – nowa nazwa    
-   `-newparent` – nowa lokalizacja
## 7. DSQUERY – wyszukiwanie
-   `dsquery group` – wyszukiwanie grup    
-   `-limit 0` – brak limitu wyników
## 8. DSRM – usuwanie
- `dsrm` – usuwanie obiektów z AD
## 9. PowerShell – tworzenie grupy
-   `Import-Module ActiveDirectory` – ładowanie modułu AD    
-   `New-ADGroup` – tworzenie grupy    
-   `-Name` – nazwa grupy    
-   `-SamAccountName` – nazwa logowania    
-   `-GroupScope Global` – zakres globalny    
-   `-GroupCategory Security` – grupa zabezpieczeń    
-   `-Path` – lokalizacja grupy
## 10. PowerShell – członkowie grup
-   `Add-ADGroupMember` – dodaje członka 
-   `Remove-ADGroupMember` – usuwanie członka
-   `Get-ADGroupMember` – wyświetlanie członków
-   `-Identity` – nazwa grupy   
-   `-Members` – użytkownik
## 11. PowerShell – CSV
-   `$` – zmienna    
-   `Import-Csv` – wczytuje CSV  
-   `foreach` – pętla
-   `-split ";"` – dzieli tekst po średniku


# Wnioski
-   Potrafię tworzyć globalne i lokalne grupy zabezpieczeń w Active Directory za pomocą polecenia Dsadd.

-   Potrafię importować grupy z plików CSV i LDIF za pomocą narzędzi CSVDE i LDIFDE.
    
-   Potrafię dodawać i usuwać członków grup oraz modyfikować grupy za pomocą Dsmod i Dsget.
    
-   Potrafię zmieniać nazwy grup i przenosić je do innych jednostek organizacyjnych za pomocą Dsmove.
    
-   Potrafię dodawać członków do grup w Windows PowerShell przy użyciu ścieżek LDAP.
    
-   Potrafię tworzyć grupy w Active Directory za pomocą skryptów PowerShell i VBScript.
    
-   Potrafię automatyzować tworzenie wielu grup i dodawanie do nich użytkowników na podstawie plików CSV.
