# Bar UniScreen

Windows app for the Lian Li 8.8" Universal Screen (480 × 1920 LCD with ARGB frame).
Shows CPU, GPU, RAM, disk, network and clock with themes and ARGB effects. No L-Connect needed.

Lian Li 8.8" Universal Screen için Windows uygulaması: CPU, GPU, RAM, disk, ağ ve saat göstergeleri,
temalar ve ARGB efektleri. L-Connect gerekmez.

## İndir / Download

**[Son sürümü indir (Bar-UniScreen-Setup)](https://github.com/felicrutter/bar-uniscreen-releases/releases/latest)**

1. `Bar-UniScreen-Setup-x.y.z.exe` dosyasını indirip çalıştırın. Yönetici izni gerekmez.
2. Windows "Windows bilgisayarınızı korudu" uyarısı gösterirse **Ek bilgi → Yine de çalıştır** seçin
   (kurulum dosyası imzalı değildir).
3. Uygulama sistem tepsisinde çalışır. Ayarlar için tepsi simgesine çift tıklayın.

Güncellemeler: uygulama yeni sürümü kendisi bulur ve kurmadan önce sorar
(Ayarlar → Genel → Güncellemeler).

Requirements: Windows 10/11 x64, .NET Framework 4.8 (built into Windows 10 1903+ and Windows 11).

## Sensörler / Sensors

Sensors are built in and need no driver: GPU (AMD/NVIDIA), CPU load/power/clock, RAM, disk temperature,
network. CPU temperature needs a kernel driver on Windows: run HWiNFO (shared memory / gadget) or enable
the optional PawnIO setting (Intel MSR only). Bar UniScreen never installs drivers.

## Notes

This repository only hosts releases; the source code is private.
Bar UniScreen is an independent project and is not affiliated with or endorsed by Lian Li.
Third-party licenses: [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).
