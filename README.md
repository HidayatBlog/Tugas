# Ujian 1 
Apa itu git?
1. Git adalah salah satu sistem pengontrol versi (Version Control System)                                                                                    
   pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.                                                                                                                                                                                                                                                                                        
2. Pengontrol versi bertugas mencatat setiap perubahan pada file
   proyek yang dikerjakan oleh banyak orang maupun sendiri.                                                                                                 
3. Git dikenal juga dengan distributed revision control (VCS terdistribusi),
   artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.                                                                                    
                                                                                                                                                      
   Cara menggunakan Git                                                                                                                                        
                                                                                                                                                                     
    Instalasi Git

 • Download Git, buka website resminya Git (git-scm.com).                                                                                            
 • Kemudian unduh Git sesuai dengan arsitektur komputer kita.                                                                                                         
 • Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit.                                                                                        
 • Selamat, Git sudah terinstal di Windows. Untuk mencobanya,                                                                                                   
 • silahkan buka CMD atau PowerShell, kemudian ketik perintah                                                                                                                                                                 
                                                                                                                                                         
Menambahkan Global Config

•  Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email                                                     
•  konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.                                                                    
•  apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit                                                                                                      
                                                                                                                                                                              
 Config Global Repository                                                                                                                            
$ git config --global user.name “nama_user”                                                                                                                                            
                                                                                                                                                                                                                           
$ git config --global user.email “nama_user”                                                                                                                
 ![latihan git](https://user-images.githubusercontent.com/46746119/51958671-9d4e9780-2483-11e9-8929-1036fc80c7b9.jpg)
                                                                                                                                                                                   
   Membuat Reposiory Local

• Buka direktory aktif, misal: d:\labs_pemrograman1 (buka menggunakan Windows Explorer)                                                               
• klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad                                                     
• Buat direktory project praktikum pertama dengan nama latihan1                                                                                    
                                                                                                                                                                                       
• Sehingga terbentuk satu direktori baru dibawahnya,                                                                                                                                                                                                     
   selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory)                                                                                                                                     
• direktory aktif menjadi: d:\labs_pemrograman1\latihan1                                                                                                                                                                                                                                                                                                                                                                                      
• Jalankan perintah git init, untuk membuat repository local.                                                                                       
• Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git                                                      
• Pada direktori tersebut, semua perubahan pada working directory akan disimpan.                                                                         

![latihan git4](https://user-images.githubusercontent.com/46746119/51959679-18b24800-2488-11e9-86ed-14befa29c218.jpg)

Menambahkan File baru pada repository                                                                                                                    

• Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)                                                                  
• disini kita akan coba buat satu file bernama README.md (text file)                                                                                                                
• File README.md berhasil dibuat. $ echo “#Latihan 1” >> README.md                                                                                                      

• Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.                                                                                  
• File README.md berhasil ditambahkan. $ git add README.md                                                                                                                 

Commit (Menyimpan perubahan ke database)                                                                                                                                   

• Untuk menyimpan perubahan yang ada kedalam database repository local,                                                                                
   gunakan perintah git commit -m “komentar commit”                                             
• Perubahan berhasil disimpan.

![latihan git10](https://user-images.githubusercontent.com/46746119/51959820-c160a780-2488-11e9-85d0-cb6c7339e55f.jpg)
