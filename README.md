# PatikaSQL - SQL Ödevleri

Patika.dev SQL eğitim programı kapsamında hazırlanan SQL ödevlerinin çözümlerini içerir. Bu repo, ilişkisel veritabanı yönetim sistemleri (RDBMS) ile çalışırken kullanılan temel ve ileri düzey SQL sorgularını uygulamalı olarak öğretmeyi amaçlamaktadır.

## Proje Hakkında

Tüm ödevler **PostgreSQL** ortamında ve **DVD Rental** örnek veritabanı (`film`, `actor`, `customer`, `payment`, `inventory` vb.) üzerinde uygulanmaktadır. Her ödev klasörü, ilgili konuya odaklı SQL sorgularını barındırır.

### İçerik / Ödev Listesi

| Ödev | Konu |
|------|------|
| Odev1 | Tanışma ve temel SQL kavramları |
| SQLODEV2 | `SELECT`, `WHERE`, `AND/OR`, `IN/NOT IN` operatörleri |
| SQLODEV3 | `BETWEEN` ve `IN` operatörleri |
| SQLODEV4 | `LIKE` ve karakter eşleme ile filtreleme |
| SQLODEV5 | `DISTINCT`, `COUNT` aggregate fonksiyonları |
| SQLODEV6 | `ORDER BY`, `LIMIT`, `OFFSET`, `FETCH` kullanımı |
| SQLODEV7 | `MIN`, `MAX`, `AVG`, `SUM` aggregate fonksiyonları |
| SQLODEV8 | `GROUP BY` ve `HAVING` kullanımı |
| SQLODEV9 | `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN` |
| SQLODEV10 | `UNION`, `INTERSECT`, `EXCEPT` |
| SQLODEV11 | `EXISTS`, `ANY`, `ALL` operatörleri |
| SQLODEV12 | Subquery (alt sorgu) ve `JOIN` ile kombine kullanım |

## Kullanılan SQL Özellikleri

- **DML (Data Manipulation Language)**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`
- **Filtreleme**: `WHERE`, `AND`, `OR`, `NOT`, `IN`, `BETWEEN`, `LIKE`, `ILIKE`
- **Sıralama ve sayfalama**: `ORDER BY`, `LIMIT`, `OFFSET`, `FETCH FIRST`
- **Gruplama**: `GROUP BY`, `HAVING`
- **Aggregate fonksiyonlar**: `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`
- **Joinler**: `INNER JOIN`, `LEFT/RIGHT/FULL OUTER JOIN`, `CROSS JOIN`, `SELF JOIN`
- **Küme operatörleri**: `UNION`, `UNION ALL`, `INTERSECT`, `EXCEPT`
- **Alt sorgular (Subqueries)**: Skaler, satır ve tablo bazlı alt sorgular
- **Subquery operatörleri**: `EXISTS`, `ANY`, `ALL`, `IN`

## Gereksinimler

- **PostgreSQL 13+** (önerilen)
- Bir SQL istemcisi (pgAdmin 4, DBeaver, DataGrip veya `psql`)
- **DVD Rental** örnek veritabanı

### DVD Rental Veritabanını Kurma

PostgreSQL Tutorial sayfasından örnek veritabanını indirip yükleyebilirsiniz:

```bash
createdb -U postgres dvdrental
pg_restore -U postgres -d dvdrental dvdrental.tar
```

## Nasıl Çalıştırılır?

1. PostgreSQL kurulumunu yapın ve `dvdrental` veritabanını yükleyin
2. pgAdmin ya da tercih ettiğiniz SQL istemcisi ile bağlanın
3. İlgili ödev klasörüne gidip içerisindeki SQL sorgularını query editöründe çalıştırın

```bash
psql -U postgres -d dvdrental -f SQLODEV2
```

## Notlar

> Sorgular eğitim amaçlıdır. Bazı dosyalarda yorum satırları içerisinde Türkçe karakterli (`İ`, `MİN`) anahtar kelimeler bulunabilir; PostgreSQL hata vermesi durumunda bu kelimeleri ASCII karşılıklarıyla (`MIN`, `IN`) güncelleyiniz.

## Lisans

Repoda yer alan `LICENSE` dosyasına bakınız.
