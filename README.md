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

Membuat repository server

• Server reopsitory yang akan kita gunakan adalah http://github.com                                                                                      
• Anda harus membuat akun terlebih dahulu.                                                                                                                                              
• Pada laman github, klik tombol start a project, atau                                                                                                         
• Dari menu (icon +) klik New Repository                                                                                                              
![latihan git11](https://user-images.githubusercontent.com/46746119/51959934-49df4800-2489-11e9-85d9-aafbba6580cc.jpg)

• Isi nama repositorynya, misal: Ujian1.                                                                                                              
• Kemudian klik Creat Repository                                                                                                                            

• Remote Repository merupakan repository server yang akan                                                                                                   
digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.                                                      
• Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]                                                                     
$ git remote add origin https://github.com/HidayatBlog/Ujian1.git                                                                                              

Push (Mengirim perubahan ke server)

• Untuk mengirim perubahan pada local repository ke server gunakanperintah git push.                                                                            
• Perintah ini akan meminta memasukkan username dan password pada akun github.com                                                                           
![latihan git14](https://user-images.githubusercontent.com/46746119/51960197-88c1cd80-248a-11e9-9b46-830c567f3b86.png)

Melihat hasilnya pada server repository

• Buka laman github.com, arahkan pada repositori- nya.                                                                                                 
• Maka perubahan akan terlihat pada laman tersebut.                                                                                                      
![latihan git15](https://user-images.githubusercontent.com/46746119/51960292-07b70600-248b-11e9-9770-0fe8a6c892e3.jpg)

Clone Repository

• Clone repository, pada dasarnya adalah meng-copy repository server                                                                                        
dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).                                                                   
• Untuk melakukan cloning, gunakan perintah git clone [url]                                                                                              
![latihan git16](https://user-images.githubusercontent.com/46746119/51960453-a2afe000-248b-11e9-8815-5aae1bf33f9d.jpg)


Kegunaan file README.md

• Apabila kita menggunakan github, untuk memberikan penjelasan awal pada project yang kita buat,                                                             
maka dapat menggunakan sebuah file yang bernama README.md                                                                                          
• Pada file tersebut kita dapat membuat dokumentasi awal dari setiap                                                                                     
project yang kita buat untuk memberikan penjelasan atau sekedar cara penggunaan dari aplikasi yang kita kembangkan.                                    
• Penulisan file README.md berbasis teks, dan untuk pemformatannya menggunakan Markdown format.                                                                 
• untuk lebih jelasnya, dapat anda pelajari cara penggunaan markdown pada url berikut:


#Kurang Lebihnya Mohon maaf
