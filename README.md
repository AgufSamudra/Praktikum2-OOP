# Praktikum2-OOP

*Nama: Gufranaka Samudra*</br>
*NIM: 312110300*</br>
*Matkul: Pemrograman Berorientasi Objek*</br>

## Step 1
Software yang saya gunakan adalah intellij IDEA sebagai IDE Java, saya melakukan new projek pada software tersebut dan tercipta Main.java.

## Step 2
Saya membuat file java baru/class baru bernama Person, kemudian Person akan di isi dengan 3 atribut yaitu,
- Nama
- Jenis Kelamin
- Umur

Kita membuat ketiga atribute tersebut menjadi private, dan ketika kita mengubahnya menjadi private 
`private String name;
    private char jenisKelamin;
    private int umur;`
maka atribute itu tidak bisa di akses di luar Class Person. Sehingga kita membuat seperti jembatan penghubungnya yaitu, Setter dan Getter.

- Setter: Penghubung yang berfungsi untuk mengisi sebuah nilai terhadap atribute private tersebut.
- Getter: Setelah nilai di isi, maka nilai tersebut akan kita panggil dengan Getter. Getter akan mengembalikan nilai yang telah di set di Setter.

Contoh *Setter:*</br>
`public void setName(String name){
        this.name = name;
    }

    public void setUmur(int umur){
        this.umur = umur;
    }

    public void setJenisKelamin(char jenisKelamin){
        this.jenisKelamin = jenisKelamin;
    }`
