# 📘 Test z Sieci Komputerowych

---

## 1. Komunikaty ICMP używane do przekazywania informacji o pomyślnym wykonaniu polecenia ping:

- [ ] a) Echo Replay  
- [ ] b) TTL  
- [ ] c) Source Quench  
- [ ] d) Information Request  

## 2. Połączono komputery: Host A - `10.0.0.10/22`, Host B - `10.10.0.0/12`. Które stwierdzenie jest prawdziwe?

- [ ] a) Komputer A poprawnie wyśle pakiet do komputera B  
- [ ] b) Komputer B **nie** wyśle poprawnie pakietu do komputera A  
- [ ] c) Komputer A **nie** wyśle poprawnie pakietu do komputera B  
- [ ] d) Komputer B poprawnie wyśle pakiet do komputera A  

## 3. Skąd IP wie, gdzie dostarczyć pakiet o wskazanym adresie IP?

- [ ] a) Żadna z powyższych odpowiedzi nie jest poprawna  
- [ ] b) IP korzysta z protokołu ICMP do określania trasy  
- [ ] c) Wszystkie odpowiedzi są poprawne  
- [ ] d) W datagramie IP zapisany jest adres routera następnego przeskoku  
- [ ] e) W tablicy routingu zapisana jest trasa  

## 4. Adresami prywatnymi są:

- [ ] a) 10.10.10.10  
- [ ] b) 172.168.10.1  
- [ ] c) 192.168.0.1  
- [ ] d) 192.10.10.1  

## 5. Które działania realizują protokoły routingu?

- [ ] a) Uzyskiwanie informacji o trasach  
- [ ] b) Dostarczanie schematu adresacji  
- [ ] c) Informowanie hostów o nowych bramach  

## 6. Dwa komputery A i B połączone przez router. Tablice ARP są puste. Co jest prawdą?

- [ ] a) Na routerze niepotrzebne są wpisy ARP  
- [ ] b) Router potrzebuje MAC obu komputerów  
- [ ] c) Wysłanie pakietu możliwe po ustaleniu MAC przez każde urządzenie  
- [ ] d) Komputer A nie potrzebuje MAC_B  
- [ ] e) Router wysyła zapytanie ARP w imieniu komputera A  

## 7. Pierwszy komunikat DHCP po podłączeniu hosta:

- [ ] a) DHCPOFFER wysłany przez serwer  
- [ ] b) DHCPDISCOVER wysłany przez serwer  
- [ ] c) DHCPOFFER wysłany przez hosta  
- [ ] d) DHCPDISCOVER wysłany przez hosta  

## 8. Adres `225.225.0.0` to:

- [ ] a) Grupa hostów  
- [ ] b) Pojedyncze urządzenie  
- [ ] c) Podsieć  
- [ ] d) Sieć  

## 9. Mechanizm split horizon a zliczanie do nieskończoności:

- [ ] a) Może wystąpić, ale zmniejsza ruch  
- [ ] b) Może wystąpić rzadziej  
- [ ] c) Nie może wystąpić  

## 10. Cechy protokołu IP:

- [ ] a) Potwierdza doręczenia  
- [ ] b) Niezawodny  
- [ ] c) Poprzedzony fazą uzgadniania  
- [ ] d) Obsługuje split-horizon  
- [ ] e) Bezpołączeniowy  
  
  

## 11. Datagram IP:

- [ ] a) Ma zmienną długość  
- [ ] b) Pozwala uzyskać adres innego hosta  
- [ ] c) Wskazuje trasę przesyłania w sieci  
- [ ] d) Posiada sumę kontrolną całego pakietu  
- [ ] e) Nie może być wysyłany multicastowo  

## 12. Informacje o sfragmentowanym pakiecie przenoszą pola nagłówka IP:

- [ ] a) Identyfikator wersji  
- [ ] b) Pole TTL  
- [ ] c) Pole TOS  
- [ ] d) Flaga MF (More Fragments)  
- [ ] e) Flaga DF (Don't Fragment)  

## 13. Ponowne złożenie pakietu IP, który uległ fragmentacji, odbywa się:

- [ ] a) U hosta-odbiorcy  
- [ ] b) Na ruterze najbliższego przeskoku  
- [ ] c) Na najbliższym ruterze, który ma wystarczające MTU  

## 14. Dwa komputery A i B oraz ruter R są w jednej sieci. Co pojawi się w tablicach ARP?

- [ ] a) W komputerze A: IP_B – MAC_B  
- [ ] b) W ruterze R nie pojawi się żaden nowy wpis  
- [ ] c) W komputerze B: IP_A – MAC_A  
- [ ] d) W ruterze R: IP_B – MAC_B oraz IP_A – MAC_A  
- [ ] e) W komputerze A: IP_R – MAC_R  

## 15. Najczęstsza przyczyna powstawania pętli routingu:

- [ ] a) Niespójne informacje w tablicach routingu  
- [ ] b) Liczba przeskoków przekracza wartość maksymalną  
- [ ] c) Liczenie do nieskończoności  
- [ ] d) Split horizon  

## 16. Dla adresu `172.168.10.4/20` prawdziwe są:

- [ ] a) Na numer podsieci przeznaczone są 4 bity  
- [ ] b) Adres podsieci to `172.168.10.0`  
- [ ] c) Można stworzyć 16 podsieci  
- [ ] d) Maska to `255.255.240.0`  
- [ ] e) To adres prywatny  

## 17. Protokół DHCP pozwala na:

- [ ] a) Uzyskanie nazwy domenowej  
- [ ] b) Automatyczne uzyskanie adresu IP  
- [ ] c) Uzyskanie adresu IP odbiorcy  
- [ ] d) Przetłumaczenie domeny na IP  
- [ ] e) Uzyskanie adresu bramy domyślnej  

## 18. Zadaniem której warstwy jest routing pakietów?

- [ ] a) Warstwa aplikacji  
- [ ] b) Warstwa sieciowa  
- [ ] c) Warstwa łącza danych  
- [ ] d) Warstwa transportowa  

## 19. Czy adresy `126.12.5.3` i `126.12.6.3` są w tej samej podsieci, jeśli identyfikacja podsieci to 8 bitów?

- [ ] a) Tak  
- [ ] b) Nie  
- [ ] c) Nie da się jednoznacznie odpowiedzieć  

## 20. Które zdanie opisuje routing statyczny?

- [ ] a) Administrator ręcznie wstawia trasy do tablicy  
- [ ] b) Trasy są zdefiniowane w statycznej tablicy RARP  
- [ ] c) Trasy są automatycznie dodawane  
- [ ] d) Trasy pobierane są z serwera nazw  

## 21. Dla adresu `192.168.10.131` z maską `255.255.255.192`, adres podsieci to:

- [ ] a) 192.168.10.192  
- [ ] b) 192.168.10.128  
- [ ] c) 192.168.10.0  
- [ ] d) 192.168.0.0  

## 22. Protokół ARP służy do wyznaczenia:

- [ ] a) Adresu IP hosta na podstawie jego MAC  
- [ ] b) Adresu MAC hosta na podstawie jego IP  
- [ ] c) Źródłowego IP na podstawie MAC  
- [ ] d) Numeru portu urządzenia  

## 23. W protokołach routingu dynamicznego metryka określa:

- [ ] a) Odległość do sieci docelowej  
- [ ] b) Odległość z sieci źródłowej do docelowej  
- [ ] c) Liczbę przeskoków z sieci źródłowej do docelowej  

## 24. Protokół ARP służy do:

- [ ] a) Przydzielenia adresu Ethernet dla hostów bezdyskowych  
- [ ] b) Przydzielenia adresu IP dla hostów bezdyskowych  
- [ ] c) Znalezienia adresu MAC na podstawie IP  
- [ ] d) Znalezienia adresu IP na podstawie MAC  

## 25. Co się stanie, gdy router otrzyma datagram IP z polem TTL = 1?

- [ ] a) TTL zostanie zmniejszone i datagram przesłany dalej  
- [ ] b) Datagram zostanie odrzucony, a ICMP zgłosi błąd trasy  
- [ ] c) Datagram zostanie odrzucony bez powiadomienia  
- [ ] d) Datagram zostanie odrzucony, a ICMP zgłosi przekroczony czas życia  

## 26. Adres multicast to:

- [ ] a) Pakiety zawsze przekazywane przez routery  
- [ ] b) Adres rozgłoszeniowy do grupy urządzeń  
- [ ] c) Adres klasy E  
- [ ] d) Adres klasy D  
- [ ] e) Adres broadcastowy  

## 27. Dwie stacje w różnych sieciach połączone przez jeden router:

- [ ] a) Muszą mieć ustawiony adres bramki  
- [ ] b) Muszą mieć taką samą maskę  
- [ ] c) Router wymaga statycznych tras domyślnych  

## 28. Adres odbiorcy ramki zawierającej żądanie ARP to:

- [ ] a) MAC broadcastowy  
- [ ] b) IP bramy domyślnej  
- [ ] c) MAC bramy domyślnej  
- [ ] d) IP broadcastowy  

## 29. Który protokół informuje o błędach transmisji IP?

- [ ] a) IGMP  
- [ ] b) SMTP  
- [ ] c) ICMP  
- [ ] d) RARP  

## 30. Co się stanie, jeśli datagram IP przekracza MTU?

- [ ] a) Zostanie odrzucony z komunikatem ICMP „sieć nieosiągalna”  
- [ ] b) Zostanie odrzucony bez komunikatu  
- [ ] c) Zostanie pofragmentowany i przesłany  
- [ ] d) Zostanie odrzucony z komunikatem ICMP „źródło stłumione”  



## 31. Suma kontrolna w nagłówku pakietu IP dotyczy:

- [ ] a) Całego pakietu (nagłówek + dane)  
- [ ] b) Tylko nagłówka  
- [ ] c) Tylko danych  

## 32. Ponowne złożenie pakietu IP po fragmentacji odbywa się:

- [ ] a) U węzła-odbiorcy  
- [ ] b) Na routerze najbliższego przeskoku  
- [ ] c) Na najbliższym routerze, który ma wystarczające MTU  

## 33. W której warstwie modelu OSI działa protokół ICMP?

- [ ] a) Warstwa łącza danych  
- [ ] b) Warstwa sieci  
- [ ] c) Warstwa sesji  
- [ ] d) Warstwa transportowa  

## 34. Co opisuje routing dynamiczny?

- [ ] a) Administratorzy ręcznie wprowadzają trasy  
- [ ] b) Tablice routingu są aktualizowane automatycznie na podstawie informacji od innych routerów  
- [ ] c) Za zbieranie i przesyłanie informacji odpowiada serwer tras  
- [ ] d) Kierunki i odległości się nie zmieniają  

## 35. Liczenie do nieskończoności w RIP:

- [ ] a) Powoduje nieskończoną wędrówkę pakietów  
- [ ] b) Pozwala na budowę sieci do 16 routerów  
- [ ] c) Pozwala na sieć o nieograniczonym rozmiarze  
- [ ] d) Powoduje, że pakiety krążą 16 razy „w koło”  

## 36. Dla adresu `200.0.10.141` z maską `255.255.255.192`, prawdziwe są:

- [ ] a) Na numer hosta przeznaczone jest 6 bitów  
- [ ] b) Na numer hosta przeznaczone są 3 bity  
- [ ] c) W podsieci jest 30 adresów użytecznych  
- [ ] d) W podsieci jest 64 adresy użyteczne  
- [ ] e) W podsieci jest 62 adresy użyteczne  

## 37. Jakie informacje wykorzystuje router z RIP do wyznaczenia najlepszej ścieżki?

- [ ] a) Szybkość zbieżności  
- [ ] b) Część adresu hosta  
- [ ] c) Metryka do sieci docelowej  

## 38. Adres `112.10.3.4` należy do klasy:

- [ ] a) A  
- [ ] b) B  
- [ ] c) C  
- [ ] d) D  

## 39. Tablica ARP zawiera:

- [ ] a) Adres IP bramy domyślnej  
- [ ] b) MAC hosta obcego  
- [ ] c) Typ wpisu (statyczny/dynamiczny)  
- [ ] d) IP hosta obcego  
- [ ] e) Numer portu przełącznika, do którego podłączony jest host  

## 40. Aby hosty `192.172.16.41` i `192.172.16.27` były w tej samej podsieci, maska powinna wynosić:

- [ ] a) 255.255.255.240  
- [ ] b) 255.255.255.224  
- [ ] c) 255.255.255.248  
- [ ] d) 255.255.255.192  
