# DNS Ayarları - screentranslate.com → GitHub Pages

## ⏳ ÖNCELİKLE KONTROL ET

GitHub Pages build durumunu kontrol et:
```bash
gh api repos/esarikaya-ops/screentranslate-web/pages --jq .status
```
**"built" gösterene kadar DNS değiştirme!** (2-5 dakika sürer)

---

## 🔧 DNS KAYITLARI (screentranslate.com)

### 1. Apex (@) A Kayıtları
**Mevcut IP'leri SİL, bunları ekle:**
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

### 2. www CNAME Kaydı
```
www → esarikaya-ops.github.io
```

---

## 📋 KESİNTİSİZ GEÇİŞ PLANI

1. **GitHub Pages build tamamlandı mı?** → Yukarıdaki komutu çalıştır
2. **DNS'i değiştir** → Apex A kayıtları + www CNAME
3. **DNS yayılmasını bekle** → 10 dk - 48 saat (genelde 1-2 saat)
4. **Test et:**
   ```bash
   curl -I http://screentranslate.com
   # Location: https://screentranslate.com görmeli
   ```
5. **HTTPS aktifleştir** (DNS yayılınca):
   - https://github.com/esarikaya-ops/screentranslate-web/settings/pages
   - "Enforce HTTPS" ✓ işaretle
   - SSL sertifikası otomatik (Let's Encrypt, 1-2 saat)

6. **Eski hosting'i kapat** → DNS yayılınca (veri kaybı riski yok - GitHub'da yedek)

---

## ✅ TEST LİSTESİ (DNS yayılınca)

- [ ] http://screentranslate.com → index.html yükleniyor
- [ ] http://www.screentranslate.com → redirect ediyor
- [ ] http://screentranslate.com/nasil-kullanilir → yeni sayfa
- [ ] http://screentranslate.com/gizlilik-politikasi → Android paywall linki çalışıyor
- [ ] http://screentranslate.com/kullanici-sozlesmesi → Android paywall linki çalışıyor
- [ ] HTTPS aktif mi? → https://screentranslate.com yeşil kilit

---

## 🔗 REPO BİLGİLERİ

- **GitHub Repo:** https://github.com/esarikaya-ops/screentranslate-web
- **Pages URL:** http://screentranslate.com/ (DNS yayılınca)
- **Branch:** master
- **CNAME:** screentranslate.com

---

## 🚨 SORUN GİDERME

**DNS yayılmadı mı?** (48 saat sonra)
```bash
# DNS kontrolü
nslookup screentranslate.com
# 185.199.10x.153 IP'lerini görmeli

# CNAME kontrolü
nslookup www.screentranslate.com
# esarikaya-ops.github.io görmeli
```

**HTTPS hatası alıyorum:**
- GitHub Pages Settings → "Enforce HTTPS" kapalı mı kontrol et
- 24 saat bekle (SSL sertifikası oluşması zaman alabilir)
- Tarayıcı cache'ini temizle (Ctrl+Shift+Del)

**Site yüklenmiyor:**
- GitHub Pages status kontrol: `gh api repos/esarikaya-ops/screentranslate-web/pages`
- DNS yayılması tamamlandı mı: `nslookup screentranslate.com`
- GitHub Pages down mu: https://www.githubstatus.com/
