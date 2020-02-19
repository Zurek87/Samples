### Example 1
-----------------------------------------------------------------------------------------------------

Przyk�ad pokazuje mo�liwo�� zastosowania w�asnej listy w oparciu o istniej�ce obiekty enova. Zawiera zdefiniowane w�asne    View, z kt�rym zosta�a powi�zana odpowiednia definicja w postaci struktury viewform.xml. 
    
W wyniku zastosowania dodatku, powinna pojawi� si� dodatkowa grupa w menu g��wnym programu o nazwie *Samples* z opcj� *"Towary w�asne"*, po wybraniu kt�rej pojawi si� zaimplementowana lista.

* Extender\TowaryUlubioneKontaktuViewInfo.cs

    Przyk�adowan klasa z implementacj� View zbudowanego na bazie tabel enova.
* Extender\Menu.cs

    Rejestracja listy dla View

* UI\TowaryUlubioneKontaktu.viewform.xml

    Definicja page'a dla View

* UI\Config.TowaryUlubione.pageform.xml
  
  Definicja formularza ustawie� w Narz�dzia/Opcje...
    
* Extender\TowaryUlubioneConfigExtender.cs

  Obs�uga zapisu ustawie� w Narz�dzia/Opcje...

* Extender\TowaryUlubionePokazKontaktWorker.cs
  
  Rejestracja akcji dla listy towar�w ulubionych otwarcia powiazanych rekord�w 