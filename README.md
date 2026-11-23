# ynk.studio

Yeni Nesil Kafası web sitesi. Düz HTML; derleme adımı yok.

- `index.html` ana sayfa (ekip ve içerik bölümleri veritabanından gelir)
- `kvkk.html` KVKK aydınlatma metni (`/kvkk`)
- `admin.html` yönetim paneli (`/admin`): analitik, aboneler, başvurular, ekip, içerikler
- `ekibe-katil.html` davetle doldurulan ekip formu (`/ekibe-katil?k=<davet kodu>`); talepler admin'de onay bekler
- `vercel.json` temiz adresler ve logo yönlendirmesi

Veriler wapimusic Supabase projesindeki `ynk_` ön ekli tablolarda durur.

Tıklamalar `ynk_page_views` tablosuna `click:<etiket>` adıyla yazılır; admin bunları sayfa görüntülemelerinden ayırır.
