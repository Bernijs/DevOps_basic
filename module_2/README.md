13. Salīdzināt vienādu failu (ne README) hash no mapes module_1 un module_2. Vai git redz atšķirību starp šiem failiem?
14. Rezultātus apkopot module_2 > README.md

commit hash ir atšķirīgi. 

16. Pārbaudīt kādas izmaiņas tika veiktas iepriekšējās nedēļas laikā. Atrast vismaz divus veidus kā to izdarīt.  
git log --since=1.week  
https://github.com/hashicorp/terraform/commits/main

17. Atrast commit kurus veica autors - “Laura Pacilio”  
git log --author="Laura Pacilio"

18. Atrast vai Laura ir veikusi commit pagājušā gada septembrī?  
Laura ir veikusi 11 commit pagājušā gada septembrī  
git log --pretty="%an - %cd" --author="Laura Pacilio" --since="09-01-2021" --until="30-09-2021"

19. Vai Laura ir veikusi commit vakar?  
Laura nav veikusi commit vakar.  
git log --since=yesterday

20. Rezultātus apkopot module_2 > README.md un pārsūtīt rezultātu github.

* Atlasot rezultātus no pagājušā gada 20 līdz 21 aprīlim var atrast commit kurš ir datēts ar 16 aprīli? Kāpēc tā ir? Atbildi apkopot module_2 > README.md un pārsūtīt rezultātu Github.  
git log --pretty="%an - %ad - %cd" --since="20-04-2021" --until="21-04-2021"  
cenšos saprast. Atbilde varētu būt šeit:  https://stackoverflow.com/questions/11856983/why-is-git-authordate-different-from-commitdate

--date=<date>
Override the author date used in the commit.