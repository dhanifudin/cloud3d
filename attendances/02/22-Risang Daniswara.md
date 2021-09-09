# Rangkuman Layanan Cloud
- Nama : Risang Daniswara
- Kelas : TI3D
- Abs : 22

# Kategori Layanan Cloud
  - SaaS
  - PaaS
  - IaaS

# Service OCI Core 
  - Compute
  - Storage
  - Network
  - IAM
  - Database Cloud Service

# Compute 
  Terdiri dari 5 komponen :
  - bare metal 
  - dedicated virtual host
  - virtual machine
  - container engine
  - function

  1. Bare Metal Compute : 
	blank server sehingga pengguna harus menangani virtualisasi, 
        operating system, language runtime, app container dan code
	sangat cocok untuk aplikasi web yang memerlukan resource komputasi 
	yang besar, atau aplikasi yang memproses big data, 
	pemrosesan yang memerlukan bring-your-own-licensing (BYOL).
  
  2. Compute -  Dedicated Virtual Host dan Virtual Machine :
	merupakan single tenant model sehingga tidak ada resource yang akan dibagi dengan pengguna lain 
	dan layer virtualisasi ditangani oleh Oracle Sedangkan pada layanan virtual machines yang berwarna coklat, 
	merupakan multitenant model dengan virtualisasi berbasis hypervisor

  3. Compute -  Dedicated Virtual Host dan Virtual Machines:
        Pengguna ingin melakukan setting sebagian besar dari operating system, 
	misalnya OS Patch, security configuration, network, firewall, konfigurasi aplikasi 
	dan manual atau auto scaling untuk menangani kebutuhan trafik.
	
  4. Compute – Container Engine :
	Dapat melakukan setup pada app container dan code aplikasi anda. Pada layanan ini Container runtime 
	environment yang mengeksekusi Containers dan mengelola Container Image pada node.

  5. Compute – Oracle Function :
	Layanan yang memungkinkan pengguna hanya menulis code dengan beberapa 
	macam bahasa tanpa kawatir infrastrukturnya yang sudah ditangani OCI.
  
# Storage – Storage Model OCI
  membutuhkan penyimpanan dengan spesifikasi tertentu. Berikut adalah storage model OCI, yaitu:
	- Mendukung persistent and non persistent storage
	- Multiple format seperti data terstruktur, semi-terstruktur dan streaming
	- High Performance Computing dengan biaya yang rendah
	- Data dilindungi dari kerusakan perangkat keras
	- Data dapat disimpan di lokal untuk keperluan sendiri atau di remote storage untuk keperluan berbagi data
	- Data diakses menggunakan protokol tertentu

# Storage – Storage Services
	Terdapat 5 layanan penyimpanan yang didukung oleh OCI yaitu :
	- block volume 
	- local NVME 
	- file storage 
	- object storage  
	- archive storage
	Berikut Karakteristik dari penyimpanan diatas :

# Storage - Block Volume
	- Digunakan ketika mendeploy SAN (Storage Area Network)
	- Menggunakan low latency NVME SSD 
	- Dapat digunakan untuk keperluan komputasi yang tinggi
	- Data disimpan pada perangkat dengan fixed sized block misalnya 512 bytes
	- Dapat menggunakan system file apapun misalnya NTFS untuk windows, VMFS untuk VMWare
	- Dapat menambah block volume ketika storage sedangan online tanpa dampak pada aplikasi 
	  dan proses yang sedang berjalan
	- Secara otomatis direplikasi untuk menghindari kehilangan data
  
# Storage - Local NVME
	- Penyimpanan sementara yang diperlukan oleh aplikasi yang memerlukan latency yang sangat rendah dan pemrosesan yang tinggi.
	- NVME storage merupakah penyimpanan non-persistent (data hilang ketika direboot) sehingga perlu dibackup menggunakan RAID. 
	  RAID yang dapat digunakan pada OCI ada 3 macam yaitu RAID 1, RAID 10 dan RAID 6.
	- Biasanya digunakan pada NoSQL database (misalnya: MongoDB, Redis)

# Storage - File Storage
	- Mendukung distributed file system seolah-olah seperti local file system
	- Mendukung 2 sistem file yaitu NFS (Network File System) dan SMB (Server Message Block). 
	  Dapat digunakan pada Windows dan Unix.
	- Dapat diakses melalui jaringan, pada umumnya tidak memerlukan software tambahan
	- Sesuai untuk aplikasi yang dapat berjalan pada OS yang berbeda

# Storage - Object Storage
	- Semua data dikelola seperti object sehingga dapat menyimpan data apapun sesuai format aslinya
	- Objek disimpan pada storage bucket. Data disimpan pada struktur yang flat tanpa folder hirarki.
	- Dapat digunakan untuk menyimpan data yang berasal dari banyak sumber yang berguna untuk analisa, backup, atau arsip (archive)
	- Setiap objek terdiri dari metadata dan objek itu sendiri sehingga memudakan untuk melakukan indeksasi dan mengakses data.

# Storage - Archive Storage
	Terdiri dari 2 tier yaitu Standard Storage Tier (Hot) dan Archive Storage Tier (Cold). 
	Standard Storage Tier memiliki karakteristik seperti berikut:
	- Cepat, segera dan sering diakses
	- Pengambilan data seketika
	- Pada umumya untuk menampilkan data yang terbaru
	- Standard bucket tidak dapat didowngrade ke archive storage
 
	Karakteristik Archive Storage (Cold):
	- Jarang diakses tetapi data tetap harus disimpan untuk jangka waktu yang lama
	- Biayanya penyimpanan 10 kali lebih murah dari Standard Tier
	- Data minimum disimpan 90 hari
	- Object harus direstore sebelum didownload
	- Tidak dapat diupgrade menjadi standard tier
 
# Networking
	- VCN merupakan network yang dimiliki oleh VM anda
	- VCN merupakan layanan Infrastructures as a Service (IaaS).
	- VCN memungkinkan pengguna untuk mengatur jaringan yang ada di lingkungan cloud. Dalam hal ini, kita bisa mengatur IP Address, membuat subnets dan tabel route, juga mengkonfigurasi firewall. 
	- Manfaat  Virtual Cloud Network ( VCN ) yaitu: 
	  1. Untuk memperluas jaringan lokal ke Oracle Cloud. 
	  2. Meningkatkan keamanan pada jaringan VM. 
	  3. Mengatur lalu lintas data yang masuk dan juga keluar 

 	Beberapa komponen yang terdapat dalam VCN, yaitu : 
	- Subnets 
	- Route Table 
	- Security List 
	- Internet Gateway 
	- Nat Gateway 
	- Service Gateway 
	- Dynamic Router Gateway

# IAM
	- IAM (Identity and Access Management ) memungkinkan Anda mengontrol siapa yang memiliki akses ke sumber daya cloud yang Anda miliki, dan jenis akses apa yang mereka miliki, dan ke sumber daya tertentu. 
	- IAM policy adalah dokumen yang menentukan siapa dan bagaimana cara yang dapat digunakan untuk mengakses sumber daya. 
	- Akses tingkat grup dan compartment  diberikan, yang berarti Anda dapat menulis kebijakan yang memberi jenis akses tertentu dalam grup dan menggunakan compartment tertentu. 
	- Compartment adalah kumpulan resource yang saling terkait yang membantu Anda untuk menentukan akses ke resources yang anda miliki.

# Database dan Cloud Service 
	OCI memiliki pilihan Oracle Cluster Databases, juga dikenal sebagai Real Application Clusters, atau RAC, telah menjadi pilihan untuk mengelola high availability and performance selama lebih dari 20 tahun terakhir. 
	OCI juga menawarkan sistem Exadata DB, yang menawarkan kinerja ekstrem baik untuk Online Transaction Processing (OLTP) maupun aplikasi data warehouse. 

	Autonomous database dibangun di atas arsitektur Exadata Oracle yang highly available architecture, sehingga Anda dapat dengan mudah scaling database deployment. 
	Beberapa model autonomous database adalah Autonomous Data Warehouse (ADW) , Autonomous Transaction Processing, (ATP) dan Autonomous JSON.
	
	- ATP adalah layanan basis data cloud yang menghilangkan kerumitan pengoperasian dan pengamanan high performance 
	  databases. Layanan ATP dibangun untuk mendukung segalanya, mulai dari aplikasi web sederhana hingga aplikasi besar dan canggih yang sangat penting untuk operasi bisnis.
	- ADW adalah layanan Data Warehouse yang menghilangkan semua kerumitan pengoperasian Data Warehouse, 
	  Mengamankan data dan mengembangkan aplikasi berbasis data. ADW menyertakan alat untuk pemuatan data 
	  secara mandiri, transformasi data, automatic insights, dan analis menggunakan pembelajaran mesin. 
	- Database Oracle Autonomous JSON adalah database dokumen yang memudahkan pengembangan aplikasi JSON-centric. 
	  Layanan ini menampilkan API dokumen sederhana, penskalaan tanpa server, transaksi aset dengan cepat 
          (high performance) dengan keamanan yang komprehensif.

