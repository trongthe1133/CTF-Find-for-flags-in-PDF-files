# CTF Write-Up: Find-for-flags-in-PDF-files

## Mô tả bài thử thách  
Bài thử thách tại [viblo](https://ctf.viblo.asia/puzzles/pdf-m6w6gidsrpl) với tên pdf

Trong bài thử thách CTF này, chúng ta cần tìm kiếm Flag trong file PDF.
Truy cập url của đề bài, chúng ta sẽ tải file pdf được cung cấp.

## Phân tích vấn đề

Bài thử thách này yêu cầu tìm kiếm Flag bên trong file PDF, trên thực tế trong File PDF chỉ có hình, dự đoán Flag nằm phía sau bức hình.

## Giải pháp

### Giải pháp 1: Dùng [extract pdf](https://www.extractpdf.com/) để phân tách nội dung
Import file pdf đang có vào link để phân tích, sau khi phân tích sẽ tách các nội dung trong file ra và hiển thị Flag

```
flag{easy_show_flag_pdf_to_word}
```
![atl](Images/extractpdf)

### Giải pháp 2: Dùng convert file từ PDF sang Word

Sau khi convert file pdf sang word, chúng ta kéo hình ảnh ra vị trí khác và sẽ thấy được Flag

```
flag{easy_show_flag_pdf_to_word}
```
![atl](Images/converttoword)
