# GPT-Verify Projesini Bulut Bilişimciler Ortamında Çalıştırma Rehberi

Hoş geldiniz! Bu rehberde, GPT-Verify projesini [GitHub deposundan](https://github.com/a-mertdincer/gpt-verify) çekerek ve Docker kullanarak yerel ortamınızda ayağa kaldırma adımlarını bulacaksınız.

## Adım 1: Proje Klonlama

Proje deposunu bilgisayarınıza klonlayın:

```
git clone https://github.com/a-mertdincer/gpt-verify.git
```

## Adım 2: Proje Dizinine Girme
İndirilen projenin dizinine gidin:
```
cd gpt-verify
```

## Adım 3: Docker İmajını Oluşturma
Ardından, Dockerfile'ın bulunduğu dizinde terminal veya komut istemcisini açın ve şu komutu çalıştırarak Docker imajını oluşturun
```
docker build -t myproject:latest .
```
Bu komut, "myproject:latest" adında bir Docker imajı oluşturur.

## Adım 4: Docker İmajını Çalıştırma

Docker imajını oluşturduktan sonra, aşağıdaki komutla bu imajı çalıştırabilirsiniz:
```
docker run -p 5000:5000 myproject:latest
```
## Adım 4: Tarayıcıda Kontrol Etme
Sol menüden port seçeneğini tıklayarak 5000 portuna gidip kontrol edin.