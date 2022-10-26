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

```java
private String name;
private char jenisKelamin;
private int umur;
```

Kita membuat ketiga atribute tersebut menjadi private, dan ketika kita mengubahnya menjadi privatemaka atribute itu tidak bisa di akses di luar Class Person. Sehingga kita membuat seperti jembatan penghubungnya yaitu, Setter dan Getter.

- Setter: Penghubung yang berfungsi untuk mengisi sebuah nilai terhadap atribute private tersebut.
- Getter: Setelah nilai di isi, maka nilai tersebut akan kita panggil dengan Getter. Getter akan mengembalikan nilai yang telah di set di Setter.

Contoh *Setter:*</br>
```java
    public void setName(String name){
        this.name = name;
    }

    public void setUmur(int umur){
        this.umur = umur;
    }

    public void setJenisKelamin(char jenisKelamin){
        this.jenisKelamin = jenisKelamin;
    }
```

Contoh *Getter:*</br>
```java
    public String getName(){
        return this.name;
    }

    public int getUmur(){
        return this.umur;
    }

    public char getJenisKelamin(){
        return this.jenisKelamin;
    }
```

## Step 3

Setelah Class Person di buat maka kita bisa menaruh/menetapkan nilai dari atribut Person di Main.java. Kita tidak memanggil atribut tersebut secara langsung akan tetapi kita akan memanggil fungsi *Setter* untuk memberikan nilai dan fungsi *Getter* untuk mengembalikan nilai. Maka Full Code Main.java akan menjadi seperti berikut.

```java
public class Main {
    public static void main(String[] args) {
        Person person = new Person();
        Person person2 = new Person();

        // ANTON
        person.setName("Anton");
        person.setJenisKelamin('L');
        person.setUmur(20);
        System.out.println("Nama: " + person.getName());
        System.out.println("Jenis Kelamin: " + person.getJenisKelamin());
        System.out.println("Umur: " + person.getUmur());

        System.out.println();

        // RIKO
        person2.setName("Riko");
        person2.setJenisKelamin('L');
        person2.setUmur(25);
        System.out.println("Nama: " + person2.getName());
        System.out.println("Jenis Kelamin: " + person2.getJenisKelamin());
        System.out.println("Umur: " + person2.getUmur());
    }
}
```

