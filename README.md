# Praktikum 5 - Pemrograman Web

```
Satria Dimas Permana
312010450
TI.20.B.2
Universitas Pelita Bangsa
```

## buat dokumen HTML dengan nama file lab5_javascript.html dan masukan coding

![LANGKAH 1 membuat javascript](https://user-images.githubusercontent.com/20396585/162877227-f0938879-c635-43cd-9d68-ab1d1f22ae83.png)


# Java Script Dasar

## Pemakaian Alert sebagai property window

![LANGKAH 2 membuat alert box](https://user-images.githubusercontent.com/20396585/162877391-84830abc-4f76-42c0-b480-cae3a1d1dee9.png)

## Pemakaian method dalam objek

![LANGKAH 3 Pemakaian metod](https://user-images.githubusercontent.com/20396585/162877449-020473ab-0f22-4a64-ac3a-f400aa569cfe.png)

## Pemakaian Prompt

![LANGKAH 4 Pemakaian prompt](https://user-images.githubusercontent.com/20396585/162877715-f08f4c8d-05d6-406f-a1e0-339c71bd0925.png)


## Pembuatan fungsi dan cara pemanggilannya

![LANGKAH 5 Pembuatan fungsi dan pemanggilan](https://user-images.githubusercontent.com/20396585/162877834-53d80551-7176-4f51-9dfc-39f783936a93.png)

# Dasar Pemrograman Di Javascript

## Operasi dasar Aritmatika

![LANGKAH 6 Operasi dasar Aritmatika](https://user-images.githubusercontent.com/20396585/162878008-8a5bc6fd-e5e1-4184-9eb6-48ed2fb6f3ae.png)


## Seleksi kondisi (if..else)

- Coding
  ![LANGKAH 7 seleksi kondisi (coding)](https://user-images.githubusercontent.com/20396585/162878111-6cc0ff7e-2586-40e6-a52a-d2291d90ca15.png)

- Output

![LANGKAH 7 seleksi kondisi (hasil 1)](https://user-images.githubusercontent.com/20396585/162878142-5c713d56-b4bb-4b5e-8d15-d413ee493106.png)


![LANGKAH 7 seleksi kondisi (hasil 2)](https://user-images.githubusercontent.com/20396585/162878185-157dda61-138d-4a33-b807-da7feaef6abc.png)


## Penggunaan operator switch untuk seleksi kondisi

- Coding
  ![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (coding)](https://user-images.githubusercontent.com/20396585/162878273-d5c65809-76a6-4ca2-87e9-b440fe76f2bf.png)

- Output

![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (hasil 1)](https://user-images.githubusercontent.com/20396585/162878337-07ff377c-d070-438b-beb1-d03d93dd7ac4.png)

![LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (hasil 2)](https://user-images.githubusercontent.com/20396585/162878381-4eb7cf8e-43bd-40ff-99a3-e7afe038e94f.png)


# Pembuatan Form

## Form Input

- Coding
  ![LANGKAH 9 Form input (coding)](https://user-images.githubusercontent.com/20396585/162878428-bb91e549-7ccf-4e5e-80f9-5056ca39741e.png)


- Output
  ![LANGKAH 9 Form input (hasil)](https://user-images.githubusercontent.com/20396585/162878464-1943dc47-77d4-4667-8e75-dcf64c278601.png)

## Form Button

- Coding
  ![LANGKAH 10 Form Button (coding)](https://user-images.githubusercontent.com/20396585/162878672-0c0e73be-8e76-4eec-82a9-e029407b2934.png)


- Output
  ![LANGKAH 10 Form Button (HASIL)](https://user-images.githubusercontent.com/20396585/162878723-96521374-0bf1-46c2-a40b-a9d523247af9.png)

## HTML DOM

- Coding
  ![LANGKAH 11 HTML DOM (coding)](https://user-images.githubusercontent.com/20396585/162879045-f00fec38-ea07-4f79-9511-62acdbb54fc6.png)


- Output
  ![LANGKAH 11 HTML DOM (hasil)](https://user-images.githubusercontent.com/20396585/162879083-942ecd36-5413-47f2-b5ab-c5c02eb80ef6.png)

# TUGAS

## 1. Buat script untuk melakukan validasi pada isian form.

- Buat form pada `tugas.html`

```
<!DOCTYPE html>
<html>
  <head>
    <title>Belajar JavaScript</title>
    <link rel="stylesheet" href="style.css" />
     Validasi JavaScript -->
    <script language="JavaScript">
      //   fungsi alphabet
      function cekAlphabet(input, pesan) {
        var alphaExp = /^[a-zA-Z ]+$/;
        if (input.value.match(alphaExp)) {
          return true;
        } else {
          alert(pesan);
          input.focus();
          return false;
        }
      }
      //   fungsi number
      function cekNumber(input, pesan) {
        var numberExp = /^[0-9]+$/;
        if (input.value.match(numberExp)) {
          return true;
        } else {
          alert(pesan);
          input.focus();
          return false;
        }
      }
      //   fungsi Email
      function cekEmail(input, pesan) {
        var email =
          /^([a-zA-Z0-9_.+-])+@(([a-zA-Z0-9-])+.)+([a-zA-Z0-9]{2,4})+$/;
        if (input.value.match(email)) {
          return true;
        } else {
          alert(pesan);
          input.focus();
          return false;
        }
      }
      function validasi() {
        cekAlphabet(
          document.getElementById("nama"),
          "Nama harus Huruf semua!!"
        );
        cekNumber(
          document.getElementById("telp"),
          "Telp. hanya berisi Number!!"
        );

        cekEmail(document.getElementById("email"), "Email tidak benar!!");
      }
    </script>
  </head>
  <body>
    <div class="login">
		<form action="beranda.html" method="POST" onSubmit="validasi()">
			<fieldset>
				<legend>Data User</legend>
				<div class="input-data">
					<label for="nama">Nama</label>
					<input type="text" id="nama" name="nama" required />
				</div>
				<div class="input-data">
					<label for="telp">Telp</label>
					<input type="text" id="telp" name="telp" required />
				</div>
				<div class="input-data">
					<label for="email">Email</label>
					<input type="text" id="email" name="email" required />
				</div>
				<div class="justify-right">
					<input type="submit" value="Daftar" class="tombol">
				</div>
		</form>
		</fieldset>
	</div>
  </body>
</html>
```

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
}

form {
  display: flex;
  justify-content: center;
}

form div {
  margin: 0.8rem 0rem;
}

form div > label {
  display: inline-block;
  width: 100px;
}

fieldset {
  width: fit-content;
}

input[type="text"] {
  width: 80%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  border: 1px solid #197a43;
}

input[type="submit"] {
  background-color: #4caf50;
  border: 1px solid #197a43;
  color: white;
  padding: 7px 10px;
  margin: 8px 0;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.flex {
  display: flex;
  justify-content: space-around;
}

.mx-1 {
  margin-right: 0.5rem;
  margin-left: 0.5rem;
}

.input-data {
  display: flex;
  align-items: center;
}

.justify-right {
  display: flex;
  justify-content: right;
}

```

- Hasil Akhir

![TUGAS (Hasil 1)](https://user-images.githubusercontent.com/20396585/162879396-9d323332-86db-4d03-988c-d9ffbed8ef25.png)

![TUGAS (Hasil 2)](https://user-images.githubusercontent.com/20396585/162879475-c4b9c0da-27b4-4e38-a055-3754594e653f.png)
