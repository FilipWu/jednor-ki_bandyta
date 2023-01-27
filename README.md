# jednoreki_bandyta


Kod jest symulacją gry w automat do gier. Gracz może doładować swój konto, a następnie wybrać opcję zakręcenia bębnami automatu naciskając enter. Gracz może również wybrać liczbę linii do obstawienia oraz kwotę do obstawienia na każdej linii. Gra generuje losowe symbole dla automatu i sprawdza, czy gracz wygrał jakieś pieniądze na podstawie pojawiających się symboli na wygrywających liniach.


Funkcja check_winnings(columns, lines, bet, values) sprawdza, ile gracz wygrał i na jakich liniach.
Funkcja przyjmuje cztery argumenty:
columns - kolumny z symbolami na automacie,
lines - liczba linii, na których gracz obstawia,
bet - kwota, którą gracz obstawił na jedną linię,
values - wartości symboli.
Funkcja zwraca dwa argumenty:
winnings - kwotę, którą gracz wygrał oraz winning_lines - listę linii, na których wygrał.

Funkcja get_slot_machine_spin(rows, cols, symbols) generuje losowy układ symboli na automacie. Funkcja przyjmuje trzy argumenty:
rows - liczba wierszy,
cols - liczba kolumn,
symbols - słownik symboli i ich liczby.
Funkcja zwraca kolumny z symbolami na automacie.


Funkcja print_slot_machine(columns) drukuje układ symboli na automacie. Funkcja przyjmuje jeden argument:
columns - kolumny z symbolami na automacie.


Funkcja deposit() pozwala graczowi na wpłacenie pieniędzy na swoje konto. Funkcja zwraca wpłaconą kwotę.


Funkcja get_number_of_lines() pozwala graczowi na wybór liczby linii, na których chce obstawiać. Funkcja zwraca liczbę linii.


Funkcja get_bet() pozwala graczowi na wybór kwoty, którą chce obstawić na jedną linię. Funkcja zwraca kwotę.


Funkcja spin(balance) pozwala graczowi na rozpoczęcie gry. Funkcja przyjmuje jeden argument: balance - aktualny stan konta gracza. Funkcja zwraca różnicę między wygraną a wydatkami.


Funkcja main jest główną funkcją programu, która odpowiada za logikę gry. Inicjuje ona grę, umożliwiając graczowi wprowadzenie depozytu, a następnie pozwala na grę w pętlę, w której gracz może wybrać opcję zakręcenia bębnami lub zakończenia gry. Po każdym zakręceniu bębnami, stan konta gracza jest aktualizowany o wygraną lub przegraną. Po zakończeniu gry, komunikat końcowy jest wyświetlany z informacją o pozostawionych środkach.
