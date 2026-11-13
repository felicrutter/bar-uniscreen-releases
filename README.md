<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/wordmark-light.png">
    <img src="assets/wordmark-dark.png" alt="Bar UniScreen" width="420">
  </picture>
</p>

# Bar UniScreen

Windows app for the Lian Li 8.8" Universal Screen (480 × 1920 LCD with ARGB frame).
Shows CPU, GPU, RAM, disk, network and clock with themes and ARGB effects. No L-Connect needed.

Lian Li 8.8" Universal Screen için Windows uygulaması: CPU, GPU, RAM, disk, ağ ve saat göstergeleri,
temalar ve ARGB efektleri. L-Connect gerekmez.

## İndir / Download

**[Son sürümü indir (Bar-UniScreen-Setup)](https://github.com/felicrutter/bar-uniscreen-releases/releases/latest)**

1. `Bar-UniScreen-Setup-x.y.z.exe` dosyasını indirip çalıştırın. Kurulum tüm bilgisayara yapılır ve
   yönetici izni (UAC) ister. Intel işlemcilerde işlemci sıcaklığı için PawnIO sürücüsünü de kurar (aşağıya bakın).
2. Windows "Windows bilgisayarınızı korudu" uyarısı gösterirse **Ek bilgi → Yine de çalıştır** seçin
   (kurulum dosyası imzalı değildir).
3. Uygulama sistem tepsisinde çalışır. Ayarlar için tepsi simgesine çift tıklayın.

Güncellemeler: uygulama yeni sürümü kendisi bulur ve kurmadan önce sorar
(Ayarlar → Genel → Güncellemeler).

Requirements: Windows 10/11 x64, .NET Framework 4.8 (built into Windows 10 1903+ and Windows 11).

## Sensörler / Sensors

Sensors are built in: GPU (AMD/NVIDIA), CPU load/power/clock, RAM, disk temperature, network.

CPU temperature needs a kernel driver on Windows. On Intel CPUs the setup installs the official, signed
[PawnIO](https://github.com/namazso/PawnIO) driver (only if it is not already installed) and a small
Bar UniScreen service that reads only the CPU temperature registers (IntelMSR module). It does not touch
SMBus, SuperIO, the EC or RGB devices, so it does not conflict with RGB and monitoring apps. Uninstalling
Bar UniScreen removes the service; PawnIO stays installed because other apps may use it. On AMD CPUs,
run HWiNFO (shared memory / gadget) for the CPU temperature.

İşlemci sıcaklığı: Intel işlemcilerde kurulum imzalı PawnIO sürücüsünü kurar (zaten kuruluysa atlar) ve
yalnızca işlemci sıcaklığını okuyan küçük bir servis ekler. SMBus, SuperIO, EC ve RGB cihazlarına erişmez.
AMD işlemcilerde işlemci sıcaklığı için HWiNFO kullanın.

## Notes

This repository only hosts releases; the source code is private.
Bar UniScreen is an independent project and is not affiliated with or endorsed by Lian Li.
Third-party licenses: [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).
