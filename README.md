Nama &nbsp; &nbsp;: Yoga Pratama<br>

NIM&nbsp; &nbsp; &nbsp; : 312210042<br>

Kelas&ensp; &nbsp; : TI.22.A.1<br>

Matkul &nbsp;: Pemrograman Mobile<br>

Dosen &nbsp; : Donny Maulana, S.Kom., M.M.S.I.<br>

# Project UAS Mobile

## TUGAS
<p align="justify"> Tugas Project UAS ini adalah mengumpulkan semua hasil yang sudah dibuat dari pertemuan pertama sampai akhir, hasil dari semua project tersebut digabungkan dalam satu Aplikasi. Berikut ini semua code yang telah Saya buat.</p>

## Source Code
<p align="justify"> jika saya beri satu persatu source code nya akan menjadi terlalu banyak,maka source code akan saya beri dengan filennya saja yang dibuka.</p>

  - Source Code SplashScreen<br>
        - SplashScreen.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/SplashScreen.java)<br>
        - Logo SplashScreen [Lihat Source Code](UAS_MOBILE/app/src/main/res/drawable/backgroundlauncher.xml)<br>
  
  - Source Code Menu Utama<br>
        - MainActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/MainActivity.java)<br>
        - Activity_Main.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_main.xml)<br>
        - String.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/values/strings.xml)<br>
        - Color.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/values/colors.xml)<br>
        - Android Manifest [Lihat Source Code](UAS_MOBILE/app/src/main/AndroidManifest.xml)<br>
  
  - Source Code Menu Hello Word </br>
        - HelloActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/HelloActivity.java)<br>
        - Activity_Hello.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_hello.xml)<br>
        
  - Source Code Menu Count</br>
        - CountActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/CountActivity.java)<br>
        - Activity_Count.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_count.xml)<br>

  - Souce Code Menu Scroll Movie</br>
        - SianidaActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/SianidaActivity.java)<br>
        - Activity_Sianida.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_sianida.xml)<br>
        
  - Source Code Menu Two Activity</br>
        - TwoActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/TwoactActivity.java)<br>
        - TwoActivity2.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/Twoact2Activity.java)<br>
        - Activity_Twoact.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_twoact.xml)<br>
        - Activity_Twoact2.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_twoact2.xml)<br>
        
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
  - Source Code Menu Movie</br>
          - FragmentActivity.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/FragmentActivity.java)<br>
          - ActionFragment.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/ActionFragment.java)<br>
          - ComedyFragment.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/ComedyFragment.java)<br> 
          - RomaceFragment.java [Lihat Source Code](UAS_MOBILE/app/src/main/java/com/example/appintent/RomanceFragment.java)<br>
          - Activity_Movie.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/activity_movie.xml)<br>
          - Fragment_Action.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/fragment_action.xml)<br>
          - Fragment_Comedy.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/fragment_comedy.xml)<br>
          - Fragment_Romance.xml [Lihat Source Code](UAS_MOBILE/app/src/main/res/layout/fragment_romance.xml)<br>
          




