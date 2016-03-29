## Türkiye İl-İlçe Veritabanı Yapısı

Türkiye il ve ilçelerini veritabanında tutmanıza yarayan, mysql formatında hazırlanmış dump dosyası

Sıralama problemlerini aşmak için extra alan eklendi.

# h1 TOPLU SLUG
update cities set slug = lower(name) where 1;
update cities set slug = replace(slug,'ğ','g') where 1;
update cities set slug = replace(slug,'ü','u') where 1;
update cities set slug = replace(slug,'ş','s') where 1;
update cities set slug = replace(slug,'ç','c') where 1;
update cities set slug = replace(slug,'ı','i') where 1;
update cities set slug = replace(slug,'ö','o') where 1;


update counties set slug = lower(name) where 1;
update counties set slug = replace(slug,'ğ','g') where 1;
update counties set slug = replace(slug,'ü','u') where 1;
update counties set slug = replace(slug,'ş','s') where 1;
update counties set slug = replace(slug,'ç','c') where 1;
update counties set slug = replace(slug,'ı','i') where 1;
update counties set slug = replace(slug,'ö','o') where 1;
