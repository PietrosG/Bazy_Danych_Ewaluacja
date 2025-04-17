# Bazy_Danych_Ewaluacja
Zadania Ewaluacyjne

## Zadanie 1
```sql
select nazwa_towaru from towar
order by nazwa_towaru asc
```
## Zadanie 2

```sql
select * from pracownik
order by pensja desc
limit 5;
```

## Zadanie 3

```sql
SELECT MAX(id_towaru * cena_zakupu) FROM towar;
```
## Zadanie 4

```sql
select nazwa_statusu_zamowienia from status_zamowienia as z
left join zamowienie as sz on z.id_statusu_zamowienia = sz.status_zamowienia
where sz.status_zamowienia is null;
```

## Zadanie 5

```sql
select nazwa_kategori, count(t.kategoria) from kategoria as k 
left join towar as t on k.nazwa_kategori = t.kategoria
group by k.nazwa_kategori
```
