PERTANYAAN DAN PENJELASAN family.pl
PERTANYAAN :
1. Siapakahanakdariarfan?
2. Siapakahanakdarifarah,burhan ?
3. Siapakah orang tuadaribahrun,raja ?
4. Siapakahanakperempuandarifarah ?
5. Siapakahanakdarifahri, salsa ?

PENJELASAN :
1. queryuntukmencarianak
anak(Y,X):-orang tua (X,Y).
caramembacanyaadalah Y adalahanakdari X dimana X adalah orang tuadari Y.
pertanyaan :siapakahanakdariarfan?

maka di prolog perintahnyaadalahsebagaiberikut :
?-laki(arfan).

2. queryuntukmencarianak
anak(Y,X):-orang tua (X,Y).
caramembacanyaadalah Y adalahanakdari X dimana X adalah orang tuadari Y.
pertanyaan :siapaanakdarifarah,burhan ?

maka di prolog perintahnyaadalahsebagaiberikut :
?- anak(farah, burhan).

3. queryuntukmencari orang tua
orangtua(X,Y):-perempuan(X).
caramembacanyaadalah X adalah orang tuadari Y dimana X itusendiriadalah orang tuadari Y.
pertanyaan :siapakahketurunandaribahrun, raja ?

maka di prolog perintahnyaadalahsebagaiberikut :
?- keturunan(bahrun, raja).

4. queryuntukmencarianakperempuan
anakpria (X,Y):-orang tua (X,Y),wanita(X).
caramembacanyaadalah X adalahanakwanitadari Y dimana Y itusendiriadalah orang tuadari X dan X adalahketeranganbuatanggotawanita
pertanyaan :siapakahanakperempuandarifarah?

maka di prolog perintahnyaadalahsebagaiberikut :
?-perempuan(farah).

5. queryuntukmencarianak
anak(Y,X):-orang tua (X,Y).
caramembacanyaadalah Y adalahanakdari X dimana X adalah orang tuadari Y.
pertanyaan :siapakahanakdarifahri, salsa?

?- anak(ferdi, syifa).



PERTANYAAN DAN PENJELASAN family.pl

PERTANYAAN :

1. siapakahorangtuadaribasir ?
2. siapakahneneksiti ?
3. siapakahanakdarituti?

PENJELASAN :

1. Mencari orang tuabasir
anak(Y,X):-Orangtua(X,Y).
caramembacanyaadalah Y adalahanakdari X dimana X adalah orang tuadari Y

makaperintahnya di prolog adalah
 ?- orangtua(basir, arfan).


2. Mencarineneksiti

nenek(X,Y):-orangtua(Z,Y)orangtua(Z,X),wanita(X).
caramembacanyaadalah X adalahnenekdari Y dimana Z itusendiriorangtuadari Y dan Z adalahorangtuadari X. dan (X) adalahmenyatakan data perempuan. 

maka di prolog perintahnyaadalahsebagaiberikut : 
 ?- nenek(siti).

3. Mencariapakahtutimempunyaianak
anak(Y,X):-Orangtua(X,Y).
caramembacanyaadalah Y adalahanakdari X dimanaXitusendiriorangtuadari Y 

maka di prolog perintahnyaadalahsebagaiberikut :
?- anak(tuti).
