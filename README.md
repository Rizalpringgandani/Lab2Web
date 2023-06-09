# PROJECT PRAKTIKUM 2 (PHP Dasar)

**_Nama: Rizal Pringgandani_** <br/>
**_Nim : 312110151_** <br/>
**_Kelas : TI.21.A2_** <br/>

<br/>

## **Latihan 1**


### _Code :_

```php
<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
    echo "Hello World";
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_1.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 2**


### _Code :_

```php
<body>
    <h1>Variable</h1>
    <?php
    $nim = "312110151";
    $nama = 'Rizal Pringgandani';
    echo "NIM : " . $nim . "<br>";
    echo "Nama : $nama";
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_2.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 3**


### _Code :_

```php
<body>
    <h1>Predefine Variable </h1>
    <?php
    echo 'Selamat Datang ' . $_GET['nama'];
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_3.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 4**


### _Code :_

```php
<body>
  <h2>Form Input</h2>
  <form method="post">
    <label>Nama: </label>
    <input type="text" name="nama">
    <input type="submit" name="kirim">
  </form>
  <?php
    if(isset($_POST["kirim"])){
      echo 'Selamat Datang ' . $_POST['nama'];
    }
  ?>
</body>
```

### _Output :_

<img src="ss/Latihan_4.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 5**


### _Code :_

```php
<body>
    <h1>Operator</h1>
    <?php
    $gaji = 1000000;
    $pajak = 0.1;
    $thp = $gaji - ($gaji * $pajak);
    echo "Gaji sebelum pajak = Rp. $gaji <br>";
    echo "Gaji yang dibawa pulang = Rp. $thp";
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_5.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 6**


### _Code :_

```php
<body>
    <h1>Kondisi if</h1>
    <?php
    $nama_hari = date("l");
    if ($nama_hari == "Sunday") {
        echo "Minggu";
    } elseif ($nama_hari == "Monday") {
        echo "Senin";
    } else {
        echo "Selasa";
    }
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_6.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 7**


### _Code :_

```php
<body>
    <h1>Switch</h1>
    <?php
    $nama_hari = date("l");
    switch ($nama_hari) {
        case "Sunday":
            echo "Minggu";
            break;
        case "Monday":
            echo "Senin";
            break;
        case "Tuesday":
            echo "Selasa";
            break;
        default:
            echo "Sabtu";
    }
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_7.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 8**


### _Code :_

```php
<body>
    <h1>Perulangan For</h1>
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    for ($i = 1; $i <= 10; $i++) {
        echo "Perulangan ke: " . $i . '<br />';
    }
    echo "Perulangan Menurun dari 10 ke 1 <br />";
    for ($i = 10; $i >= 1; $i--) {
        echo "Perulangan ke: " . $i . '<br />';
    }
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_8.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 9**


### _Code :_

```php
<body>
    <h1>Perulangan While</h1>
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    $i = 1;
    while ($i <= 10) {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    }
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_9.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **Latihan 10**


### _Code :_

```php
<body>
    <h1>Do While</h1>
    <?php
    echo "Perulangan 1 sampai 10 <br />";
    $i = 1;
    do {
        echo "Perulangan ke: " . $i . '<br />';
        $i++;
    } while ($i <= 10);
    ?>
</body>
```

### _Output :_

<img src="ss/Latihan_10.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

</br></br>

## **POGRAM SEDERHANA**


### _Code :_

```php
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <title>PHP Dasar</title>
</head>

<body>
  <h2>Pertanyaan dan Tugas</h2>
  <form method="post" style="align-items: center;">
    <div style="display: flex; flex-direction: column; gap: 5px; max-width: 200px; margin-bottom: 10px;">
      <label for="nama">Nama :</label>
      <input type="text" name="nama" required>
    </div>
    <div style="display: flex; flex-direction: column; gap: 5px; max-width: 200px; margin-bottom: 10px;">
      <label for="tanggal_lahir">Tanggal lahir :</label>
      <input type="date" name="tanggal_lahir" required>
    </div>
    <div style="display: flex; flex-direction: column; gap: 5px; max-width: 200px; margin-bottom: 10px;">
      <label for="pekerjaan">Pekerjaan :</label>
      <select name="pekerjaan">
        <option value="">- PILIH -</option>
        <option value="mahasiswa">Mahasiswa</option>
        <option value="dosen">Dosen</option>
        <option value="staf">Staf</option>
        <option value="teknisi">Teknisi</option>
        <option value="karyawan">Karyawan</option>
      </select>
    </div>
    <button type="submit" name="kirim">Submit</button>
  </form>
  <?php
  if (isset($_POST['kirim'])) {
    $nama = $_POST['nama'];
    $tanggal_lahir = $_POST['tanggal_lahir'];
    $pekerjaan = $_POST['pekerjaan'];
    $tanggal_sekarang = date('Y-m-d');
    
    switch ($pekerjaan) {
      case 'dosen':
        $gaji = 'Rp6.000.000';
        break;
      case 'staf':
        $gaji = 'Rp5.000.000';
        break;
      case 'teknisi':
        $gaji = 'Rp4.500.000';
        break;
      case 'karyawan':
        $gaji = 'Rp4.000.000';
        break;
      default:
        $gaji = 'Rp0';
        break;
    }
    function hitungUsia($tanggal_lahir, $tanggal_sekarang) {
      $tgl_lahir = new DateTime($tanggal_lahir);
      $tgl_sekarang = new DateTime($tanggal_sekarang);
      $perbedaan = $tgl_lahir->diff($tgl_sekarang);
      return $perbedaan->y;
    }
    ?>
    <div>
      <h3>Hasil Inputan</h3>
       <table>
        <tr>
            <td>Nama</td>
            <td>:</td>
            <td><?=$nama?></td>
        </tr>
        <tr>
            <td>Usia</td>
            <td>:</td>
            <td><?=hitungUsia($tanggal_lahir, $tanggal_sekarang)?> tahun</td>
        </tr>
        <tr>
            <td>Gaji</td>
            <td>:</td>
            <td><?=$gaji?></td>
        </tr>
    </table>
    </div>
    <?php
  }
  ?>
</body>

</html>
```

### _Output :_

<img src="ss/Program_Sederhana.png" style="border: 2px solid #333; border-radius: 5px; box-shadow: 2px 2px 4px #00000040">

### _Penjelasan :_

- pada from pengambilan data menggunakan method `post`
- pada saat button sumbit di klick maka semua data yang berada di dalam form akan dikirim kepada page ini sendiri dengan http method `post`
- lalu pada script php di menangkap `event` submit dari button yang bernama kirim
- mendeklarasikan variable nama, tanggal lahir dan pekerjaan. dengan mengambil value dari isi method `post` yang sudah di submit
- mendeklarasikan variable tanggal_sekarang dengan mengambil object data dengan format `Y-m-d`
- membuat fungsi perhitungan usia yang memiliki parameter `tanggal_lahir` dan `tanggal_sekarang` dengan memanfaatkan method bawaan dari php yaitu `diff` untuk menghitung selisih waktu dari tanggal sekarang dan tanggal lahir
- membuat pengkondisiian pekerjaan untuk mengetahui gaji dengan menggunakan `switch case`
- menampilkan `Hasil Inputan` dengan tag `table`

