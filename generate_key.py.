import random
import string

def generate_key():
    # Menghasilkan kunci acak yang terdiri dari huruf kapital dan angka
    # Panjang kunci diatur 12 karakter
    characters = string.ascii_uppercase + string.digits
    new_key = ''.join(random.choices(characters, k=12))
    
    # Menyimpan kunci ke dalam file bernama 'Key'
    # File ini akan otomatis diperbarui setiap kali script dijalankan oleh GitHub Actions
    try:
        with open('Key', 'w') as f:
            f.write(new_key)
        print(f"Berhasil menghasilkan kunci baru: {new_key}")
    except Exception as e:
        print(f"Terjadi kesalahan saat menyimpan kunci: {e}")

if __name__ == "__main__":
    generate_key()
