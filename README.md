Για την δημιουργία του εκτελέσιμου προγράμματος τρέξτε:
    g++ main.cpp functions.cpp -o (όνομα εκτελέσιμου)

Προσχέδιο σχεδίασης λογισμικού:  
α)Καθολικές συναρτήσεις: 
    1)Generate map 
    2)Move(virtual) 
    3)Place(player,werewolves,vampires) 
    4)Check/Action(decision) 
    5)Heal(use of potions) 
 
β)Κλάσεις: 
Γονέας:
    1)Creatures 
    
Παιδιά/Απόγονοι: 
    2)Vampires 
    3)Werewolves 
    4)Avatar 

    main.cpp: Αρχικά ζητάει τις διαστάσεις του πίνακα και την 
    ομάδα που υποστηρίζει ο παίκτης χρησιμοποιώντας συναρτήσεις από την 
    Functions, υλοποιεί και εκτυπώνει τον χάρτη. Παράλληλα δημιουργεί 
    ισοπληθή αντικείμενα και από τα δύο είδη σύμφωνα με τον χάρτη και τα 
    αποθηκεύει σε δύο μονοδιάστατους πίνακες αντίστοιχα. Έπειτα, υπάρχει ένα 
    μεγάλο loop(while) του οποίου κάθε επανάληψη αντιστοιχεί σε έναν γύρο. 
    Πρώτα παίζει ο παίκτης χρησιμοποιώντας τα βελάκια και κάποια κουμπιά με 
    διαφορετικέςλειτουργίες, όπως pause και heal και αμέσως μετά αλλά στην 
    ίδια επανάληψη παίζουν οι λυκάνθρωποι κι έπειτα τα βαμπίρ. Επιπλέον, κάθε 
    δύο επαναλήψεις η κατάσταση της ημέρας αλλάζει(μέρα-νύχτα)και αναλόγως με 
    την ομάδα όπως αναγράφεται στις οδηγίες ο παίκτης μπορεί να 
    χρησιμοποιήσει το φίλτρο μαγικής επούλωσης για την ομάδα του σε περίπτωση 
    που έχει ένα στην κατοχή του.Όταν σκοτωθούν όλα τα μέλη μιας ομάδας, η 
    while σταματάει και το παιχνίδι ολοκληρώνεται. 
 
    Functions.cpp: Περιέχει τις υλοποιήσεις όλων των συναρτήσεων που 
    χρησιμοποιούνται από την main, πιο συγκεκριμένα όλες τις συναρτήσεις των 
    κλάσεων, όλες τις συναρτήσεις που χρησιμοποιούνται για την κατασκευή του 
    χάρτη και την τοποθέτηση και κίνηση των οντοτήτων. 

    Definitions.h: Αποτελεί το αρχείο επικεφαλίδας στο οποίο 
    ορίζονται όλες οι συναρτήσεις της Functions και περιέχονται οι ορισμοί και 
    τα περιεχόμενα των κλάσεων, στις οποίες υπάρχει μια κλάση creatures ως 
    hyperclass και άλλες τρεις κλάσεις, τις werewolf, vampire και ang οι 
    οποίες είναι απόγονοι της creatures.
