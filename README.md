# Proiect final pentru cursul de testare manuală ITF

Scopul proiectului final pentru cursul de testare manuală ITF este de a folosi toate cunoștințele acumulate de-a lungul cursului și de a le aplica în practică, folosind o aplicație live.

Aplicație în curs de testare: https://opensource-demo.orangehrmlive.com/

Documentația API: https://orangehrm.github.io/orangehrm-api-doc/

**Proiectul final va fi împărțit în 2 secțiuni: [Secțiunea de testare](https://github.com/IulianB0/Proiect-Practic-Testare-Manuala/blob/main/README.md#specifica%C8%9Bii-func%C8%9Bionale# 1 Secțiunea de testare) și [SQL secțiune](https://github.com/julai215/itf_final_project_example_and_portofolio/blob/main/Final%20Project/README.md#2-sql-section).**

Instrumente folosite: JIRA, Zephyr Squad, Postman, MySQL Workbench.

# Specificații funcționale

Povestea de mai jos a fost creată în JIRA și descrie specificațiile funcționale ale modulului Dependenți, pentru care se realizează proiectul final.

![imagine](https://user-images.githubusercontent.com/99291143/163687093-6f1780d1-2808-4038-9ae2-65c22540a55c.png)


# 1 Secțiunea de testare

## 1.1 Planificarea testelor

Planul de testare este conceput pentru a descrie toate detaliile testării pentru modulul Dependenți din aplicația OrangeHRM.

Planul identifică elementele de testat, caracteristicile care trebuie testate, tipurile de testare care trebuie efectuate, personalul responsabil de testare, resursele și programul necesar pentru finalizarea testării și riscurile asociate cu planul.

#### 1.1.1 Rolurile atribuite proiectului și persoanele alocate

* Manager de proiect - Andrei Popescu
* Product owner - Mădălina Ionescu
* Dezvoltator software - Gabriela Tomescu
* Inginer QA - Iulia Albu

#### 1.1.2 Criteriile de intrare definite

* sunt definite specificatiile functionale
* sunt alocate rolurile necesare pentru proiect
* au fost detectate și atenuate riscurile inițiale ale proiectului

#### 1.1.3 Criteriile de ieșire definite

* numărul de erori nerezolvate este nesemnificativ sau au prioritate scăzută
* toate testele au fost executate
* toate erorile rezolvate au fost re-testate și aprobate de echipa QA
* termenul limită a fost atins
* niciun risc major detectat nu a rămas neatenuat
* testarea de regresie exploratorie trebuie efectuată pe modulul My Info, care include secțiunea Dependenți

#### 1.1.4 Domeniul testului

* __Teste în domeniu:__ Toate caracteristicile modulului Dependenți care au fost definite în specificațiile cerințelor software trebuie testate: testare funcțională, testare GUI și testare API
* __Teste care nu intră în domeniul de aplicare:__ testare de performanță, integrări ale modulului de dependență cu alte module, testare de compatibilitate cu mai multe browsere

#### 1.1.5 Riscuri detectate

* Riscuri ale proiectului: lipsa de experiență a echipei QA, termen scurt pentru încercarea Zephyr Squad, indisponibilitatea mediului de testare
* Riscuri de produs: constrângerile de validare asupra câmpurilor ar putea fi prea restrictive pentru utilizatorul final

#### 1.1.6 Evaluarea criteriilor de intrare

Criteriile de intrare definite în faza de planificare a testelor au fost atinse și procesul de testare poate continua.

## 1.2 Monitorizare și control de testare

Au fost generate diverse rapoarte periodice pentru a reflecta stadiul actual al procesului de testare, în cazul unor probleme majore s-ar putea lua măsuri de control.
Următorul raport de stare a fost generat după ce 40% din cazurile de testare au fost executate, la 1 aprilie 2022:

![imagine](https://user-images.githubusercontent.com/99291143/163689699-e0295daa-e5dc-4e87-a984-546d9351fbac.png)


## 1.3 Analiza testului

Procesul de testare va fi executat pe baza cerințelor de mai sus pentru modulul Dependenți. Au fost găsite următoarele condiții de testare:
  * Introduceți date numai pentru câmpurile obligatorii și verificați dacă persoana dependentă este creată/actualizată
  * Introduceți datele pentru toate câmpurile disponibile și verificați dacă persoana dependentă este creată/actualizată
  * Lăsați câmpurile obligatorii goale și verificați dacă persoana dependentă nu poate fi creată/actualizată
  * Vizualizați detaliile dependente și verificați că sunt corecte
  * Vedeți toate persoanele aflate în întreținere într-o listă
  * Verificați toate constrângerile de validare pentru câmpuri

## 1.4 Testare de proiectare

Cazurile de testare funcționale au fost create în Zephyr Squad. Pe baza analizei specificațiilor, tehnicile de proiectare a testelor utilizate pentru generarea cazurilor de testare
sunt analiza valorii limită, partiționarea echivalenței și testarea cazurilor de utilizare.

**Cazuri de testare:**

![imagine](https://user-images.githubusercontent.com/99291143/163688901-26234e0a-abfa-4034-93bf-bca37ad2b50c.png)


Cazurile de testare cu pași pot fi vizualizate aici: [Dependents_test_cases.pdf](https://github.com/julai215/itf_final_project_example_and_portofolio/blob/main/Final%20Project/Dependents_test_cases.pdf)

Pentru API-ul Dependents, a fost generată următoarea listă de verificare: [API_test_checklist.csv](https://github.com/julai215/itf_final_project_example_and_portofolio/blob/main/Final%20Project/API_test_checklist.csv)


## 1.5 Implementarea testului

Următoarele elemente sunt necesare pentru a fi pregătite înainte de începerea fazei de execuție a testului:

* Mediul de testare este activ și rulează: https://opensource-demo.orangehrmlive.com/
* Accesul la mediul de testare este dat: Nume utilizator : Admin | Parola: admin
