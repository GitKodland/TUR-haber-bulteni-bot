# Haber Bülteni Botu

### Komutlar:

- **!news**: Belirtilen bir RSS kaynağından haberleri alır ve görüntüler.
- **!subscribe**: Bir kullanıcıya anahtar kelime ile bildirimlere abone olma imkanı sunar.
- **!unsubscribe**: Bir kullanıcıya anahtar kelime ile bildirim aboneliğinden çıkma imkanı sunar.
- **!notifications**: Kullanıcının mevcut aboneliklerini gösterir.
- **!latest**: Kullanıcının tüm abonelikleri için en son haberleri görüntüler
- **!info**: Bot hakkında bilgi verir.

### Arka Plan Görevi:

**update_news**:  Her 10 dakikada bir haberleri günceller ve başlık, aboneliklerden bir anahtar kelime içeriyorsa önbelleğe kaydeder.

### Veri Yapısı:

**subscriptions**: Kullanıcı aboneliklerini depolamak için bir sözlük.  
**news_cache**: Anahtar kelimelerle ilgili haberleri depolamak için bir önbellek.

### RSS Ayrıştırıcı:

Haberleri RSS kaynaklarından almak için **feedparser** kütüphanesini kullanır.
