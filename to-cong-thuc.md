# 🧭 TỜ CÔNG THỨC TRẮC ĐỊA XÂY DỰNG - PHÒNG THI (CHƯƠNG 3 & 4)

> **Tài liệu mang vào phòng thi**: Tóm tắt ngắn gọn các dạng đề, chỉ ghi các biến số dữ liệu cho (không ghi số cụ thể), kèm công thức chi tiết từng bước giải.

---

## DẠNG 1: THỦY CHUẨN TỪ GIỮA & TRUYỀN ĐỘ CAO (Slide 130; Bài 1)
- **Dữ liệu cho**: Mia sau tại $M$ đọc chỉ giữa $a$ (mm); Mia trước tại $N$ đọc chỉ giữa $b$ (mm); Độ cao mốc chuẩn $H_M$ (m).
- **Bước 1**: Tính chênh cao $h_{MN}$ (Sau trừ Trước):
  $$h_{MN} = a - b \text{ (mm)} \implies h_{MN} = \frac{a - b}{1000} \text{ (m)}$$
  *(Lưu ý: Nếu $a < b$ thì $h_{MN} < 0$. Tuyệt đối không lấy $b - a$).*
- **Bước 2**: Tính độ cao điểm trước $H_N$:
  $$H_N = H_M + h_{MN} \text{ (m)}$$

---

## DẠNG 2: SAI SỐ TRUNG PHƯƠNG THỦY CHUẨN & BÀI TOÁN NGƯỢC (Slide 131; Bài 1)
- **Dữ liệu cho**: Sai số đọc mia $m_{đọc}$ (mm); hoặc yêu cầu hạn sai chênh cao trạm máy $m_{h,cp}$ (mm); hoặc số trạm máy $N$.
- **Bước 1 (Bài toán thuận)**: Sai số chênh cao 1 trạm máy:
  $$m_h = \sqrt{m_a^2 + m_b^2} = \sqrt{m_{đọc}^2 + m_{đọc}^2} = m_{đọc} \cdot \sqrt{2} \text{ (mm)}$$
- **Bước 2 (Bài toán ngược)**: Điều kiện $m_h \le m_{h,cp}$, tìm sai số đọc mia tối đa:
  $$m_{đọc} \le \frac{m_{h,cp}}{\sqrt{2}} \text{ (mm)}$$
- **Bước 3 (Toàn tuyến)**: Sai số tích lũy qua $N$ trạm máy độc lập:
  $$m_{tuyến} = m_h \cdot \sqrt{N} = m_{đọc} \cdot \sqrt{2N} \text{ (mm)}$$

---

## DẠNG 3: ĐO CAO LƯỢNG GIÁC CÔNG TRÌNH TỪ XA (Slide 145–146; Bài 2)
- **Dữ liệu cho**: Khoảng cách ngang $D$ (m); Góc đứng ngắm đỉnh $V_Đ$ (độ ngẩng); Góc đứng ngắm chân $V_C$ (độ chúc); Chiều cao gương $L_1 = L_2 = 0$; Chiều cao máy $i$ không cho.
- **Bước 1**: Đổi phút sang độ thập phân & xác định dấu góc:
  $$V_Đ = \text{độ} + \frac{\text{phút}}{60} > 0; \quad V_C = -\left(\text{độ} + \frac{\text{phút}}{60}\right) < 0$$
- **Bước 2**: Lập luận chứng minh $i$ triệt tiêu:
  $$H_Đ = H_{trạm} + i + D \tan V_Đ; \quad H_C = H_{trạm} + i + D \tan V_C$$
  $$h_{CĐ} = H_Đ - H_C = D \cdot (\tan V_Đ - \tan V_C)$$
- **Bước 3**: Bấm máy tính hiệu tang (trừ cho số âm thành cộng):
  $$\Delta \tan = \tan V_Đ - \tan V_C = \tan V_Đ + |\tan V_C|$$
- **Bước 4**: Tính chiều cao công trình:
  $$h_{CĐ} = D \times \Delta \tan \text{ (m)}$$
  *(Cảnh báo: Bấm riêng $\tan V_Đ - \tan V_C$, KHÔNG bấm gộp $\tan(V_Đ - V_C)$).*

---

## DẠNG 4: ĐO CAO TOÀN ĐẠC ĐIỆN TỬ NGẮM THÁP (Giáo trình tr. 69–70; Bài 3)
- **Dữ liệu cho**: Trạm máy tại $A$ cao $i$ (m). Ngắm đỉnh 1: cự ly nghiêng $S_1$, góc đứng $V_1$, chiều cao gương $L_1$. Ngắm chân 2: cự ly nghiêng $S_2$, góc đứng $V_2$, chiều cao gương $L_2$.
- **Bước 1**: Tính chênh cao đo:
  $$h'_1 = S_1 \cdot \sin V_1 \text{ (m)}; \quad h'_2 = S_2 \cdot \sin V_2 \text{ (m)}$$
- **Bước 2**: Tính độ cao đỉnh và chân so với mốc trạm máy:
  $$\Delta H_1 = i + h'_1 - L_1 \text{ (m)}; \quad \Delta H_2 = i + h'_2 - L_2 \text{ (m)}$$
- **Bước 3**: Tính chiều cao tháp:
  $$h = \Delta H_1 - \Delta H_2 = (h'_1 - L_1) - (h'_2 - L_2) \text{ (m)}$$

---

## DẠNG 5: ĐO CỰ LY BẰNG DÂY THỊ CỰ KHI TIA NGẮM NGANG (Giáo trình tr. 60; Bài 4)
- **Dữ liệu cho**: Mia đứng, tia ngắm nằm ngang ($V = 0^\circ$). Đọc 3 chỉ: chỉ trên $c_t$, chỉ giữa $c_g$, chỉ dưới $c_d$ (mm). Hằng số $K = 100$.
- **Bước 1**: Kiểm tra đọc số đối xứng: $c_g = (c_t + c_d)/2$ (lệch $\le 1 \div 2$ mm).
- **Bước 2**: Tính khoảng chắn mia $l$ (đổi ra mét):
  $$l = \frac{c_t - c_d}{1000} \text{ (m)}$$
- **Bước 3**: Tính cự ly ngang $D$:
  $$D = K \cdot l = 100 \times \frac{c_t - c_d}{1000} = \frac{c_t - c_d}{10} \text{ (m)}$$

---

## DẠNG 6: KHÔI PHỤC CHỈ THỊ CỰ BỊ CHE KHUẤT (Giáo trình tr. 60 & 67; Bài 5)
- **Dữ liệu cho**: Biết chỉ giữa $c_g$ và một chỉ ngoài ($c_d$ hoặc $c_t$). Chỉ còn lại bị che khuất. Hằng số $K = 100$.
- **Bước 1**: Khôi phục chỉ bị khuất qua chỉ giữa:
  - Nếu khuất chỉ trên: $c_t = 2c_g - c_d$ (mm).
  - Nếu khuất chỉ dưới: $c_d = 2c_g - c_t$ (mm).
- **Bước 2**: Tính khoảng cách nằm ngang $D$:
  $$D = 100 \times \frac{c_t - c_d}{1000} \text{ (m)} \quad \text{hoặc} \quad D = 200 \times \frac{|c_g - c_{ngoài}|}{1000} \text{ (m)}$$

---

## DẠNG 7: ĐO THỊ CỰ KHI TIA NGẮM NGHIÊNG GÓC V (Giáo trình tr. 60, CT 3.2-12; Bài 6)
- **Dữ liệu cho**: Mia đứng, tia ngắm nghiêng góc đứng $V$ ($|V| \ge 2^\circ$). Khoảng chắn mia $l = c_t - c_d$ (m); Hằng số $K = 100$.
- **Bước 1**: Đổi góc $V$ ra độ thập phân: $V = \text{độ} + \text{phút}/60$.
- **Bước 2**: Tính cự ly nằm ngang $D$:
  $$D = 100 \cdot l \cdot \cos^2 V \text{ (m)} \quad \left(\text{hoặc } D = 200 \cdot l' \cdot \cos^2 V\right)$$
  *(Lưu ý: Công thức có bình phương $\cos^2 V$).*

---

## DẠNG 8: SAI SỐ CHỈ TIÊU MO & GÓC ĐỨNG ĐÚNG V (Giáo trình tr. 41; Bài 7)
- **Dữ liệu cho**: Bàn độ đứng khắc vạch liên tục theo chiều kim đồng hồ ($0^\circ$ tại thiên đỉnh). Đọc 2 vị trí Thuận kính $Tr$ và Đảo kính $Ph$.
- **Bước 1**: Tính sai số chỉ tiêu $MO$:
  $$MO = \frac{Tr + Ph - 360^\circ}{2}$$
- **Bước 2**: Tính góc đứng đúng $V$:
  $$V = 90^\circ - Tr + MO \quad \left(\text{hoặc } V = Ph - 270^\circ - MO\right)$$

---

## DẠNG 9: KIỂM NGHIỆM SAI SỐ GÓC NGẮM 2c CỦA MÁY KINH VĨ (Giáo trình tr. 45; Bài 8)
- **Dữ liệu cho**: Ngắm mục tiêu xa trên bàn độ ngang ở 2 vị trí Thuận kính $Tr$ và Đảo kính $Ph$; Tiêu chuẩn cho phép $[2c]$ ($\le 20''$).
- **Bước 1**: Tính sai số ngắm $2c$:
  $$2c = Tr - Ph \pm 180^\circ$$
  *(Nếu $Tr - Ph < 0 \implies +180^\circ$; Nếu $Tr - Ph > 0 \implies -180^\circ$).*
- **Bước 2**: So sánh $|2c| \le [2c]$ ($\le 20''$) $\implies$ Kết luận ĐẠT hay CẦN HIỆU CHỈNH.

---

## DẠNG 10: BÌNH SAI TUYẾN THỦY CHUẨN THEO CHIỀU DÀI D_i (Slide 198; Giáo trình tr. 111; Bài 9)
- **Dữ liệu cho**: Mốc gốc $A$ ($H_A$), mốc gốc $B$ ($H_B$). Tuyến gồm $k$ đoạn với cự ly $D_i$ (m) và chênh cao đo $h_{đo, i}$ (m).
- **Bước 1**: Tính tổng chênh cao đo và sai số khép $f_h$:
  $$\Sigma h_{đo} = \sum_{i=1}^k h_{đo, i}; \quad \Delta H_{gốc} = H_B - H_A$$
  $$f_h = \Sigma h_{đo} - \Delta H_{gốc} \text{ (m)} \implies f_h \text{ (mm)} = f_h \times 1000$$
- **Bước 2**: Kiểm tra hạn sai khép $f_{hcp}$:
  $$L = \frac{\sum D_i}{1000} \text{ (km)}; \quad f_{hcp} = \pm 50\sqrt{L} \text{ (mm)}$$
  Điều kiện: $|f_h| \le |f_{hcp}| \implies$ ĐẠT YÊU CẦU.
- **Bước 3**: Tính số hiệu chỉnh $v_i$ cho từng đoạn:
  $$v_i = -f_h \times \frac{D_i}{\sum D_i} \text{ (mm)}$$
  *(Bắt buộc kiểm tra: $\sum v_i = -f_h$. Bù trừ 1 mm ở đoạn dài nhất nếu lệch do làm tròn).*
- **Bước 4**: Tính chênh cao bình sai và cao độ bình sai các điểm:
  $$h_i^{BS} = h_{đo, i} + \frac{v_i}{1000} \text{ (m)}; \quad H_j = H_{j-1} + h_j^{BS} \text{ (m)}$$
  *(Kiểm tra mốc cuối $H_B$ phải trùng khít 100% với đề cho).*

---

## DẠNG 11: BÌNH SAI THEO SỐ TRẠM MÁY n_i (Slide 199; Giáo trình tr. 109, 113)
- **Dữ liệu cho**: Vùng đồi dốc ($> 25$ trạm/km). Số trạm từng đoạn $n_i$, tổng trạm $N = \sum n_i$. Sai số khép $f_h$ (mm).
- **Bước 1**: Hạn sai cho phép theo số trạm:
  $$f_{hcp} = \pm 10\sqrt{N} \text{ (mm)} \implies |f_h| \le |f_{hcp}| \text{ (Đạt)}$$
- **Bước 2**: Phân bổ số hiệu chỉnh $v_i$:
  $$v_i = -f_h \times \frac{n_i}{N} \text{ (mm)}$$
- **Bước 3**: Nguyên tắc làm tròn: Luôn điều chỉnh làm tròn ở đoạn có số trạm lớn nhất để bảo toàn nghiêm ngặt $\sum v_i = -f_h$.

---

## DẠNG 12: BÌNH SAI MỐC CÔNG TRÌNH CỐT ±0.000 SÀN A (Slide 200–201; Giáo trình tr. 67; Bài 10)
- **Dữ liệu cho**: Máy đặt tại mốc công trình $A$ ($i$), ngắm 2 mốc gốc $N_1$ ($H_{N1}$) và $N_2$ ($H_{N2}$). Cự ly $D_1, D_2$; Chênh cao đo $h_{AN1}, h_{AN2}$; Hạn sai $f_{hcp}$.
- **Bước 1**: Tính chênh cao đo máy - mia (nếu đọc chỉ giữa $c_g$): $h = i - c_g$ (m).
- **Bước 2 (BƯỚC SỐNG CÒN)**: Lập tuyến $N_1 \to A \to N_2$ và **ĐỔI DẤU ĐOẠN ĐẦU**:
  $$h_1 = h_{N1A} = -h_{AN1} \text{ (ĐỔI DẤU)}; \quad h_2 = h_{AN2} \text{ (GIỮ NGUYÊN)}$$
- **Bước 3**: Tính sai số khép $f_h$:
  $$\Sigma h_{đo} = h_1 + h_2; \quad \Delta H_{gốc} = H_{N2} - H_{N1}; \quad f_h = \Sigma h_{đo} - \Delta H_{gốc} \text{ (mm)}$$
- **Bước 4**: Phân bổ số hiệu chỉnh $v_1, v_2$:
  $$v_1 = -f_h \times \frac{D_1}{D_1 + D_2} \text{ (mm)}; \quad v_2 = -f_h \times \frac{D_2}{D_1 + D_2} \text{ (mm)}$$
- **Bước 5**: Tính cao độ bình sai mốc cốt 0 sàn $A$:
  $$h_1^{BS} = h_1 + \frac{v_1}{1000} \text{ (m)} \implies H_A = H_{N1} + h_1^{BS} \text{ (m)}$$
  *(Kiểm tra tính khép với $N_2$: $H_A + h_2 + \frac{v_2}{1000} = H_{N2}$).*

---

## DẠNG 13: BÀI TOÁN TRẮC ĐỊA THUẬN (Giáo trình tr. 94; Bài 11)
- **Dữ liệu cho**: Điểm $A(X_A, Y_A)$; Cự ly $D_{AB}$; Góc định hướng $\alpha_{AB}$.
- **Bước 1**: Đổi góc $\alpha_{AB}$ ra độ thập phân.
- **Bước 2**: Tính số gia tọa độ ($X$ đi với $\cos$, $Y$ đi với $\sin$):
  $$\Delta X_{AB} = D_{AB} \cdot \cos\alpha_{AB}; \quad \Delta Y_{AB} = D_{AB} \cdot \sin\alpha_{AB}$$
- **Bước 3**: Tính tọa độ điểm $B$:
  $$X_B = X_A + \Delta X_{AB}; \quad Y_B = Y_A + \Delta Y_{AB}$$

---

## DẠNG 14: BÀI TOÁN TRẮC ĐỊA NGHỊCH (Giáo trình tr. 94; Bài 12)
- **Dữ liệu cho**: Tọa độ hai điểm $A(X_A, Y_A)$ và $B(X_B, Y_B)$.
- **Bước 1**: Tính số gia tọa độ:
  $$\Delta X = X_B - X_A; \quad \Delta Y = Y_B - Y_A$$
- **Bước 2**: Tính cự ly ngang:
  $$D_{AB} = \sqrt{\Delta X^2 + \Delta Y^2}$$
- **Bước 3**: Tính góc phương vị phụ $r$:
  $$r = \arctan \left| \frac{\Delta Y}{\Delta X} \right|$$
- **Bước 4**: Xét dấu $(\Delta X, \Delta Y)$ để tìm góc định hướng $\alpha_{AB}$:
  - Phần tư I ($\Delta X > 0, \Delta Y > 0$): $\alpha_{AB} = r$
  - Phần tư II ($\Delta X < 0, \Delta Y > 0$): $\alpha_{AB} = 180^\circ - r$
  - Phần tư III ($\Delta X < 0, \Delta Y < 0$): $\alpha_{AB} = 180^\circ + r$
  - Phần tư IV ($\Delta X > 0, \Delta Y < 0$): $\alpha_{AB} = 360^\circ - r$

---

## DẠNG 15: TRUYỀN GÓC ĐỊNH HƯỚNG TRONG ĐƯỜNG CHUYỀN (Giáo trình tr. 96, 98)
- **Dữ liệu cho**: Góc định hướng cạnh trước $\alpha_{trước}$; Góc ngoặt $\beta$ (trái hoặc phải).
- **Bước 1**: Áp dụng công thức:
  - Góc ngoặt bên **TRÁI**: $\alpha_{sau} = \alpha_{trước} + \beta_{trái} - 180^\circ$
  - Góc ngoặt bên **PHẢI**: $\alpha_{sau} = \alpha_{trước} + 180^\circ - \beta_{phải}$
- **Bước 2**: Hiệu chỉnh góc trong khoảng $[0^\circ, 360^\circ)$:
  - Nếu $\alpha_{sau} \ge 360^\circ \implies - 360^\circ$.
  - Nếu $\alpha_{sau} < 0^\circ \implies + 360^\circ$.

---

## CHECKLIST PHÒNG THI & QUY TẮC CASIO 580 / 880
1. **Đổi đơn vị**: Mia luôn là mm $\implies$ chia 1000 ra mét; Chiều dài $L$ trong $50\sqrt{L}$ luôn đổi sang **km**.
2. **Chế độ Casio**: Màn hình luôn ở chữ **D** (Deg), KHÔNG để chữ **R** (Radian).
3. **Quy tắc dấu**: Thủy chuẩn luôn là Sau - Trước ($a - b$); Góc ngắm chân công trình chúc xuống mang dấu âm ($V_C < 0$).
4. **Mốc công trình A**: Đoạn đầu bắt buộc đổi dấu $h_1 = -h_{AN1}$.
5. **Cân bằng số hiệu chỉnh**: Luôn kiểm tra $\sum v_i = -f_h$.
