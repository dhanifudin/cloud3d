# Oracle Cloud Infrastructure (OCI) Core Services
## OCI Core Service meliputi 5 hal yaitu :
1. **Compute** yang terdiri dari bare metal, dedicated virtual host, virtual machines, container engine, dan function.
* Bare metal yaitu pemrosesan inti dari sebuah server yang bertugas untuk memproses sebagian besar operasi yang dilakukan
dalam server.
* **Dedicated Virtual Host** yaitu layanan yang dilakukan oleh single virtual machines tanpa dibagi dengan pengguna lain.
* **Virtual Machines** adalah kebalikan dari Dedicated Virtual Host yaitu melakukan layanan dengan berbabi resource dengan pengguna lain.
* **Container Engine** yaitu proses dalam menyiapkan app dan code untuk software yang akan dijalankan.
* **Oracle Functions** yaitu layanan yang memungkinkan pengguna untuk menulis dan memodifikasi code tanpa melakukan pengaturan server.

2. **Storage** (Penyimpanan), dalam melakukan komputasi pastinya memerlukan spesifikasi penyimpanan tertentu. Penyimpanan
dalam OCI memiliki model penyimpanan persistent dan non-persistent, multiple format, high performance computing, data dilindungi dari
kerusakan harfware, data dapat disimpan secara lokal maupun publik, dan diakses menggunakan protokol tertentu.
* Terdapat 5 layanan penyimpanan yang didukung, yaitu Block Volumes, Local NVME, File Storage, Object Storage, dan Archive Storage.

3. **Networking**, Oracle memiliki VCN (Virtual Cloud Network) yaitu layanan yang digunakan dalam Oracle untuk mengatur jaringan yang
terdapat dalam lingkungan cloud. Komponen yang terdapat dalam VCN yaitu Subnet, Route Table, Security List, Internet Gateway, NAT Gateway,
Service Gateway, Dynamic Router Gateway.

4. **IAM** (Identity and Access Management), cloud computing kebanyakan nantinya digunakan untuk melayani sebagian besar permintaan
dari publik sehingga perlu diperhatikan dalam akses yang diberikan. Nantinya akan dilakukan pembagian dalam grup sehingga memiliki hak
akses yang berbeda-beda menggunakan compartment. Setelah dilakukan pembagian hak akses maka nantinya pengguna akan dapat mengakses dan
mengelola sumber daya sesuai dengan hak aksesnya masing-masing tanpa mencampuri sumber daya pengguna lain.

5. **Database Cloud Service** Oracle memiliki Oracle Cluster Databases yang memiliki kinerja sistem ekstrem untuk Online Transaction
Processing maupun aplikasi pergudangan data. Penemuan Autonomous database membebeaskan admin database untuk melakukan operasional database 
secara berkala dengan adanya journaling functions, keamanan database dan troubleshooting.
