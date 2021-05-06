# custom-nginx
1. buat folder nginx
2. masukkan file Dockerfile dan index.html ke folder nginx
3. build nginx : sudo docker build -t lekmin/custom-nginx .
4. kita run image : sudo docker run -p 8080:80 --name lekmin -d lekmin/custom-nginx
5. lalu cek pada browser : (http://localhost:8080)
6. untuk stop : sudo docker stop lekmin (lekmin : nama container kita)
7. lalu apabila ingin mengupload ke hub docker harus membuat repositori dulu, akun saya lekmin dan saya sudah membuat repository custom-nginx, jadi nama image yang dibuat harus sama dengan nama repository kita di hub docker
8. perintahnya : sudo docker push lekmin/custom-nginx
