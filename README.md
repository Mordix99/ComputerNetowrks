# 📘 Test z Sieci Komputerowych
---

## 1. Komunikaty ICMP używane do przekazywania informacji o pomyślnym wykonaniu polecenia ping:

- [x] a) Echo Replay  
- [ ] b) TTL  
- [ ] c) Source Quench  
- [ ] d) Information Request  

## 2. Połączono komputery: Host A - `10.0.0.10/22`, Host B - `10.10.0.0/12`. Które stwierdzenie jest prawdziwe?

- [ ] a) Komputer A poprawnie wyśle pakiet do komputera B  
- [x] b) Komputer B **nie** wyśle poprawnie pakietu do komputera A  
- [x] c) Komputer A **nie** wyśle poprawnie pakietu do komputera B  
- [ ] d) Komputer B poprawnie wyśle pakiet do komputera A

<details>
<summary>💡 <strong>Chat podpowiada</strong></summary>

- Komputer **A** (mały zakres: `/22`) widzi komputer **B** (`10.10.0.0`) jako **spoza swojej sieci** – więc **kieruje pakiet przez bramkę (router)**, jeśli jest skonfigurowana.  
- Komputer **B** (duży zakres: `/12`) widzi komputer **A** (`10.0.0.10`) **jako lokalny adres** i **wysyła pakiet bezpośrednio**, próbując odwołać się do MAC-a A.

❗ **Ale... ruchu ICMP nie ma.**  
Sprawdzone w Cisco Packet Tracer – **brak odpowiedzi** na `ping`, ponieważ komputer A ignoruje ARP od B (uważa go za host spoza sieci), a B nie korzysta z bramki, bo „widzi” A jako lokalnego.  
</details>

## 3. Skąd IP wie, gdzie dostarczyć pakiet o wskazanym adresie IP?

- [ ] a) Żadna z powyższych odpowiedzi nie jest poprawna  
- [ ] b) IP korzysta z protokołu ICMP do określania trasy  
- [ ] c) Wszystkie odpowiedzi są poprawne  
- [ ] d) W datagramie IP zapisany jest adres routera następnego przeskoku  
- [ ] e) W tablicy routingu zapisana jest trasa  

## 4. Adresami prywatnymi są:

- [x] a) 10.10.10.10  
- [ ] b) 172.168.10.1  
- [x] c) 192.168.0.1  
- [ ] d) 192.10.10.1  

## 5. Które działania realizują protokoły routingu?

- [x] a) Uzyskiwanie informacji o trasach  
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
- [x] d) DHCPDISCOVER wysłany przez hosta

<details>
<summary>💡 <strong>Notatka: Proces DHCP (DORA)</strong></summary>
1. 🛰️ <strong>DHCPDISCOVER</strong> – klient wysyła rozgłoszeniowo zapytanie o dostępne serwery DHCP<br>
2. 📦 <strong>DHCPOFFER</strong> – serwer DHCP odpowiada oferując konfigurację (adres IP i inne parametry)<br>
3. 🙋 <strong>DHCPREQUEST</strong> – klient wybiera jedną ofertę i prosi o przydzielenie adresu<br>
4. ✅ <strong>DHCPACK</strong> – serwer potwierdza przydzielenie i kończy proces<br><br>
</details>


## 8. Adres `225.225.0.0` to:

- [x] a) Grupa hostów  
- [ ] b) Pojedyncze urządzenie  
- [ ] c) Podsieć  
- [ ] d) Sieć  

## 9. Mechanizm split horizon a zliczanie do nieskończoności:

- [ ] a) Może wystąpić, ale zmniejsza ruch  
- [x] b) Może wystąpić rzadziej  
- [ ] c) Nie może wystąpić  

## 10. Cechy protokołu IP:

- [ ] a) Potwierdza doręczenia  
- [ ] b) Niezawodny  
- [ ] c) Poprzedzony fazą uzgadniania  
- [ ] d) Obsługuje split-horizon  
- [x] e) Bezpołączeniowy  
  
  

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
- [x] d) Flaga MF (More Fragments)  
- [x] e) Flaga DF (Don't Fragment)  

## 13. Ponowne złożenie pakietu IP, który uległ fragmentacji, odbywa się:

- [x] a) U hosta-odbiorcy  
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

- [x] a) Na numer podsieci przeznaczone są 4 bity  
- [ ] b) Adres podsieci to `172.168.10.0`  
- [x] c) Można stworzyć 16 podsieci  
- [x] d) Maska to `255.255.240.0`  
- [ ] e) To adres prywatny  

## 17. Protokół DHCP pozwala na:

- [ ] a) Uzyskanie nazwy domenowej  
- [x] b) Automatyczne uzyskanie adresu IP  
- [ ] c) Uzyskanie adresu IP odbiorcy  
- [ ] d) Przetłumaczenie domeny na IP  
- [x] e) Uzyskanie adresu bramy domyślnej  

## 18. Zadaniem której warstwy jest routing pakietów?

- [ ] a) Warstwa aplikacji  
- [x] b) Warstwa sieciowa  
- [ ] c) Warstwa łącza danych  
- [ ] d) Warstwa transportowa  

## 19. Czy adresy `126.12.5.3` i `126.12.6.3` są w tej samej podsieci, jeśli identyfikacja podsieci to 8 bitów?

- [x] a) Tak  
- [ ] b) Nie  
- [ ] c) Nie da się jednoznacznie odpowiedzieć

<details>
<summary>💡 Wyjaśnienie</summary>
Maska /8 to domyślna klasa A (255.0.0.0). Dodając 8 bitów na podsieć, mamy maskę /16 (255.255.0.0).
Adresy różnią się na trzecim oktetie (5 vs 6), ale mają takie same dwa pierwsze oktety (126.12), więc z maską /16 należą do tej samej podsieci.
</details>

## 20. Które zdanie opisuje routing statyczny?

- [x] a) Administrator ręcznie wstawia trasy do tablicy  
- [ ] b) Trasy są zdefiniowane w statycznej tablicy RARP  
- [ ] c) Trasy są automatycznie dodawane  
- [ ] d) Trasy pobierane są z serwera nazw  

## 21. Dla adresu `192.168.10.131` z maską `255.255.255.192`, adres podsieci to:

- [ ] a) 192.168.10.192  
- [x] b) 192.168.10.128  
- [ ] c) 192.168.10.0  
- [ ] d) 192.168.0.0  

## 22. Protokół ARP służy do wyznaczenia:

- [ ] a) Adresu IP hosta na podstawie jego MAC  
- [x] b) Adresu MAC hosta na podstawie jego IP  
- [ ] c) Źródłowego IP na podstawie MAC  
- [ ] d) Numeru portu urządzenia  

## 23. W protokołach routingu dynamicznego metryka określa:

- [ ] a) Odległość do sieci docelowej  
- [ ] b) Odległość z sieci źródłowej do docelowej  
- [ ] c) Liczbę przeskoków z sieci źródłowej do docelowej  

## 24. Protokół ARP służy do:

- [ ] a) Przydzielenia adresu Ethernet dla hostów bezdyskowych  
- [ ] b) Przydzielenia adresu IP dla hostów bezdyskowych  
- [x] c) Znalezienia adresu MAC na podstawie IP  
- [ ] d) Znalezienia adresu IP na podstawie MAC  

## 25. Co się stanie, gdy router otrzyma datagram IP z polem TTL = 1?

- [ ] a) TTL zostanie zmniejszone i datagram przesłany dalej  
- [ ] b) Datagram zostanie odrzucony, a ICMP zgłosi błąd trasy  
- [ ] c) Datagram zostanie odrzucony bez powiadomienia  
- [ ] d) Datagram zostanie odrzucony, a ICMP zgłosi przekroczony czas życia  

## 26. Adres multicast to:

- [ ] a) Pakiety zawsze przekazywane przez routery  
- [x] b) Adres rozgłoszeniowy do grupy urządzeń  
- [ ] c) Adres klasy E  
- [x] d) Adres klasy D  
- [ ] e) Adres broadcastowy  

## 27. Dwie stacje w różnych sieciach połączone przez jeden router:

- [x] a) Muszą mieć ustawiony adres bramki  
- [ ] b) Muszą mieć taką samą maskę  
- [ ] c) Router wymaga statycznych tras domyślnych  

## 28. Adres odbiorcy ramki zawierającej żądanie ARP to:

- [x] a) MAC broadcastowy  
- [ ] b) IP bramy domyślnej  
- [ ] c) MAC bramy domyślnej  
- [ ] d) IP broadcastowy  

## 29. Który protokół informuje o błędach transmisji IP?

- [?] a) IGMP  
- [ ] b) SMTP  
- [x] c) ICMP  
- [ ] d) RARP  

## 30. Co się stanie, jeśli datagram IP przekracza MTU?

- [ ] a) Zostanie odrzucony z komunikatem ICMP „sieć nieosiągalna”  
- [ ] b) Zostanie odrzucony bez komunikatu  
- [x] c) Zostanie pofragmentowany i przesłany  
- [ ] d) Zostanie odrzucony z komunikatem ICMP „źródło stłumione”  



## 31. Suma kontrolna w nagłówku pakietu IP dotyczy:

- [ ] a) Całego pakietu (nagłówek + dane)  
- [ ] b) Tylko nagłówka  
- [ ] c) Tylko danych  

## 32. Ponowne złożenie pakietu IP po fragmentacji odbywa się:

- [x] a) U węzła-odbiorcy  
- [ ] b) Na routerze najbliższego przeskoku  
- [ ] c) Na najbliższym routerze, który ma wystarczające MTU  

## 33. W której warstwie modelu OSI działa protokół ICMP?

- [ ] a) Warstwa łącza danych  
- [x] b) Warstwa sieci  
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
- [x] c) Metryka do sieci docelowej  

## 38. Adres `112.10.3.4` należy do klasy:

- [x] a) A  
- [ ] b) B  
- [ ] c) C  
- [ ] d) D  

## 39. Tablica ARP zawiera:

- [ ] a) Adres IP bramy domyślnej  
- [x] b) MAC hosta obcego  
- [x] c) Typ wpisu (statyczny/dynamiczny)  
- [x] d) IP hosta obcego  
- [ ] e) Numer portu przełącznika, do którego podłączony jest host  

## 40. Aby hosty `192.172.16.41` i `192.172.16.27` były w tej samej podsieci, maska powinna wynosić:

- [ ] a) 255.255.255.240  
- [ ] b) 255.255.255.224  
- [ ] c) 255.255.255.248  
- [ ] d) 255.255.255.192  

## 41. Co oznacza skrót DTE?
- [ ] a) Klasą urządzeń, do której można zaliczyć switch  
- [ ] b) Rodzaj kabla do przyłączenia konsol  
- [ ] c) Rodzaj kabli wykorzystywanych w sieciach Ethernet  
- [x] d) Klasą urządzeń, do której można zaliczyć router  

## 42. Zadaniem warstwy 1 modelu OSI/ISO jest:
- [ ] a) Adresacja fizyczna  
- [ ] b) Ramkowanie  
- [ ] c) Kompresja danych  
- [x] d) Kodowanie strumienia danych do postaci odpowiedniej dla medium  
- [ ] e) Zapewnienie dostępu do medium  

## 43. Poprawnym adresem grupowym (multicastowym) Ethernet jest:
- [x] a) 01:00:5e:30:a3:d0  
- [ ] b) f0:aa:0d:23:10:01  
- [ ] c) 0b:0b:09:01:03:02  
- [ ] d) 02:00:5e:92:ff:c1  
- [ ] e) 10:2a:3c:ff:ff:ff  

## 44. W protokołach routingu dynamicznego metryka używana jest do określania:
- [ ] a) Odległości z sieci źródłowej do sieci docelowej pakietu  
- [ ] b) Opóźnienia pakietów na interfejsach wyjściowych  
- [ ] c) Liczby przeskoków z sieci źródłowej do sieci docelowej  
- [ ] d) Odległości do sieci docelowej pakietu  

## 45. Dwie stacje w różnych sieciach połączone przez jeden router:
- [ ] a) Na routerze konieczne jest dodanie pozycji routingu statycznego lub działanie protokołu routowania  
- [ ] b) Obydwie stacje muszą posiadać jednakową maskę  
- [x] c) Każda stacja musi mieć ustawiony adres IP bramy  

## 46. Kontrola przepływu w TCP polega m.in. na tym, że:
- [ ] a) Odbiorca przesyła do nadawcy informacje o pakietach, które do niego dotarły  
- [ ] b) Odbiorca kontroluje ilość danych, które może odebrać  
- [ ] c) Odbiorca przesyła do nadawcy informacje o pakietach, które do niego **nie** dotarły  
- [ ] d) Nadawca kontroluje ilość danych, które może nadać  

## 47. W protokole UDP:
- [ ] a) Przesyłanie datagramów jest niezawodne  
- [ ] b) Odbiorca potwierdza otrzymanie datagramów  
- [ ] c) Nie można fragmentować datagramów  
- [ ] d) Przesyłanie możliwe tylko w konfiguracji punkt–wielopunkt (multicast)  

## 48. Jaki jest cel uzgadniania trójetapowego (3-way handshake) w TCP?
- [ ] a) Weryfikowanie adresów IP nadawcy i odbiorcy  
- [ ] b) Określenie liczby bajtów w każdym segmencie  
- [ ] c) Synchronizacja numerów sekwencji  
- [ ] d) Dostosowanie etapów szyfrowania pakietów  

## 49. Adres `195.225.0.0` jest adresem:
- [ ] a) Sieci  
- [ ] b) Podsieci  
- [ ] c) Grupy hostów  
- [ ] d) Pojedynczego urządzenia  

## 50. Mechanizm split horizon a zliczanie do nieskończoności:
- [ ] a) Może nadal wystąpić, jego zastosowanie zmniejsza tylko ruch w sieci  
- [x] b) Może nadal wystąpić, ale rzadziej  
- [ ] c) Nie może wystąpić  

## 51. Aby hosty `197.11.199.41` i `197.11.199.27` były w tej samej podsieci, maska powinna wynosić:
- [ ] a) 255.255.255.248  
- [ ] b) 255.255.255.224  
- [ ] c) 255.255.255.240  
- [ ] d) 255.255.255.192 

## 52. Adres `192.10.13.42` należy do klasy adresów:
- [ ] a) A  
- [ ] b) B  
- [x] c) C  
- [ ] d) D  

## 53. Jakie mechanizmy umożliwiają komunikację pomiędzy przełącznicami (z włączonymi sieciami VLAN)?
- [ ] a) Synchronizacja ramek  
- [x] b) Tagowanie ramek  
- [ ] c) FCS  
- [ ] d) Fragmentacja ramek  
- [ ] e) TDM (Time Division Multiplexing)  

## 54. Dla adresu `220.1.1.133` z maską `255.255.255.192`:
- [ ] a) Adres podsieci to 220.1.1.128  
- [ ] b) Adres rozgłoszeniowy to 220.1.255.255  
- [ ] c) Adres podsieci to 220.1.1.103  
- [ ] d) Adres rozgłoszeniowy to 220.1.1.255  
- [ ] e) Adres podsieci to 220.1.1.0  

## 55. Dla adresu `23.194.10.131` z maską `255.255.248.0` adres podsieci to:
- [ ] a) 23.194.10.0  
- [ ] b) 23.194.8.0  
- [ ] c) 23.194.248.0  
- [ ] d) 23.194.0.0  

## 56. Czy adresy IP `100.22.6.2` oraz `100.32.6.3` należą do tej samej podsieci, jeśli do identyfikacji podsieci przeznaczono 8 bitów?
- [ ] a) Tak  
- [ ] b) Nie da się jednoznacznie odpowiedzieć  
- [ ] c) Nie  

## 57. Tablica ARP zawiera:
- [ ] a) Adres IP bramy domyślnej  
- [ ] b) Adres IP hosta źródłowego  
- [x] c) Typ wpisu (statyczny/dynamiczny)  
- [ ] d) Numer portu, na którym jest podłączony obcy host  
- [x] e) Adres MAC hosta obcego  

## 58. Które pole występuje zarówno w nagłówku segmentu UDP, jak i TCP?
- [ ] a) Numer potwierdzenia  
- [ ] b) Numer portu  
- [ ] c) Rozmiar okna  
- [ ] d) Numer kolejny  

## 59. Skąd IP wie, gdzie dostarczyć pakiet o wskazanym adresie IP?
- [ ] a) Wszystkie powyższe odpowiedzi są poprawne  
- [ ] b) Do określenia trasy pakietu, IP korzysta z protokołu sterującego ICMP  
- [ ] c) Żadna z powyższych odpowiedzi nie jest poprawna  
- [ ] d) W datagramie IP zapisany jest adres routera następnego przejścia  
- [ ] e) W tablicy routingu zapisana jest trasa, którą ma przebiegać pakiet  

## 60. Datagram IP:
- [ ] a) Wskazuje trasę przesłania go poprzez sieć  
- [ ] b) Pozwala uzyskać adres innego hosta (np. odbiorcy)  
- [ ] c) Posiada sumę kontrolną całego pakietu  
- [ ] d) Ma zmienną długość  
- [ ] e) Nie może być wysłany multicastowo  

## 61. Dla adresu `194.0.10.141` z maską `255.255.255.192` prawdziwe są stwierdzenia:
- [ ] a) W podsieci jest 62 dostępne adresy użyteczne  
- [ ] b) Na numer hosta przeznaczone jest 6 bitów  
- [ ] c) W podsieci jest 64 dostępne adresy użyteczne  
- [ ] d) W podsieci jest 30 dostępnych adresów użytecznych  
- [ ] e) Na numer hosta przeznaczonych jest 3 bity  

## 62. Co się stanie, gdy datagram IP ma rozmiar większy niż MTU sieci, do której jest wysyłany?
- [ ] a) Pakiet zostanie odrzucony "po cichu"  
- [ ] b) Pakiet zostanie odrzucony i wygenerowany zostanie komunikat ICMP sieć nieosiągalna  
- [ ] c) Pakiet zostanie odrzucony i wygenerowany zostanie komunikat ICMP stłumienie źródła  
- [x] d) Pakiet zostanie podzielony na fragmenty i wysłany  

## 63. Który z wymienionych protokołów jest protokołem bezpołączeniowym?
- [ ] a) UDP  
- [ ] b) TCP  
- [ ] c) ARP  
- [ ] d) IP  

## 64. Połączono bezpośrednio ze sobą komputery:  
Host A - `120.0.0.10/22`, Host B - `120.10.0.0/12`. Które stwierdzenie jest prawdziwe?
- [ ] a) Komputer B NIE wyśle poprawnie pakietu do komputera A  
- [ ] b) Komputer B poprawnie wyśle pakiet do komputera A  
- [ ] c) Komputer A NIE wyśle poprawnie pakietu do komputera B  
- [ ] d) Komputer A poprawnie wyśle pakiet do komputera B  

## 65. Jakie są podstawowe zadania warstwy transportowej w modelu OSI?
- [x] a) Połączenia typu end-to-end  
- [ ] b) Szyfrowanie danych  
- [ ] c) Wybór ścieżki  

## 66. Adres IP multicast to:
- [x] a) Adres klasy D  
- [ ] b) Pakiety wysyłane na taki adres zawsze przekazywane są przez rutery  
- [ ] c) Adres klasy E  
- [ ] d) Adres rozgłoszeniowy do wszystkich urządzeń w sieci  
- [x] e) Adres rozgłoszeniowy do grupy urządzeń  

## 67. Dla adresu `191.0.10.1` z maską `255.255.255.224` prawdziwe są stwierdzenia:
- [ ] a) Na numer hosta przeznaczone jest 5 bitów  
- [ ] b) W podsieci jest 30 dostępnych adresów użytecznych  
- [ ] c) Na numer hosta przeznaczonych jest 3 bity  
- [ ] d) W podsieci jest 32 dostępne adresy użyteczne  
- [ ] e) W podsieci jest 62 dostępne adresy użyteczne  

## 68. Protokół IP posiada następujące cechy:
- [ ] a) Przesłanie pakietu poprzedza faza uzgodnienia połączenia  
- [ ] b) Jest protokołem połączeniowym  
- [ ] c) Zawiera mechanizmy potwierdzania doręczenia pakietów  
- [ ] d) Jest protokołem niezawodnym  
- [ ] e) Zabezpiecza przed krążeniem pakietów w sieci  

## 69. Który protokół jest używany do powiadamiania hosta IP o błędach transmisji?
- [x] a) ICMP  
- [ ] b) RARP  
- [ ] c) SMTP  
- [?] d) IGMP  

## 70. Jakie mechanizmy zapobiegają wyczerpaniu przestrzeni adresowej IPv4?
- [ ] a) Routing bezklasowy  
- [ ] b) DHCP  
- [ ] c) ARP  
- [x] d) NAT  

