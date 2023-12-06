# Jarkom-Modul-4-IT17-2023

Laporan resmi dari modul keempat mata kuliah Komunikasi Data dan Jaringan Komputer IT ITS 2023.

## Authors

| NRP        | Nama                       |
| :--------  | :------------------------  |
| 5027211038 | Ahnaf Musyaffa             |
| 5027211056 | Gilbert Immanuel Hasiholan |


## Topologi

![Topologi](images/Topology.png)

## VLSM
### Topologi VLSM
Tentukan subnet dari topologi, dengan metode VLSM.
![VLSM_Topologi](images/VLSM_Topology.png)

### Rute dan Subnet Mask
Tentukan subnet mask dari masing-masing subnet, dengan jumlah host yang dibutuhkan yang tercamtum di topologi.
![VLSM_Route](images/VLSM_Route.png)

### Konfigurasi IP
Buat perhitungan dari subnet mask dari masing-masing subnet untuk menentukan pembagian konfigurasi IP.
![VLSM_IP](images/VLSM_IP.png)

### VLSM Tree
Berdasarkan konfigurasi IP yang sudah didapatkan, gambarkan tree VLSM nya.
![VLSM_Tree](images/VLSM_Tree.drawio.png)

### Konfigurasi di CPT
1) Subnetting\
    Atur IP interface dari router yang mengarah ke client.\
    (Contoh: Subnet A2, Frieren -> Switch3 -> LakeKorridor)\
    ![Frieren2Lake](images/Frieren2Lake.png)

    Atur IP interface dari client yang mengarah ke router.
    (Contoh: Subnet A2, LakeKorridor -> Switch3 -> Frieren)
    ![Lake2Frieren](images/Lake2Frieren.png)

    Atur IP interface dari router utama yang mengarah ke router subnet.
    (Contoh: Subnet A15, Aura -> Frieren)
    ![Aura2Frieren](images/Aura2Frieren.png)

    Atur IP interface dari router subnet yang mengarah ke router utama.
    (Contoh: Subnet A15, Frieren -> Aura)
    ![Frieren2Aura](images/Frieren2Aura.png)
    Lakukan untuk semua subnet.

2) Routing\
    Atur default routing dari router subnet ke router utama.
    (Contoh: Frieren -> Aura)
    ![Routing_F2A](images/Routing_Frieren2Aura.png)

    Atur routing dari router utama ke subnet client.
    (Contoh: Subnet A2, Aura -> Frieren)
    ![Routing_A2F](images/Routing_Aura2Frieren.png)
    Lakukan untuk semua subnet.

3) Testing\
    Sekarang kita akan melakukan testing. Contoh yang akan digunakan adalah dari LakeKorridor ke Aura dan sebaliknya.
    ![VLSM_Testing](images/VLSM_TestingRes.png)

## CIDR
### Topologi CIDR
Tentukan subnet dari topologi, dengan metode CIDR.
![CIDR_Routing](images/CIDR_Routing.png)

### Rute dan Subnet Mask
Tentukan subnet mask dari masing-masing subnet, dengan jumlah host yang dibutuhkan yang tercamtum di topologi.
![CIDR_Route](images/penggabungan-cidr1.png)
![CIDR_Route](images/penggabungan-cidr2.png)
![CIDR_Route](images/penggabungan-cidr3.png)

### Konfigurasi IP
Buat perhitungan dari subnet mask dari masing-masing subnet untuk menentukan pembagian konfigurasi IP.
![CIDR_IP](images/cidr-pembagian-ip.png)

### CIDR Tree
Berdasarkan konfigurasi IP yang sudah didapatkan, gambarkan tree CIDR nya.
![CIDR_Tree](images/cidr_it17.png)

### Konfigurasi di GNS
Kami tidak sempat mengimplementasikan pada gns