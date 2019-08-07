# efi-mojave

<img src="https://raw.githubusercontent.com/ipang-dwi/efi-mojave/master/img/ss.png" />

efi partition files for install mojave on asus x45c

Copas saja semua yang ada di dalam folder EFI ke partisi EFI pada USB installer mojave yang telah dibuat.. Proses load pertama kali akan agak lama, tampilan kaya' diulang-ulang, tapi sabar saja.. Hanya seakan-akan looping, tapi sebenarnya itu proses virtualsmc, untuk menggenerate fake info hackintosh sesuai file config.plist..

Setelah selesai install dan sudah menginstall clover di hdd/ssd, buka file config.plist pada line 208 :

<string>kext-dev-mode=1 dart=0 slide=0 nv_disable=1 -cdfon -igfxnohdmi -no_compat_check -v -f</string>

Hapus opsi -v, atau bisa juga disetting pada saat booting di clover..

Device : asus x45c
Spek : core i3 2350m, ram ddr3 4gb, ssd avexir e100 120gb, hdd hgst 500gb, vga intel hd3000

Booting pertama setelah install agak lama, perfomance juga agak bikin geregetan.. tapi setelah install kext bwt vga, overall mulus.. cman agak aneh bwt light theme, jadi prefer ke dark theme..

Yg berfungsi :
- procie, totalitas, pke config.plist device mbp9.2
- intel hd3000, smooth, no glitch, cman meski dvmt disetting 512mb di bios, tetep kedetectnya 300an..
- touchpad
- usb2 + usb3
- sata2 + sata3
- lan
- ps2 mouse+keyboard
- fn key bawaan asus, tapi tombol brighness g bisa
- sound
- sisanya liat ss aj

Yg belom fungsi :
- wifi, ud coba kext wifiinject, ar9k dari om.rehabman, belum juga fix
- brighness setting
- tombol numlock, screen lock sama ctrl, g bisa dipakai, g tau knp
- tombol back n forward di usb mouse juga g bisa dipakai, juga klo pke yg dpi nya bisa disetting, tiap login harus setting ulang lagi, ane pke rexus xierra x3.. *update : ud bisa pakai app https://sensible-side-buttons.archagon.net/
- sisanya yg g ada di ss brarti g bisa :D

Wallpaper : cabutan dari wallpaper bawaan os manjaro deepin..

Installer DMG nemu di file docs grup..

Review :
Ane g sanggup lama2 di mojave, gersang euy.. ini os paling rakus ram yg pernah ane pke.. tapi emg bener seksi ini os..

Makasih bwt kang Brilliant Edgar Rosandy atas dmg nya, Yos Beda, Badruzeus Shava n Rony Roland atas inspirasinya.. Forum FB Hackintosh Indonesia..

Logs :
07/08/2019
- tested on Mojave 10.14.16
- working perfectly..
18/07/2019 5.56PM 
- persiapan install ulang Mojave 10.14.4
- tested on Mojave 10.14.4


Feel free to reach me on :
- https://www.firstplato.com
- https://www.facebook.com/firstplato
- admin@firstplato.com
