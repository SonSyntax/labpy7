# labpy7

## Dafar nilai mahasiswa menggunakan method

![bbb](https://github.com/user-attachments/assets/c29d082e-de60-4fc2-a489-ec62794bc93b)


```python
# DaftarNilaiMahasiswa.py

class DaftarNilaiMahasiswa:
    def __init__(self):
        # Inisialisasi daftar mahasiswa
        self.daftar_mahasiswa = []

    def tambah(self, nama, nilai):
        # Menambahkan data mahasiswa
        self.daftar_mahasiswa.append({"nama": nama, "nilai": nilai})
        print(f"Data mahasiswa {nama} berhasil ditambahkan.")

    def tampilkan(self):
        # Menampilkan seluruh data mahasiswa
        if not self.daftar_mahasiswa:
            print("Tidak ada data mahasiswa.")
        else:
            print("Daftar Nilai Mahasiswa:")
            for mahasiswa in self.daftar_mahasiswa:
                print(f"Nama: {mahasiswa['nama']}, Nilai: {mahasiswa['nilai']}")

    def hapus(self, nama):
        # Menghapus data berdasarkan nama mahasiswa
        for mahasiswa in self.daftar_mahasiswa:
            if mahasiswa['nama'] == nama:
                self.daftar_mahasiswa.remove(mahasiswa)
                print(f"Data mahasiswa {nama} berhasil dihapus.")
                return
        print(f"Data mahasiswa dengan nama {nama} tidak ditemukan.")

    def ubah(self, nama, nilai_baru):
        # Mengubah data nilai mahasiswa berdasarkan nama
        for mahasiswa in self.daftar_mahasiswa:
            if mahasiswa['nama'] == nama:
                mahasiswa['nilai'] = nilai_baru
                print(f"Nilai mahasiswa {nama} berhasil diubah menjadi {nilai_baru}.")
                return
        print(f"Data mahasiswa dengan nama {nama} tidak ditemukan.")

# Penggunaan program
if __name__ == "__main__":
    daftar = DaftarNilaiMahasiswa()
    
    # Menambah data mahasiswa
    daftar.tambah("Alice", 85)
    daftar.tambah("Bob", 90)
    
    # Menampilkan data
    daftar.tampilkan()
    
    # Mengubah nilai mahasiswa
    daftar.ubah("Alice", 95)
    
    # Menampilkan data setelah diubah
    daftar.tampilkan()
    
    # Menghapus data mahasiswa
    daftar.hapus("Bob")
    
    # Menampilkan data setelah dihapus
    daftar.tampilkan()

```

Penjelasan: 
1. `Mahasiswa` adalah kelas yang merepresentasikan objek mahasiswa dengan atribut `nama` dan `nilai`. 
2. `DaftarMahasiswa` adalah kelas yang mengelola daftar mahasiswa. Kelas ini memiliki metode untuk menambah, mengubah, menghapus, dan menampilkan daftar nilai mahasiswa.
3. Metode `tambah_mahasiswa` menambahkan mahasiswa baru ke dalam daftar.
4. Metode `ubah_nilai_mahasiswa` mengubah nilai mahasiswa berdasarkan nama.
5. Metode `hapus_mahasiswa` menghapus mahasiswa dari daftar berdasarkan nama.
6. Metode `daftar_nilai_mahasiswa` menampilkan daftar nilai semua mahasiswa. Contoh penggunaan di bagian bawah menunjukkan bagaimana metode-metode ini dapat digunakan untuk mengelola data mahasiswa.


<p>Berikut diagram class tersebut</p>

![dgr](https://github.com/user-attachments/assets/2c1e1bad-e327-465c-a924-9727b8b22e87)

<p>flowchart</p>

![flow bp 1](https://github.com/user-attachments/assets/58437db1-b69e-436c-8761-f543edfa6973)

![flo bp2](https://github.com/user-attachments/assets/23b06cb3-6b89-4bbd-996a-28d1572111ea)


