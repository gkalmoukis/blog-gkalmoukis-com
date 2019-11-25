---
title: Διερμηνευτής της ΓΛΩΣΣΑΣ σε  Ubuntu 18.04
date: "2019-08-01T15:33:00.169Z"
language: el
---

Ο Διερμηνευτής της ΓΛΩΣΣΑΣ είναι ένα ολοκληρωμένο περιβάλλον ανάπτυξης αλγορίθμων σε μορφή ψευδοκώδικα, ειδικά σχεδιασμένο για τη ΓΛΩΣΣΑ, μια γλώσσα προγραμματισμού που διδάσκεται στα πλαίσια του μαθήματος Ανάπτυξη εφαρμογών σε προγραμματιστικό περιβάλλον (ΑΕΠΠ) της Γ΄ Γενικού Λυκείου. Είναι εγκεκριμένος από το Παιδαγωγικό Ινστιτούτο ως κατάλληλος για εργαστηριακή χρήση στη δευτεροβάθμια εκπαίδευση αποτελεί μέρος του πακέτου [Αλγοριθμική και Προγραμματισμός](http://www.ecedu.upatras.gr/algorithmics/) του ΥΠΕΠΘ.

## Εγγατάσταση  
Ο Διερμηνευτής διατίθεται από το [Αποθετήριο Πιστοποιημένου Εκπαιδευτικού Λογισμικού](http://ts.sch.gr/repository) της υπηρεσίας Τεχνικής Στήριξης ΣΕΠΕΗΥ, η έκδοση που παρέχεται για συστήματα linux είναι η έκδοση 0.94 Για να προσθέσετε το αποθετήριο στις πηγές σας εκτελέστε τις παρακάτω εντολές:
```bash
$ sh -c 'cd /tmp && wget ts.sch.gr/repo/add-repo'  
$ wget 'ts.sch.gr/repo/add-repo' 
$ sh 'add-repo ts.sch.gr/repo'
```
και στη συνέχεια με την εντολη apt-get εγκαταστήστε το πακέτο glossa.   install:
```bash
$ sudo apt-get install glossa
```
## Εκτέλεση
Για να εκκινήσετε τον Διερμηνευτή απο το τερματικό εκτελέστε την εντολή 
```bash
$ glossa
```
αν η εγγατάσταση έχει γίνει σωστά θα ανοίξει το περιβάλλον ανάπτυξης. 
