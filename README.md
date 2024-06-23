# fall-detection-system

mendeteksi insiden jatuh berdasarkan pembacaan akselerasi dan perubahan orientasi
sistem dibangun dengan sensor MPU6050, arduino, buzzer, dan push button

terdapat tiga trigger yang harus aktif agar sistem bisa mendeteksi insiden jatuh (dengan asumsi gerakan jatuh bebas, kecepatan awal = 0)
trigger 1 : akselerasi yang melampaui lower threshold
trigger 2 : akselerasi melampaui upper threshold dan perubahan orientasi yang signifikan
trigger 3 : akselerasi konstan dan perubahan orientaasi mendekati 0 

dengan lower threshold sebesar 1,2 dan upper threshold sebesar 5,08. nilai ini diambil dari data experimental yang telah dilakukan

ketika ketiga trigger sudah aktif, sistem akan mengaktifkam buzzer untuk memberi tanda terdeteksinya peristiwa jatuh. user dapat menekan push button untuk mematikan buzzer jika tidak terjadi peristiwa jatuh (false alarm) atau ketika sudah mendapatkan pertolongan
