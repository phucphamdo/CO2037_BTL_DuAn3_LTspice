# Báo Cáo Bài Tập Lớn -- Dự Án 3: Xây Dựng Tài Liệu Thực Hành Mới Với LTspice

> **Học phần:** Linh kiện và Mạch điện tử (CO2037)  
> **Khoa:** Khoa học và Kỹ thuật Máy tính  
> **Trường:** Đại học Bách Khoa -- ĐHQG-HCM  
> **Học kỳ:** HK251 (Năm học 2026--2027)  
> **Giảng viên hướng dẫn:** TS. Lê Trọng Nhân  
> **Lớp / Nhóm:** L01 -- Nhóm 9  

---

## 👥 Danh Sách Thành Viên Nhóm 9

| STT | Họ và Tên | MSSV | Lab Phụ Trách | Vai Trò Chính |
| :---: | :--- | :---: | :---: | :--- |
| 1 | **Phạm Đỗ Hồng Phúc** | 2510359 | Lab 1, Lab 2 | Cài đặt offline, đóng gói thư viện, kiểm tra SHA-256 |
| 2 | **Lê Lương Vỹ** | 2214056 | Lab 3, Lab 4 | Xây dựng bảng ánh xạ thao tác PSpice $\to$ LTspice |
| 3 | **Nguyễn Bảo Duy Thành** | 2510372 | Lab 5, Lab 6 | Kiểm thử chéo, tổng hợp và biên tập báo cáo |

---

## 📁 Cấu Trúc Repository

```text
CO2037_BTL_DuAn3_LTspice/
├── Mau_Bao_Cao_BTL_DuAn3.tex      # Mẫu báo cáo chuẩn theo đề bài (Phần B) - Có khung cam & hướng dẫn xám
├── Mau_Bao_Cao_BTL_DuAn3.pdf      # Bản PDF mẫu báo cáo (27 trang)
├── BaoCao_BaiTapLon_DuAn3.tex     # Báo cáo tham khảo hoàn chỉnh đầy đủ nội dung giải thích
├── BaoCao_BaiTapLon_DuAn3.pdf     # Bản PDF báo cáo chi tiết tham khảo (45 trang)
├── LoiGiai_ThamKhao_DuAn3.tex     # Solution Manual giải tích và số liệu mô phỏng đối chứng
├── source/
│   └── picture/
│       └── cover.png              # Hình ảnh logo/bìa trường ĐH Bách Khoa
├── .gitignore                     # Bỏ qua các file phụ trợ sinh ra khi biên dịch LaTeX
└── README.md                      # Tài liệu giới thiệu và hướng dẫn sử dụng
```

---

## 🛠️ Hướng Dẫn Biên Dịch LaTeX

Khuyến nghị sử dụng **XeLaTeX** để hỗ trợ hoàn hảo font Unicode tiếng Việt (Times New Roman):

```bash
xelatex -interaction=nonstopmode Mau_Bao_Cao_BTL_DuAn3.tex
xelatex -interaction=nonstopmode Mau_Bao_Cao_BTL_DuAn3.tex
```

*(Biên dịch 2 lần để mục lục tự động và danh mục bảng/hình ảnh cập nhật chính xác).*

---

## 📋 Tóm Tắt Nội Dung Mẫu Báo Cáo (Phần B)

1. **Thông tin nhóm (Bảng 5):** Thành viên, phiên bản LTspice, hệ điều hành.
2. **Giới thiệu:** Mục tiêu dự án, phạm vi 6 bài lab, sơ đồ quy trình thực hiện.
3. **Tìm hiểu LTspice & Cài đặt offline:** Nguồn tải, EULA, kịch bản silent install `install_offline.bat`, mã băm SHA-256.
4. **Ánh xạ PSpice for TI $\to$ LTspice:** Bảng đối chiếu 16 thao tác kỹ thuật then chốt.
5. **Tổng quan tài liệu mới (Bảng 6):** Thống kê 39 bài Giữ nguyên, 11 bài Điều chỉnh, 10 bài Thay thế, 12 bài Nâng cao (Tổng cộng 72 bài).
6. **Chi tiết từng bài Lab (Lab 1 đến Lab 6):**
   * Bảng 10 bài tập chính mỗi lab (Bảng 7 đến Bảng 12).
   * Danh mục 2 bài tập nâng cao mỗi lab.
   * Khung viền cam chèn ảnh bài tiêu biểu.
   * **Các mục con chi tiết từng bài (Bài 1 $\to$ Bài 10)** với khung viền cam chèn ảnh schematic, ảnh kết quả mô phỏng và phần giải thích đối chiếu lý thuyết.
7. **Bài tập không chuyển đổi được:** Giải pháp thay thế cho IC nguồn xung `LM2596`, diode `Dbreak`, linh kiện cách ly quang `Opto 4N25`.
8. **Trả lời câu hỏi [1] đến [9]:** Đề bài in nghiêng màu xám kèm khung viền cam để trống.
9. **Kiểm thử chéo (Bảng 13):** Ma trận kiểm tra chéo vòng tròn giữa các thành viên.
10. **Hướng dẫn cho giảng viên:** Cấu trúc bàn giao và phương pháp chấm bài tự động bằng lệnh `.meas`.
11. **Nhật ký sử dụng AI (Bảng 14):** Khai báo minh bạch các lượt tương tác AI.
12. **Phân công công việc (Bảng 15) & Kết luận.**
