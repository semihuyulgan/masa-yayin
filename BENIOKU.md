# masa-yayin

@masaoyun Instagram hesabının otomatik yayın deposu (Maison Eva sisteminin kopyası).

- `takvim.json`: paylaşımlar ve durumları (hazir → isleniyor → yayinda / hata / belirsiz). Elle güncellenir, önce `git pull`.
- `yayinci.py`: GitHub Actions 15 dakikada bir çalıştırır, zamanı gelen `hazir` içeriği yayımlar. `--deneme` ile yalnızca listeler.
- `medya/`: görseller (JPEG) ve videolar (MP4). Görseller raw.githubusercontent'ten, videolar GitHub Pages'ten sunulur.
- Token yalnızca `IG_TOKEN` secret'ında ve yerelde `~/.config/masa/ig_token` dosyasında durur; depoya yazılmaz.
