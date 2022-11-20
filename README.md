# Jarkom-Modul-4-D01-2022
Laporan Resmi Praktikum Jarkom Modul 4

# Anggota Kelompok
Anggota  | NRP
---------|-------
Arvel Gavrilla Raissananda | 5025201148
Johnivan Aldo Sudiono | 05111940000051
Vincent Yonathan | 05111940000186

## Soal Jarkom-Modul-4 2021
- [Soal](https://docs.google.com/document/d/1hf5Vi5nbEq6YY-nqmK7XUTHGNL_KVEFVc14mW9k0FAg/edit)

## Pendahuluan
![image](https://user-images.githubusercontent.com/36225278/143553295-d3dd4ebe-0225-4c75-92df-c02dc52663e5.png)

Dalam mengerjakan soal ini, kami menggunakan teknik VLSM (Variable Length Subnet Masking) menggunakan CPT (Cisco Packet Tracer), dan teknik CIDR (Classless Inter Domain Routing) menggunakan GNS 3

## VLSM (Variable Length Subnet Masking) - CPT

![Subnet](https://user-images.githubusercontent.com/72689610/143666832-4e7ec7c7-4413-4e79-9014-3594842bd332.png)

### 1. Jumlah Alamat IP
Subnet serta jumlah IP untuk mendapatkan netmask dari tiap subnet ditunjukkan oleh tabel berikut :
| Subnet  | Jumlah IP | Netmask |
| :---         |     :---:      |          ---: |
| ------------- | ------------- | ------------- |
| A1  | 721 | /22 |
| A2  | 252 | /24 |
| A3  | 13 | /28 |
| A4  | 502 | /23 |
| A5  | 521 | /22 |
| A6  | 2 | /30 |
| A7  | 2 | /30 |
| A8  | 2 | /30 |
| A9  | 701 | /22 |
| A10  | 2 | /30 |
| A11 | 2021 | /21 |
| A12  | 101 | /25 |
| A13  | 1001 | /22 |
| Total  | 5841 | /19 |

### 2. Menghitung NID dengan tree (pohon)
Subnet pertama memiliki NID 192.173.0.0 dengan netmask /19. Perhitungan dengan pohon dapat dilihat sebagai berikut :
![image](https://user-images.githubusercontent.com/72689610/143667143-2b90879b-1ea2-41b6-a309-44405b72e3b7.png)

### [Link Tree](https://intip.in/PohonPembagianIpVSLM)

### 3. Pengaturan Konfigurasi IP
###	Foosha
1.	Cloud                                                        
    192.173.72.13 subnet 255.255.255.252
2.	Mengarah Blueno                                             
    192.173.16.1 subnet 255.255.252.0
3.	Mengarah Server Doriki                                                              
    192.173.0.33 subnet 255.255.255.240
4.	Mengarah Guanhao                                                                          
    192.173.0.5 subnet 255.255.255.252
5.	Mengarah Water7                                                                                           
    192.173.0.9 subnet 255.255.255.252                                        
                                                                                      
### Water7
1.	Mengarah Foosha                                                                     
    192.173.0.10 subnet 255.255.255.252
2.	Mengarah Cipher                                                                         
    192.173.12.1 subnet 255.255.255.0
3.	Mengarah Pucci                                                                                          
    192.173.0.13 subnet 255.255.255.252

###	Pucci
1.	Mengarah Water7                                                                                     
    192.173.0.14 subnet 255.255.255.252
2.	Mengarah Jipangu                                                                                
    192.173.0.129 subnet 255.255.255.128
3.	Mengarah Courtyard dan Calmbelt                                                                             
    192.173.24.1 subnet 255.255.248.0

###	Guanhao
1.	Mengarah Foosha                                                                     
    192.173.0.6 subnet 255.255.255.252
2.	Mengarah Jabra                                                                                      
    192.173.8.1 subnet 255.255.252.0
3.	Mengarah Alabasta                                                                     
    192.173.2.1 subnet 255.255.254.0
4.	Mengarah OIMO                                                                   
    192.173.0.1 subnet 255.255.255.252

###	Alabasta 
1.	Mengarah Guanhao                                                                                                                                                          
    192.173.2.2 subnet 255.255.254.0 
2.	Mengarah Jorge                                                                                                   
    192.173.0.17 subnet 255.255.255.240

###	OIMO
1.	Mengarah Guanhao                                                          
    192.173.0.2 subnet 255.255.255.252
2.	Mengarah Server Fukurou                                                     
    192.173.0.49 subnet 255.255.255.240
3.	Mengarah Seastone                                                                 
    192.173.1.1 subnet 255.255.255.0
                          
###	Seastone
1.	Mengarah OIMO                                                                       
    192.173.1.2 subnet 255.255.255.0
2.	Mengarah Elena                                                                          
    192.173.4.1 subnet 255.255.252.0

###	PC Jipangu <br>
![image](https://user-images.githubusercontent.com/72689610/143667457-19da630b-b00e-42e7-ae2e-7835cd829f1f.png)

###	PC Courtyard <br>
![image](https://user-images.githubusercontent.com/72689610/143667641-ce5ef71e-8342-4c22-a88d-0113fa846109.png)

###	PC Calmbelt <br>
![image](https://user-images.githubusercontent.com/72689610/143667694-e975033e-cf3a-4eed-9aa8-221b214651d5.png) 

###	PC Cipher <br>
![image](https://user-images.githubusercontent.com/72689610/143667736-83d917d4-01f2-433c-9d44-7ca210a14a4b.png) 

###	PC Blueno <br>
![image](https://user-images.githubusercontent.com/72689610/143667790-0b616249-1898-42be-9c9d-c9e88eb8276c.png) 

###	PC Jabra <br>
![image](https://user-images.githubusercontent.com/72689610/143668090-7067edc6-c90a-4dea-84f6-56a5b584bea0.png) 

###	PC Maingate <br>
![image](https://user-images.githubusercontent.com/72689610/143668152-956ca995-5164-4504-9225-13b531d9c34c.png) 

###	PC Jorge <br>
![image](https://user-images.githubusercontent.com/72689610/143668172-3545fd5c-3f0a-4ac5-99d9-f51e67adee41.png) 

###	PC Enieslobby <br>
![image](https://user-images.githubusercontent.com/72689610/143668183-d978eeee-c20c-4728-b58b-c258c1c51865.png)

###	PC Elena <br>
![image](https://user-images.githubusercontent.com/72689610/143668285-c1f1db6d-0661-4cf6-a4a7-56fc87c204d3.png) 

###	Server Fukurou <br>
![image](https://user-images.githubusercontent.com/72689610/143668317-48c6abdb-b90a-4c00-a46f-33291399c47c.png) 

###	Server Doriki <br>
![image](https://user-images.githubusercontent.com/72689610/143668337-50820ab7-5d54-409a-8d8a-ce3ee0e409da.png)

### Pengaturan Routing
Untuk langkah nya bisa masuk kedalam router, lalu menekan menu static dan menambahkan data yang diinginkan

###	Foosha
- 192.173.4.0/22 via 192.173.0.6
- 192.173.1.0/24 via 192.173.0.6
- 192.173.0.16/28 via 192.173.0.6
- 192.173.2.0/23 via 192.173.0.6
- 192.173.8.0/22 via 192.173.0.6
- 192.173.0.0/30 via 192.173.0.6
- 192.173.12.0/22 via 192.173.0.10
- 192.173.0.12/30 via 192.173.0.10
- 192.173.0.128/25 via 192.173.0.10
- 192.173.0.48/28 via 192.173.0.6
- 192.173.24.0/21 via 192.173.0.10 

![image](https://user-images.githubusercontent.com/72689610/143668562-2edb69f4-f352-4c40-979a-4e2abe672e51.png)

###	Water7
- 0.0.0.0/0 via 192.173.0.9
- 192.173.24.0/21 via 192.173.0.14
- 192.173.0.128/25 via 192.173.0.14

![image](https://user-images.githubusercontent.com/72689610/143668799-80debd20-4f8f-4552-bb75-39675cd2af38.png)

###	Pucci
- 0.0.0.0/0 via 192.173.0.13

![image](https://user-images.githubusercontent.com/72689610/143669293-8fea625d-9d2d-4a9c-a665-db3a49184228.png)

### Guanhao
- 0.0.0.0/0 via 192.173.0.5
- 192.173.4.0/22 via 192.173.0.2
- 192.173.1.0/24 via 192.173.0.2
- 192.173.0.16/28 via 192.173.2.2
- 192.173.0.48/28 via 192.173.0.2

![image](https://user-images.githubusercontent.com/72689610/143669344-4b46cad0-c35d-470c-a34e-20552ea7ccf9.png)

### Alabasta
- 0.0.0.0/0 via 192.173.2.1

![image](https://user-images.githubusercontent.com/72689610/143669361-cc54ee1e-6ff5-4d5e-9622-aa52d9e23a9f.png)

###	OIMO
- 0.0.0.0/0 via 192.173.0.1
- 192.173.4.0/22 via 192.173.1.2

![image](https://user-images.githubusercontent.com/72689610/143669408-d69f65a4-09b5-4b1e-a70e-3c2f404effc4.png)

### Seastone
- 0.0.0.0/0 via 192.173.1.1

![image](https://user-images.githubusercontent.com/72689610/143669436-c829ae6a-10ed-433b-a5d0-3d41a9b8f384.png)

### Testing
Untuk testing sendiri dapat dilakukan dengan cara berikut :
1. Klik Menu `Add Simple PDU`
2. Pilih Source
3. Pilih Destination
4. Cek apakah ping tersebut success atau tidak

Berikut adalah contohnya:

![Testing](https://user-images.githubusercontent.com/72689610/143669632-294cd1a7-8f8d-4b71-9a1b-afaba1150828.png)


## CIDR (Classless Inter Domain Routing) - GNS3

Menggabungkan subnet-subnet paling bawah dalam topologi, berikut penggabungannya:

![image](https://user-images.githubusercontent.com/36225278/143669280-02c5d18a-351f-42a9-9454-b127423a9298.png)

![image](https://user-images.githubusercontent.com/36225278/143669286-e6432d2e-91e7-4eee-a844-fc93cdd131b3.png)

![image](https://user-images.githubusercontent.com/36225278/143669290-5c25f4b5-82bf-4356-998c-7f1a0b97140d.png)

![image](https://user-images.githubusercontent.com/36225278/143669298-31bf0094-039b-4dce-98e3-da4c83bf5280.png)

![image](https://user-images.githubusercontent.com/36225278/143669302-34603afe-0e79-4afc-b289-0924b985399e.png)

![image](https://user-images.githubusercontent.com/36225278/143669304-d769a7ee-3eea-4526-8509-bbd15d43ec6e.png)

![image](https://user-images.githubusercontent.com/36225278/143669312-04f69c52-76d6-4857-acaf-85f3ead428cc.png)

### Membuat topologi di GNS3

![image](https://user-images.githubusercontent.com/36225278/143669362-2b98c6a0-adf5-4859-940a-06c77a57013b.png)

### Jumlah Alamat IP
Subnet serta jumlah IP untuk mendapatkan netmask dari tiap subnet ditunjukkan oleh tabel berikut :
| Subnet  | NID | Netmask |
| :---         |     :---:      |          ---: |
| ------------- | ------------- | ------------- |
| A1  | 192.173.0.0 /21 | 255.255.248.0 |
| A2  | 192.173.8.0 /25 | 255.255.255.128 |
| A3  | 192.173.32.0 /22 | 255.255.252.0 |
| A4  | 192.173.192.0 /22 | 255.255.252.0 |
| A5  | 192.173.148.0  /22 | 255.255.252.0 |
| A6  | 192.173.144.0 /23 | 255.255.254 |
| A7  | 192.173.146.0 /28 | 255.255.255.240 |
| A8  | 192.173.128.0 /22 | 255.255.252.0 |
| A9  | 192.173.132.0 /24 | 255.255.255.0 |
| A10  | 192.173.16.0 /30 | 255.255.255.252 |
| A11 | 192.173.64.0 /30 | 255.255.255.252 |
| A12  | 192.173.160.0 /30 | 255.255.255.252 |
| A13  | 192.173.136.0 /30 | 255.255.255.252 |

### Menghitung NID dengan tree (pohon)
![image](https://user-images.githubusercontent.com/72689610/143675446-cb941553-e891-41e1-af60-b3cfb67f7c0b.png)

### [Link Tree](https://miro.com/app/board/o9J_lhT-ylc=/)

### Membuat konfigurasi pada GNS3

#### Foosha
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
        address 192.173.64.1
        netmask 255.255.255.252

auto eth2
iface eth2 inet static
         address 192.173.192.1
         netmask 255.255.255.252

auto eth3
iface eth3 inet static
        address 192.173.1.1
        netmask 255.255.255.252

auto eth4
iface eth4 inet static
        address 192.173.32.1
        netmask 255.255.255.252
```

#### Water 7
```
auto eth0
iface eth0 inet static
       address 192.173.192.2
       netmask 255.255.255.252
       gateway 192.173.192.1
auto eth1
iface eth1 inet static
       address 192.173.144.1
       netmask 255.255.255.252
auto eth2
iface eth2 inet static
         address 192.173.160.1
         netmask 255.255.252.0
```

#### Pucci
```
auto eth0
iface eth0 inet static
         address 192.173.144.2
         netmask 255.255.255.252
         gateway 192.186.144.1
auto eth1
iface eth1 inet static
         address 192.173.136.1
         netmask 255.255.255.128
auto eth2
iface eth2 inet static
         address 192.173.128.1
         netmask 255.255.248.0
```

#### Guanhao
```
auto eth0
iface eth0 inet static
          address 192.173.32.2
          netmask 255.255.255.252
          gateway 192.173.32.1
auto eth1
iface eth1 inet static
          address 192.173.20.1
          netmask 255.255.252.0
auto eth2
iface eth2 inet static
          address 192.173.8.1
          netmask 255.255.255.252
auto eth3
iface eth3 inet static
           address 192.173.16.1
          netmask 255.255.254.0
```

#### Alabasta
```
auto eth0
iface eth0 inet static
       address 192.173.18.1
       netmask 255.255.254.0
auto eth1
iface eth1 inet static
       address 192.173.16.2
       netmask 255.255.255.240
       gateway 192.173.16.1
```

#### Oimo
```
auto eth0
iface eth0 inet static
         address 192.173.8.2
         netmask 255.255.255.252
         gateway 192.173.8.1
auto eth1
iface eth1 inet static
          address 192.173.4.1
          netmask 255.255.255.0
auto eth2
iface eth2 inet static
           address 192.173.1.5
           netmask 255.255.255.252
```

#### Seastone
```
auto eth0
iface eth0 inet static
        address 192.173.4.2
        netmask 255.255.255.0
        gateway 192.186.4.1
auto eth1
iface eth1 inet static
        address 192.173.0.1
        netmask 255.255.252.0
```

#### Blueno
```
auto eth0
iface eth0 inet static
        address 192.173.64.2
        netmask 255.255.252.0
        gateway 192.173.64.1
```

#### Chiper
```
auto eth0
iface eth0 inet static
       address 192.173.160.2
       netmask 255.255.252.0
       gateway 192.173.160.1
```

#### Jipangu
```
auto eth0
iface eth0 inet static
	     address 192.173.136.2
	     netmask 255.255.255.128
	     gateway 192.173.136.1
```

#### Calmbert
```
auto eth0
iface eth0 inet static
	     address 192.173.128.2
	     netmask 255.255.248.0
	     gateway 192.173.128.1
```

#### Courtyard
```
auto eth0
iface eth0 inet static
       address 192.173.128.3
       netmask 255.255.248.0
       gateway 192.173.128.1
```

#### Jabra
```
auto eth0
iface eth0 inet static
        address 192.173.20.2
        netmask 255.255.252.0
        gateway 192.173.20.1
```

#### EnniesLobby
```
auto eth0
iface eth0 inet static
         address 192.173.4.3
         netmask 255.255.255.0
         gateway 192.173.4.1
```

#### Elena
```
auto eth0
iface eth0 inet static
         address 192.173.0.2
         netmask 255.255.252.0
         gateway 192.173.0.1
```

#### MainGate
```
auto eth0
iface eth0 inet static
      address 192.173.16.3
      netmask 255.255.254.0
      gateway 192.173.16.1
```

#### Jorge
```
auto eth0
iface eth0 inet static
         address 192.173.18.2
         netmask 255.255.255.240
         gateway 192.173.18.1
```

- Kemudian uncomment `net.ipv4.ip_forward=1 pada file /etc/sysctl.conf` pada semua router.
- Pada router foosha lakukan perintah `iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.173.0.0/16` untuk client agar terhubung ke internet dan `iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.173.0.0/16` untuk server terhubung ke internet
- Lalu, lakukan routing dengan file `route.sh` pada dokumen `\root`. Kemudian jalankan dengan perintah `source route.sh`

#### Foosha
```
route add -net 192.173.144.0 netmask 255.255.255.252 gw 192.173.192.2
route add -net 192.173.136.0 netmask 255.255.255.128 gw 192.173.192.2
route add -net 192.173.160.0 netmask 255.255.252.0 gw 192.173.192.2
route add -net 192.173.128.0 netmask 255.255.248.0 gw 192.173.192.2
route add -net 192.173.8.0 netmask 255.255.255.252 gw 192.173.32.2
route add -net 192.173.20.0 netmask 255.255.252.0 gw 192.173.32.2
route add -net 192.173.18.0 netmask 255.255.255.240 gw 192.173.32.2
route add -net 192.173.16.0 netmask 255.255.254.0 gw 192.173.32.2
route add -net 192.173.4.0 netmask 255.255.255.0 gw 192.173.32.2
route add -net 192.173.0.0 netmask 255.255.252.0 gw 192.173.32.2
```

#### Guanhao
```
route add -net 192.173.4.0 netmask 255.255.255.0 gw 192.173.8.2
route add -net 192.173.0.0 netmask 255.255.252.0 gw 192.173.8.2
route add -net 192.173.18.0 netmask 255.255.254.0 gw 192.173.16.2
```

#### Water7
```
route add -net 192.173.128.0 netmask 255.255.248.0 gw 192.173.144.2
route add -net 192.173.136.0 netmask 255.255.255.128 gw 192.173.144.2
```

#### Oimo
```
route add -net 192.173.0.0 netmask 255.255.252.0 gw 192.173.4.2
```

## Hasil ping

#### Foosha
![image](https://user-images.githubusercontent.com/36225278/143685098-ed2289b1-03ba-4e28-b711-8fb9186d1bd6.png)

Kendala Praktikum:
- Pada file .cpt tidak dapat melakukan ping dari server fukurou ke server doriki (sudah diselesaikan)
- Tidak dapat menyambungkan 5 kabel dalam FOOSHA (sudah diselesaikan)
- Saat memasangkan kabel di cpt, agak sedikit bingung penamaannya (interface 0/0, interface 0/1) dan lainnya
- Saat melakukan ping di cpt, harus dilakukan 2-3x tidak bisa langsung 1x karena failed, nemun setelah dicoba lagi menjadi succesful
- Pada mengerjakan GNS3, atur konfigurasinya ada yang kebalik atau salah pada netmask
- Pada pengerjaan GNS3, pada modul tidak disuruh untuk melakukan CIDR pada server
- Terdapat berbagai kesalahan konfigurasi pada node
