Nama &nbsp; &nbsp;: Yoga Pratama<br>

NIM&nbsp; &nbsp; &nbsp; : 312210042<br>

Kelas&ensp; &nbsp; : TI.22.A.1<br>

Matkul &nbsp;: Pemrograman Mobile<br>

Dosen &nbsp; : Donny Maulana, S.Kom., M.M.S.I.<br>

# Project UAS Mobile

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|TUGAS|[Click Here](#tugas)|
|2|Penjelasan|[Click Here](#penjelasan)|
|3|Souce Code|[Click Here](#source-code)|


## TUGAS
<p align="justify"> Tugas Project UAS ini adalah mengumpulkan semua hasil yang sudah dibuat dari pertemuan pertama sampai akhir, hasil dari semua project tersebut digabungkan dalam satu Aplikasi. Berikut ini semua code yang telah Saya buat.</p>


## Penjelasan 
<p align="justify">Saya akan Menampilkan sebuah project yang sudah saya buat dari pertemuan 1 hingga pertemuan 15 serta menampilkan Source Code dari menu Hello Word, Menu Count, Menu Scroll Movie Sianida, Menu TwoActivity, Menu Alarm, Menu Gmaps,Serta Menu Movie , Fragment Movie memakai Raw untuk menampilkan Videonya/Trailernya.</p>


## Source Code
<p align="justify"> jika saya beri satu persatu source code nya akan menjadi terlalu banyak,maka source code akan saya beri dengan filennya saja yang dibuka.</p>

  - Source Code SplashScreen<br>
        - SplashScreen.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/SplashScreen.java)<br> Splashscreen.java berguna untuk menampilkan logo splashscreen<br>
        - Logo SplashScreen [Lihat Source Code](UAS_MOBILE/app/src/main/res/drawable/backgroundlauncher.xml)<br> Ini adalah tampilan dari Souce code Logo SplashScreen<br>
  
  - Source Code Menu Utama<br>
        - MainActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/MainActivity.java)<br> menggabungkan Source Code Java dari keseluruhan Project <br>
        - Activity_Main.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_main.xml)<br> Menampilkan Desai Tampilan Menu yang ada didalam project <br>
        - String.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/values/strings.xml)<br> Pemanggilan <br>
        - Color.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/values/colors.xml)<br> ini adalah warna yang digunakan untuk project ini<br>
        - Android Manifest [Lihat Source Code](UAS_MOBILE/app/src/main/AndroidManifest.xml)<br> Android Manifest memiliki fungsi yang mendefinisikan karakteristik dan perilaku aplikasi Android seperti identifikasi aplikasi , menentukan komponen aplikasi dan sebagainya.<br>
  
  - Source Code Menu Hello Word </br>
        - HelloActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/HelloActivity.java)<br> Ini adalah Source Code java dari menu hello word<br>
        - Activity_Hello.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_hello.xml)<br> ini adalah tampilan desain dari project Hello Word<br>
        - Hasil Run Menu Hello Word
    
https://github.com/yogafrtm25/Project-Mobile-UAS/assets/115678171/4e90153c-f69a-4648-8ea8-1020feefd388
        
  - Source Code Menu Count</br>
        - CountActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/CountActivity.java)<br> ini adalah source code java dari menu count yang didalamnya adalah project fibonaci <br>
        - Activity_Count.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_count.xml)<br> Ini adalah Tmpilan Desain dari Fibonaci.<br>
        - Hasil Run Menu Count

https://github.com/yogafrtm25/Project-Mobile-UAS/assets/115678171/e8ba13c3-4453-4005-8352-bfea78efa7d6

  - Souce Code Menu Scroll Movie</br>
        - SianidaActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/SianidaActivity.java)<br> ini adalah source code java dari Menu sianida<br>
        - Activity_Sianida.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_sianida.xml)<br> tampilan desain dari menu sianida<br>
        - Hasil Run Menu Sianida
    
https://github.com/yogafrtm25/Project-Mobile-UAS/assets/115678171/d4bc97ed-4606-415b-b2e2-aa10c6502ab9
    
  - Source Code Menu Two Activity</br>
        - TwoActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/TwoactActivity.java)<br> ini adalah Source Code java dari twoactivity <br>
        - TwoActivity2.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/Twoact2Activity.java)<br> ini adalah Source Code java dari twoactivity2 <br>
        - Activity_Twoact.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_twoact.xml)<br>ini adalah tampilan dan desain dari menu Twoactivity <br>
        - Activity_Twoact2.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_twoact2.xml)<br>ini adalah tampilan dan desain dari menu Twoactivity2<br>
        - Hasil Run Two Activity

https://github.com/yogafrtm25/Project-Mobile-UAS/assets/115678171/2dfde2af-3290-4844-a2d0-8bc8fe302807

  - Source Code Menu Alarm
        - Karena program ini hanya merupakan tombol, maka hanya tinggal menambahkan baris code berikut :<br>
     ```
    # Tambahkan code ini didalam protected void OnCreate :
          findViewById(R.id.btnSetAlarm).setOnClickListener(v -> {
              // Panggil metode untuk mengatur alarm
              setAlarm();
          });
      }

    # Lalu code tambahkan fungsi intent untuk tombolnya :
      private void setAlarm() {
          Intent alarm = new Intent(AlarmClock.ACTION_SET_ALARM);
          startActivity(alarm);
      }
     ```
    - Tidak hanya itu, perlu ditambahkan juga beberapa baris code di AndroidManifest.xml, seperti ini:
    ```           
    <uses-permission
          android:name="com.android.alarm.permission.SET_ALARM" />
  
    dan
        <action android:name="android.intent.action.SET_ALARM" />

                ```
   - Hasil Run Set Alarm

https://github.com/yogafrtm25/Project-Mobile-UAS/assets/115678171/8e396c3c-7ead-4338-9141-029a42531f84
      
  - Source Code Menu Maps</br>
    ```
    # Tambahkan code ini didalam protected void OnCreate :
    ImageButton btnshowMap = findViewById(R.id.btnshowMap);
        btnshowMap.setOnClickListener(v -> {
            Intent map = new Intent(Intent.ACTION_VIEW, Uri.parse("geo:-6.324307,107.169273"));
            map.setPackage("com.google.android.apps.maps");
            startActivity(map);
        });
    ```
  - Hasil Run Menu G-Maps
    
https://github.com/yogafrtm25/Project-Mobile-UAS/assets/115678171/d80de75d-685b-49c5-abe9-5f6c2b60be7e

  
  - Source Code Menu Movie</br>
          - FragmentActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/FragmentActivity.java)<br>Menampilkan Source Code java dari FragmentActivity<br> 
          - ActionFragment.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/ActionFragment.java)<br> Menampilkan Source Code java dari ActionFragment<br>
          - ComedyFragment.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/ComedyFragment.java)<br> Menampilkan Source Code java dari ComedyFragment<br>
          - RomaceFragment.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/RomanceFragment.java)<br> Menampilkan Source Code java dari RomaceActivity<br>
          - Activity_Movie.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_movie.xml)<br> ini adalah tampilan dan desain dari menu Movie<br>
          - Fragment_Action.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/fragment_action.xml)<br> ini adalah tampilan dan desain dari menu bagian Action didalam movie<br>
          - Fragment_Comedy.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/fragment_comedy.xml)<br> ini adalah tampilan dan desain dari menu bagian Comedy didalam movie<br>
          - Fragment_Romance.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/fragment_romance.xml)<br> ini adalah tampilan dan desain dari menu bagian Romance didalam movie<br>
          - Hasil Run Movie</br>
          
https://github.com/yogafrtm25/Project-Mobile-UAS/assets/115678171/8bd40bd3-8781-4d31-89aa-9aa0b0372132



<p align="center"><b>TERIMAKASIH SEMOGA BERMANFAAT</b></p>
<p align="center">Copyrights &copy; Yoga Pratama 2024</p>





