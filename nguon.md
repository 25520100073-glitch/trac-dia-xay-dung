# Nguồn tài liệu & Báo cáo đối chiếu: Trắc địa xây dựng

Thư mục môn học: `C:\Workspace\01_Projects\HeThong\study\trac-dia-xay-dung\`  
Tài liệu gốc: `C:\Workspace\01_Projects\HeThong\`  
Cập nhật đối chiếu: Tối thứ Hai 12/10/2026 (Hoàn thành đối chiếu 100% bằng PyMuPDF và Python).

---

## 1. Giáo trình đối chiếu trực tiếp

- **Tên tài liệu**: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf` (156 trang, 3.3 MB).
- **Tác giả**: TS. Nguyễn Anh Tài, Bộ môn Thi công, Khoa Xây dựng, Trường ĐH Kiến trúc TP.HCM (Năm 2025).
- **Phương pháp đối chiếu**: Trích xuất và đọc trực tiếp lớp chữ bằng thư viện `pymupdf` (Python).
- **Kết quả đối chiếu mục lục và các chương**:
  - **Chương 1**: Những kiến thức chung về Trắc địa và bản đồ (trang 7–26).
  - **Chương 2**: NHỮNG KIẾN THỨC VỀ LÝ THUYẾT SAI SỐ (trang 27–36).
    - Mục 2.2.2 (trang 29): Sai số trung phương $m$.
    - Mục 2.3 (trang 31–32): Sai số trung phương trị đo và hàm trị đo (công thức $m_h = m_{đọc}\sqrt{2}$).
    - Mục 2.5 (trang 34): Nguyên tắc đồng ảnh hưởng - Ước tính độ chính xác.
  - **Chương 3**: DỤNG CỤ VÀ PHƯƠNG PHÁP ĐO TRONG TRẮC ĐỊA (trang 37–70).
    - Mục 3.1 (trang 37–51): Dụng cụ và phương pháp đo góc (máy kinh vĩ, 4 trục chính, kiểm nghiệm $2c$ và $MO$, đo đơn, đo toàn vòng).
    - Mục 3.2 (trang 52–62): Dụng cụ và phương pháp đo khoảng cách (thước thép trang 55–58; dây thị cự quang học trang 59–60 với $D = 100(c_t - c_d)$; bài tập trang 67).
    - Mục 3.3 (trang 63–70): Dụng cụ và phương pháp đo chênh cao.
      - 3.3.1 & 3.3.2 (trang 63–64): Máy, mia thủy chuẩn.
      - 3.3.3 (trang 64–65): Kiểm nghiệm máy thủy chuẩn (điều kiện $CC_1 \parallel LL_1$, sai số góc $i$).
      - 3.3.4 (trang 66–67): Đo thủy chuẩn từ giữa và phía trước.
      - 3.3.5 (trang 68): 6 nguồn sai số trong đo thủy chuẩn.
      - 3.3.6 (trang 69–70): Đo cao lượng giác ($h = D\tan V + i - l$).
  - **Chương 4**: LƯỚI KHỐNG CHẾ TRẮC ĐỊA (trang 71–114).
    - Mục 4.1.4 (trang 93–95): Hai bài toán trắc địa cơ bản (thuận, nghịch, xét dấu góc định hướng).
    - Mục 4.1.5 (trang 95–106): Phương pháp đường chuyền kinh vĩ mặt bằng (truyền góc định hướng công thức 4.1-5 & 4.1-11; bình sai tọa độ công thức 4.1-14).
    - Mục 4.2.1.5 (trang 108–109): Lưới độ cao kỹ thuật ($f_{hcp} = \pm 50\sqrt{L}$ mm hoặc $\pm 10\sqrt{N}$ mm).
    - Mục 4.2.2 (trang 110–113): Bình sai gần đúng đường chuyền độ cao (phù hợp trang 110–112; khép kín trang 112–113).
  - **Chương 5**: Đo vẽ và sử dụng bản đồ (trang 115–127).
  - **Chương 6**: Công tác bố trí công trình (trang 128–143) — Không thi giữa kỳ.
  - **Chương 7**: Quan trắc biến dạng công trình (trang 144–156) — Không thi giữa kỳ.

---

## 2. Ảnh chụp bài giảng (06/10/2026)

Toàn bộ 18 ảnh đã được phiên mã chi tiết vào `de-va-loi-giai-anh.md`:

| Slide | Tên file ảnh gốc | Nội dung đề bài & Lời giải | Kết quả kiểm tra Python |
|:---:|:---|:---|:---|
| **130** | `e7ca19ebabe62bb872f7.jpg`<br>`ed334518f615764b2f04.jpg` | Câu 3 (0.5đ + 0.5đ): Thủy chuẩn từ giữa $M \to N$, tính $h_{MN}$ và $H_N$ theo số $ZZ$. | Khớp 100% |
| **131** | `8062724fc142411c1853.jpg` | Câu 3 (1.0đ + 1.0đ): Sai số $m_h = m_{đọc}\sqrt{2} = \pm 0.707$ mm; $m_{đọc} \le 5/\sqrt{2} \approx \pm 3.536$ mm. | Khớp 100% |
| **145** | `df15d3386035e06bb924.jpg` | Câu 2 (2.0đ): Đề bài đo cao lượng giác công trình khi không tới chân mia ($D_1 = ZZ + 25$, $V_Đ = +15^\circ ZZ'$, $V_C = -20^\circ 30'$). | Khớp 100% |
| **146** | `080ffa3e4933c96d9022.jpg` | Câu 2: Công thức $h_{CĐ} = D(\tan V_Đ - \tan V_C)$. Hướng dẫn chiều cao máy $i$ triệt tiêu. | Khớp 100% |
| **196** | `9b07742bc72647781e37.jpg` | Lý thuyết lưới độ cao kỹ thuật: $f_{hcp} = \pm 50\sqrt{L}$ (km) hoặc $\pm 10\sqrt{N}$ (trạm). | Khớp giáo trình trang 108 |
| **197** | `2f9972b2c1bf41e118ae.jpg`<br>`f0b6ee9d5d90ddce8481.jpg`<br>`f16b054cb741371f6e50.jpg` | Quy trình 3 bước bình sai tuyến phù hợp; số liệu gốc ví dụ: $H_A = 55.216$ m, $H_B = 50.000$ m. | Khớp giáo trình trang 110 |
| **198** | `17d072edc1e041be18f1.jpg`<br>`95b98a983995b9cbe084.jpg`<br>`f0f8badf09d2898cd0c3.jpg` | Bảng tính bình sai theo chiều dài ($\sum D = 520$ m, $f_h = +24$ mm, $f_{hcp} = \pm 36$ mm, khớp $H_B = 50.000$ m). | Khớp 100% |
| **199** | `131b7826cb2b4b75123a.jpg`<br>`0a5b7c7ccf714f2f1660.jpg`<br>`2a5ebe6b0d668d38d477.jpg` | Bảng tính bình sai theo số trạm ($N = 340$, $f_h = +67$ mm, $f_{hcp} = \pm 184$ mm, $\sum v = -67$ mm). | Khớp 100% (Đã ghi chú thao tác làm tròn đoạn 4) |
| **200** | `c04f6796d49b54c50d8a.jpg` | Đề bài bình sai mốc công trình $A$ cốt $\pm 0.000$ từ hai mốc gốc $N_1, N_2$. | Khớp bài tập trang 67 |
| **201** | `08483a76897b0925506a.jpg`<br>`8a23921c2111a14ff800.jpg` | Lời giải bình sai mốc $A$: đổi dấu $h_1 = -h_{AN1} = +0.225$ m, $f_h = -15$ mm, tính ra $H_A = 20.232$ m, khớp $N_2 = 19.475$ m. | Khớp 100% |

---

## 3. Ghi chú kỹ thuật đối chiếu
1. **Bài tập trang 67 giáo trình**: Câu e ở trang 67 chính là đề bài của Slide 200 & 201 (Xác định độ cao mốc công trình $A$ từ trạm máy ngắm về hai mốc $N_1$ và $N_2$). Toàn bộ số liệu khớp tuyệt đối.
2. **Công thức truyền góc định hướng (Mục 4.1.5.3, trang 96–98)**:
   - Giáo trình viết cho góc ngoặt bên **Trái**: $\alpha_{sau} = \alpha_{trước} + \beta_{trái} - 180^\circ$.
   - Nếu đo góc ngoặt bên **Phải**: $\alpha_{sau} = \alpha_{trước} + 180^\circ - \beta_{phải}$.
   - Cả hai trường hợp đã được cập nhật rõ ràng trong `to-cong-thuc.md` và `binh-sai-duong-chuyen-kinh-vi.md`.
