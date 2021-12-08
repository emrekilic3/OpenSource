# Acik_kaynak_BC_HW_1
# 1.Kısım
**1)** bash ve sh kabuklarının çevre değişkenlerini kıyaslama

1.1  >>> Bir uçbirim açın ve mevcut kabuğu ekrana yazdırın

```bash
cat /etc/shells
echo $SHELL
```
1.2  >>> bash kabuğuna geçerek çevre değişkenlerini ekrana yazdırın

```bash
bash
printenv
```
1.3  >>> sh kabuğuna geçerek çevre değişkenlerini ekrana yazdırın

```bash
sh
printenv
```

**2)** Python kabuğu üzerinde basit fonksiyon geliştirme

```bash
python3
```

```python

def fibo(sayiNo):
   if sayiNo <= 1:
       return (sayiNo)
   else:
       return (fibo(sayiNo-1) + fibo(sayiNo-2))

for x in range (10):
    print(fibo(x))
```
**3)**  Kullanıcı bazlı değil, sistem genelinde kalıcı bir çevre değişkeni tanımlanmak istense, hangi sistem dosyası kullanılabilir.

```bash
/etc/environment
```
**4)** Kullanıcı ana dizininde bulunan dosyalardan hangisi Bash geçmişini depolamak için kullanılır?
```bash
.bash_history
```
# 2.Kısım

**1)**  isim adlı bir değişlene bir isim tanımlanarak bunun ekrana yazdırılması
```bash
$ isim='emre'
$ echo $isim
```
**2)** isim ve soyisim değişkenleri tanımlanarak bunlara birer değeri verilmeli, bunların birleştirilmiş halleri bir kisi değişkenine eşitlenmeli ve kişi değişkeni ekrana yazdırılmalı.

```bash
isim='emre'
soyisim='kilic'
kisi=$isim' '$soyisim
echo $kisi
```

**3)** /home/ dizininde iken /etc/systemd/system dizinine tek komut ile gidilmeli.

```bash
cd ../../etc/systemd/system
```

