# labpy7

```python
class Mahasiswa: def __init__(self, nama, nilai): self.nama = nama self.nilai = nilai class DaftarMahasiswa: def __init__(self): self.mahasiswa_list = [] def tambah_mahasiswa(self, nama, nilai): mahasiswa = Mahasiswa(nama, nilai) self.mahasiswa_list.append(mahasiswa) print(f"Data mahasiswa {nama} berhasil ditambahkan.") def ubah_nilai_mahasiswa(self, nama, nilai_baru): for mahasiswa in self.mahasiswa_list: if mahasiswa.nama == nama: mahasiswa.nilai = nilai_baru print(f"Nilai mahasiswa {nama} berhasil diubah menjadi {nilai_baru}.") return print(f"Mahasiswa dengan nama {nama} tidak ditemukan.") def hapus_mahasiswa(self, nama): for mahasiswa in self.mahasiswa_list: if mahasiswa.nama == nama: self.mahasiswa_list.remove(mahasiswa) print(f"Data mahasiswa {nama} berhasil dihapus.") return print(f"Mahasiswa dengan nama {nama} tidak ditemukan.") def daftar_nilai_mahasiswa(self): print("Daftar Nilai Mahasiswa:") for mahasiswa in self.mahasiswa_list: print(f"Nama: {mahasiswa.nama}, Nilai: {mahasiswa.nilai}") # Contoh penggunaan daftar = DaftarMahasiswa() daftar.tambah_mahasiswa("Alice", 85) daftar.tambah_mahasiswa("Bob", 90) daftar.daftar_nilai_mahasiswa() daftar.ubah_nilai_mahasiswa("Alice", 95) daftar.daftar_nilai_mahasiswa() daftar.hapus_mahasiswa("Bob") daftar.daftar_nilai_mahasiswa() 
```

Penjelasan: 
1. `Mahasiswa` adalah kelas yang merepresentasikan objek mahasiswa dengan atribut `nama` dan `nilai`. 
2. `DaftarMahasiswa` adalah kelas yang mengelola daftar mahasiswa. Kelas ini memiliki metode untuk menambah, mengubah, menghapus, dan menampilkan daftar nilai mahasiswa.
3. Metode `tambah_mahasiswa` menambahkan mahasiswa baru ke dalam daftar.
4. Metode `ubah_nilai_mahasiswa` mengubah nilai mahasiswa berdasarkan nama.
5. Metode `hapus_mahasiswa` menghapus mahasiswa dari daftar berdasarkan nama.
6. Metode `daftar_nilai_mahasiswa` menampilkan daftar nilai semua mahasiswa. Contoh penggunaan di bagian bawah menunjukkan bagaimana metode-metode ini dapat digunakan untuk mengelola data mahasiswa.
