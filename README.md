Hakkında
=====================
Çok daha önce yazmış olduğum sayfalama sınıfımı herkes kullansın diye düzenledim. Son derece esnek olarak hazırlandı dileyenler geliştirip kullanabilirler.

Kullanımı
=====================
```php
<?php

header('Content-type: text/html; charset=utf8');
include "sPagination.class.php";

$page = new sPagination();

$page->total = 10; // Toplam data sayısı
$page->limit = 5; // Sayfada gösterilecek limit sayısı
$page->scroll = 5; // Sayfalamadaki kaydırma ayarı
$page->page = '?'; // Sayfa REQUEST_URI bilgisi
$page->request = 'page'; // Kullanılacak REQUEST değer
$page->previous_text = 'Geri'; // Geri Buton text adı
$page->next_text = 'İleri'; // İleri Buton text adı
$page->first_text = 'İlk'; // İlk Data Buton text adı
$page->end_text = 'Son'; // Son Data Buton text adı

echo $page->Paginate();

?>
```
