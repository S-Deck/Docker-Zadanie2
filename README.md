# Docker-Zadanie2

* Budowanie obrazu
```
docker compose up -d
```

* Test CVE

![image](/ss/scout1.png)
![image](/ss/scout2.png)

---CZĘŚĆ DODATKOWA---
* Opis: Dodano krok "Semantic versioning" w którym używany jest skrypt "PaulHatch/semantic-version". Odpowiada on za generowanie wartości nowej wersji na podstawie commitów w gałęzi "main". Wartość ta znajduje się w zmiennej ${{ steps.versioning.outputs.version }}, która jest używana przy tagowaniu w nastepnych krokach.

* Łańcuchy Github Action wykonają się poprawnie jeśli między ich uruchomieniami nastąpiły zmiany w gałęzi main.
  Przykład uruchomienia Action bez wprowadzenia zmian w main:
  ![image](/ss/Action_failed.PNG)
