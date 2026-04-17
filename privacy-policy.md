# Privacy Policy — Fridge

**Effective date:** 2026-04-17
**Contact:** mkceliks@gmail.com

> This document is available in English below and Turkish at the bottom.

---

## English

### 1. Who we are
"Fridge" ("we", "us", or "the App") is operated by Mustafa Kemal Çelik, Mersin, Türkiye. We can be reached at **mkceliks@gmail.com**.

### 2. What we collect

**Account data (required)**
- Email address (from Apple Sign-In, Google Sign-In, or magic-link verification)
- A display name you provide
- Your chosen @handle

**Profile data (optional)**
- Profile photo you upload
- Phone number in E.164 format, if you opt in to contact-based friend discovery
- Language preference and time zone

**Content you create (required to use the product)**
- Tracker configurations (name, icon, template)
- Daily entries: text notes, numeric fields, photos you attach, timestamps
- Reactions and comments on your own entries and entries shared with you as a supporter
- Invite codes you create or accept

**Device + usage data**
- A push notification token (provided by Apple/Google) so we can notify you of reactions, comments, invites, reminders, and weekly digests
- Telemetry events (e.g. `tracker_created`, `entry_created`, `app_opened`) — device-anonymous except for the user id we already associate with your account
- Crash and performance logs via Expo (aggregate device model, OS version, app version, stack traces)

**Contact matching (opt-in only)**
- If you grant Contacts permission, we send one-way HMAC-SHA256 hashes of your contacts' phone numbers to match you with Fridge users. The plaintext numbers **never leave your device**. Only the hashes are transmitted, and only hashes that match an existing Fridge user are returned to your device.

### 3. What we do NOT collect
- We do **not** collect plaintext phone numbers of your contacts.
- We do **not** sell, rent, or share your personal data with advertisers.
- We do **not** use third-party advertising SDKs.
- We do **not** read the content of your photos for any purpose other than displaying them to you and the supporters you invite.
- We do **not** track you across other apps or websites.

### 4. Why we collect it (legal basis under GDPR / KVKK)
- **Providing the service (contract):** account data, tracker data, entries, invites, reactions, comments.
- **Authentication and abuse prevention (legitimate interest):** auth tokens, rate-limit counters, telemetry.
- **Push notifications (consent):** push token — revocable by disabling notifications in iOS/Android settings.
- **Contact-matching (explicit opt-in consent):** phone hash exchange. Revocable by revoking Contacts permission and/or deleting your phone number from your profile.

### 5. Who sees your content
- **You:** everything you create.
- **Supporters you explicitly invite:** the specific tracker you invited them to, its entries (including photos + notes), your reactions and comments.
- **No one else** sees your trackers or entries. A user who guesses your username or email cannot access your data.
- Supporters can react and comment; you can delete your own comments and revoke any supporter at any time.

### 6. Storage + security
- Content is stored on Cloudflare R2 (private bucket, US/EU region) and Railway-hosted PostgreSQL (EU region).
- Image access is authenticated: only you and your active supporters can fetch your photos.
- Phone numbers, when provided, are HMAC-SHA256 hashed with a server-held pepper before being compared against other users' hashes. We never compare plaintext.
- All connections are TLS-encrypted.

### 7. Retention
- Entries, photos, and trackers are retained while your account is active.
- Deleted (archived) trackers and soft-deleted comments remain in our database for up to 30 days after deletion, then are hard-deleted.
- Inactive accounts: we may delete accounts that have been unused for 24 consecutive months, after a 30-day email warning.
- You can delete your account at any time from **Settings → Delete account**. Upon deletion, personal data is erased within 30 days (except where law requires longer retention).

### 8. Your rights (GDPR / KVKK)
You have the right to:
- Access a copy of your data (email **mkceliks@gmail.com** — we respond within 30 days).
- Correct inaccurate data (directly in Settings, or by email).
- Delete your account and all associated data.
- Object to or restrict processing of your data (email us).
- Port your data to another service in a machine-readable format.
- Lodge a complaint with your local data protection authority (Türkiye: KVKK / `kvkk.gov.tr`; EU: your country's DPA).

### 9. Children
Fridge is not intended for users under 13 (or under 16 in GDPR jurisdictions requiring parental consent for data processing). We do not knowingly collect data from children. If you believe a child has signed up, email **mkceliks@gmail.com** and we will delete the account.

### 10. Third-party services
We use the following service providers strictly for the functions listed:
- **Cloudflare R2** — image storage.
- **Railway** — application hosting, PostgreSQL database.
- **Expo** — mobile build, OTA updates, push-notification routing.
- **Resend** — transactional email (magic-link codes).
- **Apple + Google** — OAuth sign-in, push-notification delivery, App Store / Play Store distribution.

Each processor has its own privacy commitments; we do not pass them more data than they need to operate.

### 11. International transfers
Your data may be processed in the EU, US, or Türkiye depending on which service handles the request. Where transfers outside your home jurisdiction occur, they rely on Standard Contractual Clauses or equivalent safeguards.

### 12. Changes
We will notify you of material changes to this policy via in-app notification and an update to the "Effective date" at the top of this document. Continued use after a change constitutes acceptance.

---

## Türkçe

### 1. Kimiz?
"Fridge" ("biz" ya da "Uygulama") Mustafa Kemal Çelik tarafından Mersin, Türkiye'den işletiliyor. İletişim: **mkceliks@gmail.com**.

### 2. Topladığımız veriler

**Hesap bilgileri (zorunlu)**
- E-posta adresi (Apple, Google ya da giriş bağlantısı doğrulamasıyla)
- Belirlediğin isim
- Seçtiğin @kullanıcı adı

**Profil bilgileri (opsiyonel)**
- Yüklediğin profil fotoğrafı
- Telefon numarası (E.164 formatında) — yalnızca rehber eşleştirmeyi açtıysan
- Dil tercihi ve saat dilimi

**Oluşturduğun içerik (ürünü kullanmak için gerekli)**
- Takip yapılandırmaları (ad, simge, şablon)
- Günlük kayıtlar: notlar, sayısal alanlar, eklediğin fotoğraflar, zaman damgaları
- Kendi kayıtlarına ya da destekçisi olduğun kayıtlara verdiğin tepkiler ve yorumlar
- Oluşturduğun ya da kabul ettiğin davet kodları

**Cihaz + kullanım verisi**
- Bildirim gönderebilmek için push-notification token (Apple/Google üzerinden)
- Telemetri olayları (`tracker_created`, `entry_created`, `app_opened` gibi)
- Expo üzerinden toplanan cihaz modeli, işletim sistemi sürümü, uygulama sürümü ve çökme/performans logları

**Rehber eşleşmesi (yalnızca sen açarsan)**
- Rehber iznini verirsen, rehberindeki numaraların HMAC-SHA256 tek yönlü özetleri sunucuya gönderilir. **Numaralar telefonundan açık metin olarak asla çıkmaz.** Sadece Fridge'de kayıtlı olanların özetleri eşleşme olarak geri döner.

### 3. Toplamadıklarımız
- Rehberindeki kişilerin **telefon numaralarını açık metin olarak toplamayız.**
- Kişisel veriyi **reklamverene satmaz, kiralamaz, paylaşmayız.**
- **Üçüncü taraf reklam SDK'sı kullanmayız.**
- Fotoğraflarının içeriğini, sana ve davet ettiğin destekçilere göstermek dışında hiçbir amaçla okumayız.
- Başka uygulama ya da web sitelerinde seni takip etmeyiz.

### 4. Neden topluyoruz (KVKK / GDPR hukuki dayanak)
- **Hizmetin sağlanması (sözleşme):** hesap, takip, kayıt, davet, tepki, yorum verisi.
- **Kimlik doğrulama ve kötüye kullanımın önlenmesi (meşru menfaat):** auth token'ları, rate-limit sayaçları, telemetri.
- **Bildirimler (açık rıza):** push token — iOS/Android bildirim ayarlarından kapatabilirsin.
- **Rehber eşleşmesi (açık rıza):** telefon özeti — rehber iznini kaldırarak ya da profilinden telefonu silerek iptal edebilirsin.

### 5. İçeriğini kimler görür?
- **Sen:** oluşturduğun her şey.
- **Davet ettiğin destekçiler:** yalnızca onları davet ettiğin belirli takip + o takibin kayıtları (fotoğraflar ve notlar dâhil) + tepkiler + yorumlar.
- **Başka kimse** takibine ya da kaydına erişemez. Kullanıcı adını tahmin eden biri verilerine ulaşamaz.
- Destekçiler tepki bırakıp yorum yazabilir; kendi yorumlarını silebilirler. Sen de istediğin an bir destekçiyi kaldırabilirsin.

### 6. Depolama + güvenlik
- İçerik Cloudflare R2 (özel bucket, AB/ABD bölgesi) ve Railway üzerindeki PostgreSQL'de (AB bölgesi) saklanır.
- Görsel erişimi kimlik doğrulamalıdır: yalnızca sen ve aktif destekçilerin fotoğraflarına ulaşabilir.
- Telefon numaraları (verildiğinde), karşılaştırmadan önce sunucuda tutulan bir "pepper" ile HMAC-SHA256 özetine çevrilir. Açık metin karşılaştırma yapmayız.
- Tüm bağlantılar TLS ile şifrelenir.

### 7. Saklama süresi
- Kayıtlar, fotoğraflar ve takipler, hesabın aktif olduğu sürece saklanır.
- Silinen (arşivlenen) takipler ve soft-delete edilmiş yorumlar veritabanında 30 güne kadar tutulur, sonra kalıcı olarak silinir.
- Aktif olmayan hesaplar: Üst üste 24 ay kullanılmayan hesaplar, 30 günlük e-posta uyarısının ardından silinebilir.
- **Ayarlar → Hesabı sil** yolundan istediğin zaman hesabını silebilirsin. Silme sonrası kişisel verilerin 30 gün içinde tamamen temizlenir (yasal zorunluluk aksini gerektirmiyorsa).

### 8. Haklarınız (KVKK / GDPR)
- Verilerinin bir kopyasını almak (**mkceliks@gmail.com** — 30 gün içinde yanıt).
- Yanlış veriyi düzeltmek (Ayarlar'dan doğrudan ya da e-posta ile).
- Hesabını ve ilgili tüm veriyi silmek.
- İşlemeye itiraz etmek ya da sınırlamak.
- Verini makineyle okunabilir biçimde başka bir servise taşımak.
- Yerel veri koruma otoritesine şikâyette bulunmak (Türkiye: **kvkk.gov.tr** üzerinden KVKK).

### 9. Çocuklar
Fridge, 13 yaş altına (GDPR kapsamında 16 yaş altına) yönelik değildir. Bilerek çocuklardan veri toplamayız. Bir çocuğun kaydolduğunu düşünüyorsan **mkceliks@gmail.com** adresine yaz, hesabı silelim.

### 10. Üçüncü taraf servisler
Yalnızca listelenen işlevler için kullanırız:
- **Cloudflare R2** — görsel depolama.
- **Railway** — uygulama ve PostgreSQL hosting.
- **Expo** — mobil build, OTA güncelleme, push yönlendirmesi.
- **Resend** — işlemsel e-posta (giriş bağlantısı kodları).
- **Apple + Google** — OAuth, push iletimi, App Store / Play Store dağıtımı.

Her alt işleyiciye yalnızca işini yapacak kadar veri aktarılır.

### 11. Uluslararası aktarım
Verilerin, talebi karşılayan servise bağlı olarak AB, ABD ya da Türkiye'de işlenebilir. Yurt dışı aktarımlar Standart Sözleşme Maddeleri ya da eşdeğeri güvenceler altında yapılır.

### 12. Değişiklikler
Bu politikadaki önemli değişiklikleri uygulama içi bildirim ve yukarıdaki "Yürürlük tarihi"nin güncellenmesiyle duyururuz. Sonraki kullanım kabul anlamına gelir.
