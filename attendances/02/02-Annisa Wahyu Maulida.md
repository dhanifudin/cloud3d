Pertemuan 2

Komputasi Awan dan Sistem Terdistribusi

Kategori OCI dikategorikan menjadi 3, yakni 
- SaaS
- PaaS
- IaaS
yang mana urutannya semakin keatas semakin mudah karena sudah berupa aplikasi,dan semakin ke bawah semakin kompleks.

OCI Core Services meliputi 5 hal, 
1. Compute, terdiri dari 5 komponen. Yaitu,
- Bare metal
- Dedicated virtual host
- Virtual machines
- Container engine
- Function
Yang mana semakin ke kanan maka semakin sedikit yang perlu ditangani oleh pengguna. Misalnya penggunaan VM.
2. Storage. Pada storage dapat disimpan dalam bentuk file maupun berupa database. 
Terdapat 5 layanan penyimpanan yang didukung oleh OCI, yaitu 
- block volume
- local NVME
- file storage
- object storage
- archive storage
Penggunaan archive storage digunakan utk back up data dan bersifat jarang diakses tetapi data tetap harus disimpan untuk jangka waktu yang lama.
Block volume digunakan untuk keperluan komputasi yang tinggi. 
Local NVME Penyimpanan sementara yang diperlukan oleh aplikasi yang memerlukan latensi yang sangat rendah dan pemrosesan yang tinggi.
Umumnya pada File Storage, dapat diakses melalui jaringan tanpa software tambahan, terdapat 2 sistem file yang mendukung yaitu NFS dan SMB.
Pada Object Storage, setiap objek terdiri dari metadata dan objek itu sendiri sehingga memudakan untuk melakukan indeksasi dan mengakses data.
3. Networking. Berhubungan dengan konfigurasi firewall, mengatur IP Address, membuat subnets dan tabel route. 
Virtual Cloud Network (VCN) merupakan layanan Infrastructures as a Service (IaaS).
4. IAM (Identity and Access Management), berhubungan dengan akun. 
Seperti mengontrol siapa yang memiliki akses ke sumber daya cloud yang Anda miliki, dan jenis akses apa yang mereka miliki, dan ke sumber daya tertentu.
5. Database Cloud Service, seperti Oracle, AWS. Penyimpanan dapat berupa RDBMS maupun NO SQL.