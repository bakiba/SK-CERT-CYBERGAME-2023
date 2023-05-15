# SK-CERT - POORLY WRITTEN
> Vaša firma prevádzkuje aplikáciu, na ktorú niekto zaútočil a kompromitoval ju. Dostal si za úlohu zistiť, čo sa vlastne stalo. https://drive.google.com/file/d/1-7m5aO4B5JWz79xhNeTnOvt2m_pS4bjc/view?usp=share_link <br/>
Reported Difficulty: 1

## 1 Compromise
> Aký bol čas kompromitácie? Flag je vo formáte YYYY-MM-DD HH:MM:SS

## 2 What went wrong
> Máme čas kompromitácie, teraz musíme zistiť, čo sa pokazilo. Z logov vidíme, že útočník zneužil náš systém zabudnutých hesiel, je niečo zle s generovaním tokenov? Flag je vo formáte file_name:line_number

## 3 It worked?
> Dobre, takže sme zle vygenerovali náš token, ale prečo to fungovalo? Je niečo zlé v našich checkoch? Flag je vo formáte file_name:line_number

## 4 Technique
> Ale ako je možné, že sa dostali do servera, existujú nejaké ďalšie zraniteľnosti? Flag je vo formáte file_name:name_of_vulnerable_function

## 5 Escalation
> Po tom, čo sa útočník dostal na server, eskaloval privilégiá do bežného používateľského účtu a potom ho zneužil na root, predpokladáme, že to bolo prostredníctvom nášho programu pre štatistiky logov, môžete to skontrolovať a povedať nám, kde máme zraniteľnosť? Flag je premenná, ktorá sa používa na exploitáciu a riadok kódu vo formáte name:line
