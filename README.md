socialskip
==========
Το  SocialSkip Service είναι ελεύθερα διαθέσιμο για εγκατάσταση. Είναι μία εφαρμογή με την οποία παρέχεται η δυνατότητα συλλογής στοιχείων διαδράσεως των χρηστών σε κάποιο video(play,pause, skip).  
Υπάρχει επίσης η δυνατότητα προσθήκης ερωτηματολογίου δίπλα στο video με την ενσωμάτωση του  Google Drive. Χρήσιμο εργαλείο για την δημιουργία στατιστικων στοιχειων και γραφικής ανάλυσης των διαδράσεων των χρηστών. 

ΟΔΗΓΙΕΣ ΕΓΚΑΤΑΣΤΑΣΗΣ

Προυποθέσεις για την εγκατάσταση είναι τα εξής: 
•	JDK 6 http://www.oracle.com/technetwork/java/javase/downloads/index.html
•	Google AppEngine Java SDK 1.6.3https://code.google.com/p/googleappengine/downloads/list
•	και Eclipse. http://eclipse.org/
Αρχικά θα κάνουμε εγκατάσταση του Google plugin στο Eclipse. Από το plugin επιλέγουμε  Google  Plugin  for  Eclipse και  Google  Web  Toolkit  SDK  2.4.0. 
Στη συνέχεια κάνουμε εγκατάσταση του appengine-java-sdk-1.6.3 
Κατεβάζουμε το SocialSkip_service στο σύστημα μας με την εντολή git clone <remote repo>  <όνομα αρχείου>
Στη συνέχεια στο σύστημα μας επιλέγουμε το <όνομα αρχείου> ---->Socilaskip_service ---->Sagisoc Επιλέγουμε το Sagisoc  και το αντιγράφουμε στο workspace του Eclipse. 
Ανοίγουμε το Eclipse και από το File--->Import---->General--->Existing Projects into workspace--->Next  επιλέγουμε Browse και στη συνέχεια το πεδίο Select  root  directory 
όπου βρίσκουμε και επιλέγουμε το φάκελο Sagisoc που αποθηκεύσαμε στο workspace και αφού τον επιλέξουμε πατάμε το Finish. 
Το Sagisoc πρέπει να βρίσκεται πλέον στο Eclipse. Επιλέγουμε το project και πατάμε Project -> Properties -> Java Built Path. 
Ανοίγουμε την καρτέλα Libraries και πατάμε  Add External JARs και προσθέτουμε τα αρχεία gdata-core-1.0.jar και opencsv-2.3.jar από τον κατάλογο war/WEB-INF/lib. 
Ελέγχουμε επίσης να υπάρχουν τα εξής 
App Engine SDK[App Engine 1.6.3 – 1.6.3]
GWT SDK[GWT – 2.4.0]
JRE System Library[jdk1.6.x…]
Αν δεν είναι επιλεγμένες αυτές οι εκδόσεις τότε με το κουμπί Edit μπορούμε να επιλέξουμε την επιθυμητή έκδοση για το καθένα. 
Για τη δημιουργία των Fusion Tables υπάρχουν αναλυτικές οδηγίες στη σελίδα  https://code.google.com/p/socialskip/downloads/detail?name=SocialSkip%20Service%20v2.0%20Greek.pdf&can=2&q=
Στη  σελίδα  https://appengine.google.com  αφού κάνουμε είσοδο  με  το  λογαριασμό  μας google επιλέγουμε  Create  Application.  
Πριν γίνει το deploy, επιλέγουμε Run από το μενού και Run Configurations. Στη συνέχεια επιλέγουμε  Web  Application  ->  SagiSoc  και  ανοίγουμε την  καρτέλα  Arguments.  
Στο  πεδίο  VM arguments  προσθέτουμε τη  τιμή  “-Dappengine.user.timezone.impl=UTC”  (χωρίς  τα  εισαγωγικά), και πατάμε  Run.
Είμαστε έτοιμοι να επιλέξουμε το google--->deploy

ΑΔΕΙΑ ΧΡΗΣΗΣ

GNU GPL v2

