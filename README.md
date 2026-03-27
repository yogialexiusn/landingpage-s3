Landing Page Deployment Project (React + AWS S3 + CI/CD) www.alexinai.online

Project ini merupakan simulasi deployment aplikasi landing page untuk kebutuhan industri.
Aplikasi dibangun menggunakan React (Create React App), kemudian di-build menjadi static files dan di-deploy ke AWS S3.
Selain itu, project ini sudah terintegrasi dengan CI/CD menggunakan GitHub Actions, sehingga proses build dan deployment dapat berjalan otomatis.


Teknologi yang Digunakan
- React (Create React App)
- Amazon Web Services (S3 untuk hosting static website)
- GitHub Actions (CI/CD pipeline)
- Node.js & npm


Arsitektur Deployment
Alur kerja project ini:
1. Developer melakukan push ke repository
2. GitHub Actions akan:
  2a. Install dependencies
  2b. Build project (npm run build)
  2c. Deploy hasil build ke AWS S3
  2d. S3 akan menyajikan website sebagai static hosting
3. Akses ke website www.alexinai.online


Cara Menjalankan Project Secara Lokal
Pastikan sudah menginstall:
Node.js
npm / yarn
1. Install Dependencies
npm install
2. Menjalankan Mode Development
npm start
Aplikasi akan berjalan di:
- http://localhost:3000
Auto reload jika ada perubahan kode
- Menjalankan Testing
npm test
Menggunakan mode watch
Berguna untuk memastikan aplikasi berjalan sesuai harapan
- Build untuk Production
npm run build
Hasil build akan berada di folder:
/build


Keuntungan menggunakan S3:
- Cepat dan scalable
- Biaya rendah
- Mudah dikombinasikan dengan CDN (CloudFront) 
- CI/CD dengan GitHub Actions


Pipeline otomatis akan berjalan saat:
Push ke branch main
Proses CI/CD:
Checkout code
Install dependencies
Build project
Running Test
Deploy ke S3


Project ini dibuat untuk:
- Simulasi workflow industri (build & deploy)
- Implementasi CI/CD sederhana
- Praktik deployment static website ke cloud
- Memahami pipeline otomatis menggunakan GitHub Actions