# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Tóm tắt ngắn gọn mục tiêu của bài lab.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 | 8 | Dữ liệu lặp hoàn toàn, cực kỳ dễ đoán, độ dư thừa tối đa. |
| abcd | 2 | 6 | Các ký tự phân bố đều, khó đoán hơn chuỗi lặp. |
| hello world | 2.84535 | 5.155 | Chuỗi thực tế có sự lặp lại của một số ký tự (l, o), entropy mức trung bình. |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 |  |
| 10 | 17 | 12 |  |
| 6 | 9 | Không tồn tại |  |

## 4. Kết luận
- **Kiến thức học được:** Hiểu rõ hơn về ý nghĩa thực tế của Entropy (dữ liệu càng lặp thì entropy càng thấp, redundancy càng cao) và cách hoạt động của thuật toán Euclid mở rộng khi áp dụng vào code.
- **Khó khăn:** Quá trình cài đặt môi trường trình biên dịch C++ (g++) trên Windows (MSYS2) gặp lỗi biến môi trường và quyền truy cập.
- **Cách khắc phục:** Đã xử lý thành công bằng cách chạy cấp quyền Administrator và set lại biến môi trường Path.
