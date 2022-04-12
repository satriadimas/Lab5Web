# Praktikum 5 - Pemrograman Web

```
Satria Dimas Permana
312010450
TI.20.B.2
Universitas Pelita Bangsa
```

## buat dokumen HTML dengan nama file lab5_javascript.html dan masukan coding

![LANGKAH 1 membuat javascript](https://user-images.githubusercontent.com/22215113/116093562-fc3a0000-a6d0-11eb-98fd-d0ee348c9fee.png)

# Java Script Dasar

## Pemakaian Alert sebagai property window

![LANGKAH 2 membuat alert box](https://user-images.githubusercontent.com/22215113/116093584-022fe100-a6d1-11eb-9ebb-b7969da6f301.png)

## Pemakaian method dalam objek

![LANGKAH 3 Pemakaian metod](https://user-images.githubusercontent.com/22215113/116093591-04923b00-a6d1-11eb-8398-4ad401b46be4.png)

## Pemakaian Prompt

![LANGKAH 4 Pemakaian prompt](https://user-images.githubusercontent.com/22215113/116093616-08be5880-a6d1-11eb-88c7-bfa80fba2141.png)

## Pembuatan fungsi dan cara pemanggilannya

![LANGKAH 5 Pembuatan fungsi dan pemanggilan](https://user-images.githubusercontent.com/22215113/116093631-0b20b280-a6d1-11eb-82c2-82e12545251c.png)

# Dasar Pemrograman Di Javascript

## Operasi dasar Aritmatika

![LANGKAH 6 Operasi dasar Aritmatika](https://user-images.githubusercontent.com/22215113/116093650-0e1ba300-a6d1-11eb-9dfa-f69fdb0b39f5.png)

## Seleksi kondisi (if..else)

- Coding
  ![LANGKAH 7 seleksi kondisi (coding)](https://user-images.githubusercontent.com/22215113/116093659-107dfd00-a6d1-11eb-9573-94a20c4f8a77.png)

- Output

![LANGKAH 7 seleksi kondisi (hasil 1)](https://user-images.githubusercontent.com/22215113/116093759-268bbd80-a6d1-11eb-856f-91234517480b.png)

![LANGKAH 7 seleksi kondisi (hasil 2)](https://user-images.githubusercontent.com/22215113/116093767-2986ae00-a6d1-11eb-904f-42f3608d1e67.png)

## Penggunaan operator switch untuk seleksi kondisi

- Coding
  ![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (coding)](https://user-images.githubusercontent.com/22215113/116094011-5cc93d00-a6d1-11eb-9cda-170304e670ec.png)

- Output

![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (hasil 1)](https://user-images.githubusercontent.com/22215113/116094069-6bafef80-a6d1-11eb-83c5-7248eb946f8d.png)

![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (hasil 2)](https://user-images.githubusercontent.com/22215113/116094080-6d79b300-a6d1-11eb-8e5b-0f9471cf9d22.png)

# Pembuatan Form

## Form Input

- Coding
  ![LANGKAH 9 Form input (coding)](https://user-images.githubusercontent.com/22215113/116094109-74082a80-a6d1-11eb-96f6-84049980d45a.png)

- Output
  ![LANGKAH 9 Form input (hasil)](https://user-images.githubusercontent.com/22215113/116094143-7d919280-a6d1-11eb-8828-dfc8d446177e.png)

## Form Button

- Coding
  ![LANGKAH 10 Form Button (coding)](https://user-images.githubusercontent.com/22215113/116094214-897d5480-a6d1-11eb-9d9f-727838f5868d.png)

- Output
  ![LANGKAH 10 Form Button (HASIL)](https://user-images.githubusercontent.com/22215113/116094233-8da97200-a6d1-11eb-974a-b7b2c9dd6ae7.png)

## HTML DOM

- Coding
  ![LANGKAH 11 HTML DOM (coding)](https://user-images.githubusercontent.com/22215113/116094283-9c902480-a6d1-11eb-9732-d44e8be8f611.png)

- Output
  ![LANGKAH 11 HTML DOM (hasil)](https://user-images.githubusercontent.com/22215113/116094305-a0bc4200-a6d1-11eb-946e-7fa3da8ee846.png)

# TUGAS

## 1. Buat script untuk melakukan validasi pada isian form.

- Buat form pada `lab5_javascript.html`

```
<!DOCTYPE html>
<html lang="en">
<head>
	<title>Form Validasi</title>
	<link rel="stylesheet" type="text/css" href="style.css">
    <script type="text/javascript">
        function validasiForm() {
            var nama = document.getElementById("nama").value;
            var email = document.getElementById("email").value;
            var alamat = document.getElementById("alamat").value;
            if (nama != "" && email!="" && alamat !="") {
                return true;
            }else{
                alert('Isi Alamat Anda dengan lengkap !');
                return false;
            }
        }
    </script>
</head>
<body>
	<div class="login">
		<form action="beranda.html" method="POST" onSubmit="return validasiForm()">
			<div>
				<label>Nama Lengkap:</label>
				<input type="text" name="nama" id="nama" />
			</div>
			<div>
				<label>Email:</label>
				<input type="email" name="email" id="email" />
			</div>
			<div>
				<label>Alamat:</label>
				<textarea cols="40" rows="5" name="alamat" id="alamat"></textarea>
			</div>
			<div>
				<input type="submit" value="Daftar" class="tombol">
			</div>
		</form>
	</div>
</body>
</html>
```

![TUGAS (coding form validasi)](https://user-images.githubusercontent.com/22215113/116094374-ad409a80-a6d1-11eb-9291-5c9ab4533c78.png)

- Buat halaman beranda `beranda.html`

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beranda</title>
    <link rel="stylesheet" href="style.css">
    <script lang="javascript">
        function pesan() {
            alert ("Selamat Datang!")
        }
    </script>
</head>
<body onload=pesan()>
    <center><h1>Terimakasih telah mendaftar!!!</h1></center>
</body>
</html>
```

![TUGAS (coding Beranda)](https://user-images.githubusercontent.com/22215113/116094389-b0d42180-a6d1-11eb-8af8-4596c977a8ff.png)

- Tambahkan CSS untuk mempercantikan tampilan

```
body {
    background: darkgray;
    font-family: sans-serif;
    padding: 100px;
  }

  h2 {
    color: #fff;
  }

  .login {
    padding: 1em;
    margin: 2em auto;
    width: 17em;
    background: #fff;
    border-radius: 3px;
  }

  label {
    font-size: 10pt;
    color: #555;
  }

  input[type="text"],
  input[type="email"],
  textarea {
    padding: 8px;
    width: 95%;
    background: #efefef;
    border: 0;
    font-size: 10pt;
    margin: 6px 0px;
  }

  .tombol {
    background: #3498db;
    color: #fff;
    border: 0;
    padding: 5px 8px;
  }
```

![TUGAS (coding CSS)](https://user-images.githubusercontent.com/22215113/116094407-b5003f00-a6d1-11eb-8a22-9271b635723c.png)

- Hasil Akhir

![TUGAS (Hasil 1)](https://user-images.githubusercontent.com/22215113/116094428-b893c600-a6d1-11eb-86e1-fccaa9a3a9f4.png)

![TUGAS (Hasil 2)](https://user-images.githubusercontent.com/22215113/116094433-b92c5c80-a6d1-11eb-9111-aa5aab453d3c.png)
