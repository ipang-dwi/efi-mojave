# efi-mojave
efi partition files for install mojave on asus x45c

Copas saja semua yang ada di dalam folder EFI ke partisi EFI pada USB installer mojave yang telah dibuat.. Proses load pertama kali akan agak lama, tampilan kaya' diulang-ulang, tapi sabar saja.. Hanya seakan-akan looping, tapi sebenarnya itu proses virtualsmc, untuk menggenerate fake info hackintosh sesuai file config.plist..

Setelah selesai install dan sudah menginstall clover di hdd/ssd, buka file config.plist pada line 208 :

<string>kext-dev-mode=1 dart=0 slide=0 nv_disable=1 -cdfon -igfxnohdmi -no_compat_check -v -f</string>

Hapus opsi -v, atau bisa juga disetting pada saat booting di clover..

Feel free to reach me on :
https://www.firstplato.com
https://www.facebook.com/firstplato
admin@firstplato.com
