# redis-terminal-commands

#### Redis terminal commands. 
#### How to using Redis on terminal commands. 
#### Redis'i terminal üzerinden komutlar ile kullanmak.

<pre>
keys * 
set name huseyin //name isimli key'i set eder.
get name huseyin //name isimli key'i getirir. 
exists name //name isimli key var mı yok mu ?
del name //name isimli key'i siler.
append user huseyin
append user " aydın" //user isimli key'e değer ekler.
hset user1 name huseyin
hset user1 last_name aydin //obje keyi oluşturur ilgili objenin fieldlerini ekler.
hget user1 email //user1 isimli objenin email keyini get eder.
hgetall user1 //user1'in tüm fieldlerini get eder.
set silinecekKey 123deger123 EX 5 //keyi set eder geçerlilik süresi atar. süre bitince silinir.
1. terminal >subscribe huso //huso kanalına abone olduk. // gördük
2. terminal >subscribe huso //huso kanalına abone olduk. //gördük
3. terminal >publish huso "selamlar" //huso kanalından yayın yapıldı.

-- Docker Kısmı --
docker run --name redisapp -p 6379:6379 redis //redis'in docker app'ını indiriyor ve çalıştırıyor.
docker images //docker image'lerini listeler.
docker run redis //redis imagesinden bir konteynır üretip çalıştırır.
docker ps //çalışan containerlerin process id'lerini alırız.
docker container ls //docker containerlerinin listesini verir.
docker exec -it [containerin ismi neyse o gelecek buraya] redis-cli //ilgili containerin üstünde redis-cli komutunu çalıştırdık.
DOCKER REDIS IMAGE SHELL>
KEYS * 
SET yeniRedisKey hoppaaa
keys *
get yeni*
get yeniRedisKey
exit
_ Bitti!
</pre>
