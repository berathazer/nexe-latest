
# Single Executable Application With Nexe

## Türkçe

### Projenin Amacı
Bu projenin amacı, javascript ile geliştirilen projeleri, `Nexe` kullanarak yürütülebilir bir dosya (exe) haline getirmektir.

### Gereksinimler
- Node.js yüklü olmalıdır.
- Nexe paketini yükleyin:
  ```sh
  npm install nexe -g
  ```

### Kullanım
Aşağıdaki komutu kullanarak bir JavaScript dosyasını .exe dosyasına dönüştürebilirsiniz:

```sh
nexe -i <YOUR_INPUT_FILE>.js --remote "https://github.com/berathazer/nexe-latest/raw/main/" -t "windows-x64-20.16.0"  -o <OUTPUT_FILE_NAME>.exe
```

### Parametreler
- `<YOUR_INPUT_FILE>.js`: .exe dosyasına dönüştürmek istediğiniz JavaScript dosyası.
- `<OUTPUT_FILE_NAME>.exe`: Oluşturulacak .exe dosyasının adı.
- `-t`: Hedef versiyon. Şu an için LTS sürüm olan v20.16.0 kullanılmaktadır, ancak ileride isteklere göre farklı versiyonlar eklenebilir.

### Örnek
Bir `app.js` dosyasını `app.exe` olarak dönüştürmek için aşağıdaki komutu kullanabilirsiniz:

```sh
nexe -i app.js --remote "https://github.com/berathazer/nexe-latest/raw/main/" -t "windows-x64-20.16.0"  -o app.exe
```

## English

### Project Purpose
The aim of this project is to turn projects developed with javascript into an executable file (exe) using `Nexe`.

### Requirements
- Node.js must be installed.
- Install Nexe package:
  ```sh
  npm install nexe -g
  ```

### Usage
You can convert a JavaScript file to an .exe file using the following command:

```sh
nexe -i <YOUR_INPUT_FILE>.js --remote "https://github.com/berathazer/nexe-latest/raw/main/" -t "windows-x64-20.16.0"  -o <OUTPUT_FILE_NAME>.exe
```

### Parameters
- `<YOUR_INPUT_FILE>.js`: The JavaScript file you want to convert to an .exe file.
- `<OUTPUT_FILE_NAME>.exe`: The name of the resulting .exe file.
- `-t`: Target version. Currently, the LTS version v20.16.0 is used, but different versions can be added according to requests in the future.

### Example
To convert an `app.js` file to `app.exe`, you can use the following command:

```sh
nexe -i app.js --remote "https://github.com/berathazer/nexe-latest/raw/main/" -t "windows-x64-20.16.0"  -o app.exe
```
