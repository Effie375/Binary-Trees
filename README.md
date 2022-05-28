# Δένδρο

## Ορισμός Δένδρου

Το **"Δένδρο"** είναι μια μη γραμμική, ιεραρχική δομή δεδομένων στην οποία:

- Αποτελείται από κόμβους (κορυφές) και ακμές (πλευρές) που ομοιάζουν με ένα (ανάποδο) δένδρο. Οι κόμβοι είναι τριών ειδών:
 - Η **ρίζα** είναι ο μοναδικός κόμβος από τον οποίο μόνο ξεκινούν ακμές
 - Οι **εσωτερικοί κόμβοι** (ή μη τερματικοί) στις οποίες καταλήγουν και ξεκινούν ακμές.
 - Τα **φύλλα** (ή τερματικοί κόμβοι) στα οποία καταλήγει μόνο μία ακμή.

Παράδειγμα:

```none
     Α    
    / \   
  Β    Γ  
 / \    \ 
Δ   Ε    Ζ
    |      
    Η      
```

- Ρίζα: Α
- Εσωτερικοί Κόμβοι: Β, Γ, Ε
- Φύλλα: Δ, Η, Ζ

Παρατηρήσεις:

- Το δένδρο χωρίς κόμβους λέγεται "κενό δένδρο" (null tree).
- Ένας εσωτερικός κόμβος έχει τουλάχιστον ένα παιδί.
- Τα φύλλα δεν έχουν παιδιά.

## Οικογενειακές Σχέσεις στα Δένδρα

Σε ένα δένδρο ορίζονται οικογενειακές σχέσεις των κόμβων. Στο παράδειγμα μελετάμε την οικογένεια του κόμβου Β:

```none
     Α    
    / \   
  Β    Γ  
 / \    \ 
Δ   Ε    Ζ
    |      
    Η      
```

- Α: **Πατέρας** του Β (Πρόγονος του Β)
- Γ: **Αδελφός** του Β
- Δ, Ε, Η: **Απόγονοι** του Β
- Δ: **Αριστερό Παιδί** του Β
- Ε: **Δεξί Παιδί** του Β

```none
       /
     Β    
    / \   
  Δ    Ε  
       | 
       Η    
```

- Υποδένδρο με ρίζα το Β
