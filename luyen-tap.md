# Tuyển tập bài tập luyện thi Trắc địa xây dựng (Chương 3 & 4)

Tài liệu: `study/trac-dia-xay-dung/luyen-tap.md`  
Cập nhật: Tối thứ Hai 12/10/2026 (Ôn thi cấp tốc giữa kỳ)  
Căn cứ: 18 ảnh bài giảng của TS. Nguyễn Anh Tài và Giáo trình ĐH Kiến trúc TP.HCM (2025).  
Quy chuẩn: Mỗi dạng bài có ít nhất 3 bài tập đầy đủ lời giải từng bước, có kiểm tra tự động: đổi đơn vị, xét dấu, $\sum v_i = -f_h$, và cao độ cuối khớp mốc gốc.

---

## Dạng 1: Thủy chuẩn hình học & Đo khoảng cách bằng chỉ thị cự (Chương 3)

### Tóm tắt phương pháp & Nguyên tắc làm bài:
1. **Kiểm tra chỉ đối xứng**: $c_{giữa} = \frac{c_{trên} + c_{dưới}}{2} \iff c_{trên} = 2c_{giữa} - c_{dưới}$.
2. **Khoảng cách thị cự**: $D = K \cdot (c_{trên} - c_{dưới})$ với hằng số nhân quang học $K = 100$. (Đổi mm ra m: chia 1000).
3. **Chênh cao từ giữa**: $h_{AB} = a - b = \text{mia sau} - \text{mia trước}$.
4. **Cao độ điểm trước**: $H_B = H_A + h_{AB}$.
5. **Tự kiểm tra**: $c_{trên} > c_{giữa} > c_{dưới}$; $a > b \implies h > 0$; $a < b \implies h < 0$.

---

### Bài 1.1 (Bài tập mẫu Slide 201 & Giáo trình trang 67)
- **Đề bài**: Đặt máy thủy chuẩn tại điểm $A$, chiều cao máy $i = 1.500$ m. Ngắm mia dựng tại hai mốc $N_1$ và $N_2$:
  - Mia $N_1$ đọc được 3 chỉ: $c_t = 1975$ mm; $c_g = 1725$ mm; $c_d = 1475$ mm.
  - Mia $N_2$ đọc được: chỉ dưới $c_d = 1995$ mm; chỉ giữa $c_g = 2265$ mm (chỉ trên bị che khuất).
  - a) Tính khoảng cách từ máy đến mia $N_1$ ($D_{AN1}$).
  - b) Tính chỉ trên tại $N_2$ và khoảng cách $D_{AN2}$.
  - c) Tính chênh cao thủy chuẩn phía trước $h_{AN1}$ và $h_{AN2}$.
  - d) Tính chênh cao giữa hai mốc $h_{N1N2}$.
- **Lời giải từng bước**:
  - **Câu a**:  
    Kiểm tra đối xứng: $\frac{1975 + 1475}{2} = 1725$ mm (Khớp chỉ giữa).  
    $D_{AN1} = 100 \times (1975 - 1475) = 100 \times 500\text{ mm} = 50000\text{ mm} = \mathbf{50.0\text{ m}}$.
  - **Câu b**:  
    Chỉ trên bị che khuất suy ra từ tính chất đối xứng:  
    $c_t = 2 \times c_g - c_d = 2 \times 2265 - 1995 = 4530 - 1995 = \mathbf{2535\text{ mm}}$.  
    $D_{AN2} = 100 \times (2535 - 1995) = 100 \times 540\text{ mm} = 54000\text{ mm} = \mathbf{54.0\text{ m}}$.
  - **Câu c**:  
    Áp dụng công thức thủy chuẩn phía trước: $h = i - c_g$:  
    $h_{AN1} = 1.500 - 1.725 = \mathbf{-0.225\text{ m}}$ ($-225$ mm).  
    $h_{AN2} = 1.500 - 2.265 = \mathbf{-0.765\text{ m}}$ ($-765$ mm).
  - **Câu d**:  
    $h_{N1N2} = H_{N2} - H_{N1} = (H_A + h_{AN2}) - (H_A + h_{AN1}) = h_{AN2} - h_{AN1}$:  
    $h_{N1N2} = -0.765 - (-0.225) = \mathbf{-0.540\text{ m}}$.
- **Tự kiểm tra**: $h_{N1A} = +0.225$ m; $h_{AN2} = -0.765$ m $\implies h_{N1N2} = +0.225 + (-0.765) = -0.540$ m (Khớp 100%).

---

### Bài 1.2 (Đo thủy chuẩn từ giữa trạm máy đơn lẻ)
- **Đề bài**: Đặt máy thủy chuẩn ở giữa hai điểm $A$ và $B$.
  - Ngắm mia sau tại $A$ đọc được 3 chỉ: $c_t = 1750$ mm; $c_g = 1500$ mm; $c_d = 1250$ mm.
  - Ngắm mia trước tại $B$ đọc được: chỉ trên $c_t = 1420$ mm; chỉ dưới $c_d = 1080$ mm (chỉ giữa chưa ghi).
  - Biết độ cao mốc chuẩn $H_A = 25.000$ m.
  - Tính khoảng cách từ máy đến hai mia ($D_{MA}, D_{MB}$), khoảng cách $D_{AB}$, chênh cao $h_{AB}$ và độ cao $H_B$.
- **Lời giải từng bước**:
  - **Bước 1**: Tính chỉ giữa mia trước tại $B$:  
    $c_{gB} = \frac{c_t + c_d}{2} = \frac{1420 + 1080}{2} = \frac{2500}{2} = \mathbf{1250\text{ mm}}$.
  - **Bước 2**: Tính khoảng cách thị cự:  
    $D_{MA} = 100 \times (1750 - 1250) = 100 \times 500\text{ mm} = \mathbf{50.0\text{ m}}$.  
    $D_{MB} = 100 \times (1420 - 1080) = 100 \times 340\text{ mm} = \mathbf{34.0\text{ m}}$.  
    Khoảng cách giữa hai điểm: $D_{AB} = D_{MA} + D_{MB} = 50.0 + 34.0 = \mathbf{84.0\text{ m}}$.
  - **Bước 3**: Tính chênh cao từ giữa $h_{AB} = a - b$:  
    $a = 1500$ mm; $b = 1250$ mm $\implies h_{AB} = 1500 - 1250 = +250\text{ mm} = \mathbf{+0.250\text{ m}}$.
  - **Bước 4**: Tính độ cao điểm $B$:  
    $H_B = H_A + h_{AB} = 25.000 + 0.250 = \mathbf{25.250\text{ m}}$.
- **Tự kiểm tra**: Vì $a = 1500 > b = 1250$, điểm $B$ cao hơn điểm $A$, $h_{AB} > 0$ và $H_B > H_A$ (Hợp lý trực quan).

---

### Bài 1.3 (Trường hợp mất chỉ trên và đọc số âm)
- **Đề bài**: Đặt máy thủy chuẩn từ giữa hai điểm $M$ và $N$.
  - Mia sau $M$: $c_t = 1860$ mm; $c_g = 1600$ mm; $c_d = 1340$ mm.
  - Mia trước $N$: chỉ giữa $c_g = 2150$ mm; chỉ dưới $c_d = 1900$ mm (chỉ trên bị tán cây che).
  - Biết $H_M = 10.200$ m.
  - Tính chỉ trên mia $N$, tổng chiều dài trạm đo $D_{MN}$, chênh cao $h_{MN}$ và độ cao $H_N$.
- **Lời giải từng bước**:
  - **Bước 1**: Chỉ trên tại $N$:  
    $c_{tN} = 2 \times 2150 - 1900 = 4300 - 1900 = \mathbf{2400\text{ mm}}$.
  - **Bước 2**: Khoảng cách:  
    $D_{MM} = 100 \times (1860 - 1340) = 100 \times 520\text{ mm} = 52.0$ m.  
    $D_{MN'} = 100 \times (2400 - 1900) = 100 \times 500\text{ mm} = 50.0$ m.  
    $D_{MN} = 52.0 + 50.0 = \mathbf{102.0\text{ m}}$.
  - **Bước 3**: Chênh cao $h_{MN} = a - b = 1600 - 2150 = -550\text{ mm} = \mathbf{-0.550\text{ m}}$.
  - **Bước 4**: Cao độ $N$:  
    $H_N = H_M + h_{MN} = 10.200 + (-0.550) = \mathbf{9.650\text{ m}}$.
- **Tự kiểm tra**: Đổi mm sang m: $-550 / 1000 = -0.550$ m; $10.200 - 0.550 = 9.650$ m (Chính xác).

---

## Dạng 2: Đánh giá độ chính xác đo cao & Sai số đọc mia (Chương 2 & Chương 3)

### Tóm tắt phương pháp & Nguyên tắc làm bài:
1. **Một trạm máy từ giữa**: $h = a - b \implies m_h = \sqrt{m_a^2 + m_b^2} = m_{đọc}\sqrt{2}$.
2. **Bài toán ngược 1 trạm**: $m_{đọc} \le \frac{m_{h,cp}}{\sqrt{2}} \approx 0.707 \cdot m_{h,cp}$.
3. **Tuyến gồm $N$ trạm máy**: $m_{tuyến} = m_h\sqrt{N} = m_{đọc}\sqrt{2N}$.
4. **Bài toán ngược tuyến $N$ trạm**: $m_{đọc} \le \frac{m_{tuyến,cp}}{\sqrt{2N}}$.
5. **Tự kiểm tra**: $m_h$ luôn lớn hơn $m_{đọc}$ khoảng $1.414$ lần; không bao giờ lấy $m_h = m_a - m_b$.

---

### Bài 2.1 (Đề thi Slide 131 - Đã kiểm tra Python)
- **Đề bài**:
  - a) Nếu sai số đọc số trên mia là $m_{đọc} = \pm 0.5$ mm, tính sai số trung phương xác định chênh cao $h_{MN}$ trong một trạm đo?
  - b) Nếu yêu cầu $m_{hMN} \le \pm 5$ mm thì người đo phải đọc số với sai số $m_{đọc}$ tối đa là bao nhiêu?
- **Lời giải từng bước**:
  - **Câu a**:  
    Hàm chênh cao: $h_{MN} = a - b$.  
    Theo định luật truyền sai số Gauss: $m_{hMN} = \sqrt{m_a^2 + m_b^2} = \sqrt{m_{đọc}^2 + m_{đọc}^2} = m_{đọc}\sqrt{2}$.  
    Thay số: $m_{hMN} = 0.5 \times \sqrt{2} \approx \mathbf{\pm 0.707\text{ mm}}$.
  - **Câu b**:  
    Điều kiện: $m_{hMN} \le 5\text{ mm} \iff m_{đọc}\sqrt{2} \le 5\text{ mm}$.  
    Suy ra: $m_{đọc} \le \frac{5}{\sqrt{2}} = \frac{5}{1.4142} \approx \mathbf{\pm 3.536\text{ mm}}$.
- **Tự kiểm tra**: $0.707 > 0.5$ mm; $3.536 \times \sqrt{2} = 5.000$ mm (Khớp hoàn toàn).

---

### Bài 2.2 (Đánh giá sai số toàn tuyến $N = 16$ trạm máy)
- **Đề bài**: Một tuyến thủy chuẩn kỹ thuật dẫn qua $N = 16$ trạm máy độc lập có cùng điều kiện đo.
  - a) Nếu sai số đọc số trên mia ở mỗi lần đọc là $m_{đọc} = \pm 1.0$ mm, tính sai số trung phương chênh cao toàn tuyến $m_{tuyến}$?
  - b) Để sai số trung phương toàn tuyến không vượt quá hạn sai $m_{tuyến,cp} = \pm 10$ mm thì sai số đọc số tại mỗi trạm tối đa là bao nhiêu?
- **Lời giải từng bước**:
  - **Câu a**:  
    Sai số một trạm: $m_h = m_{đọc}\sqrt{2} = 1.0 \times \sqrt{2} \approx 1.414$ mm.  
    Sai số tích lũy toàn tuyến qua $N = 16$ trạm:  
    $$m_{tuyến} = m_h\sqrt{N} = m_{đọc}\sqrt{2N} = 1.0 \times \sqrt{2 \times 16} = 1.0 \times \sqrt{32} \approx \mathbf{\pm 5.657\text{ mm}}$$
  - **Câu b**:  
    Điều kiện: $m_{tuyến} \le 10\text{ mm} \iff m_{đọc}\sqrt{2 \times 16} \le 10$.  
    Suy ra: $m_{đọc} \le \frac{10}{\sqrt{32}} = \frac{10}{5.6568} \approx \mathbf{\pm 1.768\text{ mm}}$.
- **Tự kiểm tra**: $1.768 \times \sqrt{32} = 10.000$ mm (Đạt chuẩn).

---

### Bài 2.3 (Hai lần đọc có độ chính xác khác nhau)
- **Đề bài**: Tại một trạm thủy chuẩn, người ngắm mia sau có kinh nghiệm đọc đạt sai số $m_a = \pm 0.8$ mm; người ngắm mia trước mới vào nghề đọc đạt sai số $m_b = \pm 0.6$ mm. Tính sai số trung phương chênh cao $m_h$ của trạm đo?
- **Lời giải từng bước**:
  - Vì hai số đọc độc lập nhưng có sai số khác nhau, áp dụng trực tiếp định luật Gauss tổng quát:  
    $$m_h = \sqrt{m_a^2 + m_b^2} = \sqrt{(0.8)^2 + (0.6)^2} = \sqrt{0.64 + 0.36} = \sqrt{1.00} = \mathbf{\pm 1.000\text{ mm}}$$
- **Tự kiểm tra**: $1.000 > \max(0.8, 0.6)$ (Đúng quy luật tích lũy sai số).

---

## Dạng 3: Đo cao lượng giác không thể tới chân mia (Chương 3)

### Tóm tắt phương pháp & Nguyên tắc làm bài:
1. **Chiều cao công trình**: $h_{CĐ} = D \cdot (\tan V_Đ - \tan V_C)$.
2. **Quy ước dấu góc đứng**: Ngắm chếch lên đỉnh $V_Đ > 0$; ngắm chúc xuống chân $V_C < 0$.
3. **Hiệu số tang**: $\Delta \tan = \tan V_Đ - \tan V_C = \tan V_Đ - (-|\tan V_C|) = \tan V_Đ + |\tan V_C|$.
4. **Đổi độ**: $V = \text{độ} + \frac{\text{phút}}{60}$.
5. **Tự kiểm tra**: Chiều cao $h_{CĐ} > 0$; không bao giờ bấm $\tan(V_Đ - V_C)$.

---

### Bài 3.1 (Bài tập mẫu Slide 145 & 146)
- **Đề bài**: Đo chiều cao ống khói $h_{CĐ}$. Đặt máy tại trạm 1: khoảng cách ngang $D_1 = 35.000$ m. Góc đứng ngắm đỉnh $V_Đ = +15^\circ 30'$, ngắm chân $V_C = -20^\circ 30'$. $L_1 = L_2 = 0$.
- **Lời giải từng bước**:
  - Đổi góc: $V_Đ = 15 + \frac{30}{60} = +15.5^\circ$; $V_C = -20 - \frac{30}{60} = -20.5^\circ$.
  - Tính tang:  
    $\tan(15.5^\circ) \approx 0.27732$.  
    $\tan(-20.5^\circ) \approx -0.37388$.
  - Hiệu tang: $\Delta \tan = 0.27732 - (-0.37388) = 0.27732 + 0.37388 = 0.65120$.
  - Chiều cao công trình:  
    $$h_{CĐ} = D_1 \cdot \Delta \tan = 35.000 \times 0.65120 = \mathbf{22.792\text{ m}}$$
- **Tự kiểm tra**: Kết quả dương, hợp lý với công trình cao tầng.

---

### Bài 3.2 (Công trình cao tầng kèm tính cao độ đỉnh $H_Đ$)
- **Đề bài**: Xác định chiều cao tòa nhà $h_{CĐ}$ và cao độ đỉnh tòa nhà $H_Đ$.
  - Đặt máy tại trạm có cao độ $H_{trạm} = 15.000$ m, chiều cao máy đo được là $i = 1.450$ m.
  - Khoảng cách ngang đến tòa nhà: $D = 40.000$ m.
  - Góc ngắm đỉnh: $V_Đ = +22^\circ 15'$.
  - Góc ngắm chân: $V_C = -12^\circ 45'$.
- **Lời giải từng bước**:
  - Đổi góc: $V_Đ = 22 + \frac{15}{60} = +22.25^\circ$; $V_C = -12 - \frac{45}{60} = -12.75^\circ$.
  - Tính tang:  
    $\tan(22.25^\circ) \approx 0.40909$.  
    $\tan(-12.75^\circ) \approx -0.22630$.  
    $\Delta \tan = 0.40909 - (-0.22630) = 0.40909 + 0.22630 = 0.63539$.
  - Chiều cao tòa nhà:  
    $$h_{CĐ} = D \cdot \Delta \tan = 40.000 \times 0.63539 = \mathbf{25.416\text{ m}}$$
  - Cao độ đỉnh tòa nhà:  
    $$H_Đ = H_{trạm} + i + D \tan V_Đ = 15.000 + 1.450 + 40.000 \times 0.40909 = 16.450 + 16.364 = \mathbf{32.814\text{ m}}$$
- **Tự kiểm tra**: Cao độ chân $H_C = 16.450 + 40 \times (-0.22630) = 16.450 - 9.052 = 7.398$ m.  
  Hiệu cao độ $H_Đ - H_C = 32.814 - 7.398 = 25.416$ m (Khớp tuyệt đối $h_{CĐ}$).

---

### Bài 3.3 (Trường hợp trạm máy đặt ở thấp, cả hai góc đều dương)
- **Đề bài**: Để đo chiều cao tháp truyền hình trên đỉnh đồi, máy đặt tại chân đồi cách tháp $D = 52.500$ m.
  - Góc đứng ngắm đỉnh tháp: $V_Đ = +18^\circ 30' = +18.5^\circ$.
  - Góc đứng ngắm chân tháp: $V_C = +2^\circ 15' = +2.25^\circ$ (ngắm ngước lên vì chân tháp ở trên đồi cao).
  - Tính chiều cao thân tháp $h_{CĐ}$?
- **Lời giải từng bước**:
  - Tính tang:  
    $\tan(18.5^\circ) \approx 0.33460$.  
    $\tan(2.25^\circ) \approx 0.03929$.
  - Hiệu tang: $\Delta \tan = \tan V_Đ - \tan V_C = 0.33460 - 0.03929 = 0.29531$.
  - Chiều cao thân tháp:  
    $$h_{CĐ} = D \cdot \Delta \tan = 52.500 \times 0.29531 = \mathbf{15.504\text{ m}}$$
- **Tự kiểm tra**: Vì cả hai góc đều ngắm lên trên đường chân trời, chiều cao bằng hiệu hai đoạn nhô lên: $52.5 \times 0.33460 - 52.5 \times 0.03929 = 17.567 - 2.063 = 15.504$ m (Chính xác).

---

## Dạng 4: Bình sai đường chuyền độ cao kỹ thuật phù hợp & khép kín (Chương 4)

### Tóm tắt phương pháp & Nguyên tắc làm bài:
1. **Sai số khép**: $f_h = \sum h_{đo} - (H_{cuối} - H_{đầu})$ (khép kín thì $H_{cuối} = H_{đầu} \implies f_h = \sum h_{đo}$).
2. **Hạn sai**: $f_{hcp} = \pm 50\sqrt{L\text{ (km)}}$ hoặc $\pm 10\sqrt{N}$.
3. **Số hiệu chỉnh**: $v_{hi} = -f_h \cdot \frac{D_i}{\sum D_i}$ (hoặc $-f_h \cdot \frac{n_i}{N}$). Kiểm tra: $\sum v_{hi} = -f_h$.
4. **Chênh cao bình sai**: $h_i^{BS} = h_{đo, i} + v_{hi}$. Kiểm tra: $\sum h^{BS} = H_{cuối} - H_{đầu}$.
5. **Cao độ**: $H_i = H_{i-1} + h_i^{BS}$. Kiểm tra: điểm cuối trùng khớp $H_{cuối}$.

---

### Bài 4.1 (Bình sai theo chiều dài cạnh $D_i$ - Slide 198)
- **Đề bài**: Tuyến phù hợp từ $A$ ($H_A = 55.216$ m) đến $B$ ($H_B = 50.000$ m) gồm 6 đoạn:
  - $D = [75, 77, 80, 95, 105, 88]$ m $\implies \sum D = 520$ m $= 0.520$ km.
  - $h_{đo} = [-0.204, +0.345, +0.265, +0.410, -2.460, -3.548]$ m $\implies \sum h_{đo} = -5.192$ m.
- **Lời giải từng bước**:
  - $\Delta H_{gốc} = 50.000 - 55.216 = -5.216$ m.
  - $f_h = -5.192 - (-5.216) = +0.024$ m $= +24$ mm.
  - $f_{hcp} = \pm 50\sqrt{0.520} \approx \pm 36.06$ mm. Đánh giá: $|24| \le 36.06 \implies$ ĐẠT.
  - Số hiệu chỉnh $v_{hi} = -0.024 \times \frac{D_i}{520}$ (làm tròn mm):  
    $v = [-0.003, -0.004, -0.004, -0.004, -0.005, -0.004]$ m.  
    $\sum v = -0.024$ m $= -f_h$ (Thỏa mãn).
  - Chênh cao bình sai $h^{BS} = h_{đo} + v$:  
    $h^{BS} = [-0.207, +0.341, +0.261, +0.406, -2.465, -3.552]$ m.  
    $\sum h^{BS} = -5.216$ m (Khớp tuyệt đối).
  - Cao độ bình sai:  
    $H_A = 55.216$ m  
    $H_{KV1} = 55.216 - 0.207 = \mathbf{55.009}$ m  
    $H_{KV2} = 55.009 + 0.341 = \mathbf{55.350}$ m  
    $H_{KV3} = 55.350 + 0.261 = \mathbf{55.611}$ m  
    $H_{KV4} = 55.611 + 0.406 = \mathbf{56.017}$ m  
    $H_{KV5} = 56.017 - 2.465 = \mathbf{53.552}$ m  
    $H_B = 53.552 - 3.552 = \mathbf{50.000}$ m (Khớp 100% mốc gốc).

---

### Bài 4.2 (Bình sai theo số trạm máy $n_i$ - Slide 199)
- **Đề bài**: Tuyến qua vùng sườn dốc hiểm trở gồm 4 đoạn với số trạm: $n = [105, 60, 95, 80]$ trạm $\implies N = 340$ trạm. Sai số khép tính được $f_h = +0.067$ m $= +67$ mm.
- **Lời giải từng bước**:
  - Hạn sai: $f_{hcp} = \pm 10\sqrt{340} \approx \pm 184.4$ mm. Đánh giá: $|67| \le 184.4 \implies$ ĐẠT.
  - Số hiệu chỉnh $v_i = -0.067 \times \frac{n_i}{340}$:  
    $v_1 = -0.067 \times 105 / 340 \approx \mathbf{-0.021\text{ m}}$ ($-21$ mm).  
    $v_2 = -0.067 \times 60 / 340 \approx \mathbf{-0.012\text{ m}}$ ($-12$ mm).  
    $v_3 = -0.067 \times 95 / 340 \approx \mathbf{-0.019\text{ m}}$ ($-19$ mm).  
    $v_4 = -0.067 \times 80 / 340 \approx -0.01576 \text{ m} \rightarrow \mathbf{-0.015\text{ m}}$ ($-15$ mm, ép số nguyên để khớp tổng).  
    Kiểm tra tổng: $\sum v = -0.021 - 0.012 - 0.019 - 0.015 = \mathbf{-0.067\text{ m}} = -f_h$.

---

### Bài 4.3 (Bình sai tuyến thủy chuẩn khép kín)
- **Đề bài**: Tuyến thủy chuẩn khép kín xuất phát từ mốc $A$ ($H_A = 10.000$ m) qua các điểm 1, 2, 3 rồi khép về $A$.
  - Chiều dài 4 đoạn: $D = [120, 150, 180, 150]$ m $\implies \sum D = 600$ m $= 0.600$ km.
  - Chênh cao đo: $h_{đo} = [+1.245, -0.630, -1.820, +1.185]$ m.
  - Yêu cầu: Tính $f_h$, $f_{hcp}$, bình sai và tính độ cao các điểm 1, 2, 3.
- **Lời giải từng bước**:
  - **Bước 1**: Tổng chênh cao: $\sum h_{đo} = +1.245 - 0.630 - 1.820 + 1.185 = -0.020$ m.  
    Vì tuyến khép kín nên $\Delta H_{gốc} = 0 \implies f_h = \sum h_{đo} = \mathbf{-0.020\text{ m}} = -20\text{ mm}$.  
    Hạn sai: $f_{hcp} = \pm 50\sqrt{0.600} \approx \pm 38.73$ mm. Vì $|-20| \le 38.73 \implies$ ĐẠT.
  - **Bước 2**: Số hiệu chỉnh $v_i = -(-0.020) \times \frac{D_i}{600} = +0.020 \times \frac{D_i}{600}$:  
    $v_1 = +0.020 \times 120/600 = \mathbf{+0.004\text{ m}}$  
    $v_2 = +0.020 \times 150/600 = \mathbf{+0.005\text{ m}}$  
    $v_3 = +0.020 \times 180/600 = \mathbf{+0.006\text{ m}}$  
    $v_4 = +0.020 \times 150/600 = \mathbf{+0.005\text{ m}}$  
    Kiểm tra: $\sum v = +0.004 + 0.005 + 0.006 + 0.005 = \mathbf{+0.020\text{ m}} = -f_h$.
  - **Bước 3**: Chênh cao bình sai $h^{BS} = h_{đo} + v$:  
    $h_1^{BS} = +1.245 + 0.004 = \mathbf{+1.249\text{ m}}$  
    $h_2^{BS} = -0.630 + 0.005 = \mathbf{-0.625\text{ m}}$  
    $h_3^{BS} = -1.820 + 0.006 = \mathbf{-1.814\text{ m}}$  
    $h_4^{BS} = +1.185 + 0.005 = \mathbf{+1.190\text{ m}}$  
    Kiểm tra: $\sum h^{BS} = +1.249 - 0.625 - 1.814 + 1.190 = \mathbf{0.000\text{ m}}$.
  - **Bước 4**: Cao độ bình sai:  
    $H_A = 10.000$ m  
    $H_1 = 10.000 + 1.249 = \mathbf{11.249\text{ m}}$  
    $H_2 = 11.249 - 0.625 = \mathbf{10.624\text{ m}}$  
    $H_3 = 10.624 - 1.814 = \mathbf{8.810\text{ m}}$  
    $H_A = 8.810 + 1.190 = \mathbf{10.000\text{ m}}$ (Khớp hoàn toàn điểm xuất phát).

---

## Dạng 5: Bình sai mốc công trình từ trạm máy ngắm về hai mốc gốc (Chương 4)

### Tóm tắt phương pháp & Nguyên tắc làm bài:
1. **Thiết lập chiều tuyến**: Đi từ mốc gốc $N_1 \rightarrow$ Mốc công trình $\rightarrow$ Mốc gốc $N_2$.
2. **ĐỔI DẤU CHÊNH CAO ĐOẠN ĐẦU**: $h_1 = h_{N1\_CT} = -h_{CT\_N1}$. Đoạn sau giữ nguyên: $h_2 = h_{CT\_N2}$.
3. **Áp dụng toàn bộ quy trình bình sai tuyến phù hợp**.
4. **Tự kiểm tra**: $H_{CT} = H_{N1} + h_1^{BS}$; kiểm tra tiếp $H_{CT} + h_2^{BS} = H_{N2}$ phải trùng khít 100%.

---

### Bài 5.1 (Bài tập mẫu Slide 200 & 201)
- **Đề bài**: Đặt máy tại cốt sàn công trình $A$ ngắm mia tại $N_1$ ($H_{N1} = 20.000$ m) và $N_2$ ($H_{N2} = 19.475$ m).  
  $D_{AN1} = 50$ m; $D_{AN2} = 54$ m $\implies \sum D = 104$ m.  
  $h_{AN1} = -0.225$ m; $h_{AN2} = -0.765$ m. Tiêu chuẩn $f_{hcp} = \pm 100$ mm.  
  Tính cao độ bình sai mốc công trình $A$.
- **Lời giải từng bước**:
  - Tuyến: $N_1 \rightarrow A \rightarrow N_2$.  
    $h_1 = -h_{AN1} = -(-0.225) = \mathbf{+0.225\text{ m}}$.  
    $h_2 = h_{AN2} = \mathbf{-0.765\text{ m}}$.  
    $\sum h_{đo} = +0.225 - 0.765 = -0.540$ m.
  - $\Delta H_{gốc} = 19.475 - 20.000 = -0.525$ m.  
    $f_h = -0.540 - (-0.525) = -0.015$ m $= -15$ mm.  
    $|-15| \le 100 \implies$ ĐẠT.
  - Số hiệu chỉnh:  
    $v_1 = -(-0.015) \times \frac{50}{104} \approx \mathbf{+0.007\text{ m}}$.  
    $v_2 = -(-0.015) \times \frac{54}{104} \approx \mathbf{+0.008\text{ m}}$.  
    $\sum v = +0.007 + 0.008 = +0.015$ m $= -f_h$.
  - Chênh cao bình sai:  
    $h_1^{BS} = +0.225 + 0.007 = \mathbf{+0.232\text{ m}}$.  
    $h_2^{BS} = -0.765 + 0.008 = \mathbf{-0.757\text{ m}}$.
  - Cao độ mốc công trình $A$:  
    $$H_A = H_{N1} + h_1^{BS} = 20.000 + 0.232 = \mathbf{20.232\text{ m}}$$
  - Kiểm tra với mốc $N_2$:  
    $$H_{N2} = 20.232 - 0.757 = \mathbf{19.475\text{ m}} \quad (\text{Khớp 100\%})$$

---

### Bài 5.2 (Mốc cốt nền móng $B$)
- **Đề bài**: Để dẫn cao độ vào mốc công trình $B$, người ta đặt máy tại $B$ ngắm về hai mốc khống chế $N_1$ ($H_{N1} = 15.000$ m) và $N_2$ ($H_{N2} = 14.850$ m).
  - Khoảng cách: $D_{BN1} = 60$ m; $D_{BN2} = 40$ m ($\sum D = 100$ m).
  - Chênh cao đo từ trạm $B$: $h_{BN1} = -0.450$ m; $h_{BN2} = -0.580$ m.
  - Tiêu chuẩn cho phép: $f_{hcp} = \pm 50$ mm.
  - Bình sai và tính cao độ mốc công trình $B$.
- **Lời giải từng bước**:
  - Tuyến: $N_1 \rightarrow B \rightarrow N_2$.  
    $h_1 = -h_{BN1} = -(-0.450) = \mathbf{+0.450\text{ m}}$.  
    $h_2 = h_{BN2} = \mathbf{-0.580\text{ m}}$.  
    $\sum h_{đo} = +0.450 + (-0.580) = -0.130$ m.
  - $\Delta H_{gốc} = H_{N2} - H_{N1} = 14.850 - 15.000 = -0.150$ m.  
    $f_h = -0.130 - (-0.150) = \mathbf{+0.020\text{ m}} = +20\text{ mm}$.  
    Vì $|+20| \le 50 \implies$ ĐẠT.
  - Số hiệu chỉnh:  
    $v_1 = -0.020 \times \frac{60}{100} = \mathbf{-0.012\text{ m}}$.  
    $v_2 = -0.020 \times \frac{40}{100} = \mathbf{-0.008\text{ m}}$.  
    $\sum v = -0.012 - 0.008 = \mathbf{-0.020\text{ m}} = -f_h$.
  - Chênh cao bình sai:  
    $h_1^{BS} = +0.450 - 0.012 = \mathbf{+0.438\text{ m}}$.  
    $h_2^{BS} = -0.580 - 0.008 = \mathbf{-0.588\text{ m}}$.
  - Cao độ mốc công trình $B$:  
    $$H_B = H_{N1} + h_1^{BS} = 15.000 + 0.438 = \mathbf{15.438\text{ m}}$$
  - Kiểm tra mốc $N_2$:  
    $$H_{N2} = 15.438 - 0.588 = \mathbf{14.850\text{ m}} \quad (\text{Khớp 100\%})$$

---

### Bài 5.3 (Mốc trục định vị công trình $C$)
- **Đề bài**: Dẫn độ cao cho mốc định vị $C$ từ hai mốc quốc gia $M$ ($H_M = 30.500$ m) và $N$ ($H_N = 31.200$ m).
  - Trạm máy tại $C$ đo ngắm được: $h_{CM} = -1.150$ m; $h_{CN} = -0.420$ m.
  - Khoảng cách: $D_{CM} = 80$ m; $D_{CN} = 120$ m ($\sum D = 200$ m).
  - Tiêu chuẩn cho phép: $f_{hcp} = \pm 40$ mm.
  - Tính cao độ bình sai mốc $C$.
- **Lời giải từng bước**:
  - Tuyến: $M \rightarrow C \rightarrow N$.  
    $h_1 = -h_{CM} = -(-1.150) = \mathbf{+1.150\text{ m}}$.  
    $h_2 = h_{CN} = \mathbf{-0.420\text{ m}}$.  
    $\sum h_{đo} = +1.150 - 0.420 = +0.730$ m.
  - $\Delta H_{gốc} = 31.200 - 30.500 = +0.700$ m.  
    $f_h = +0.730 - (+0.700) = \mathbf{+0.030\text{ m}} = +30\text{ mm}$.  
    Vì $|+30| \le 40 \implies$ ĐẠT.
  - Số hiệu chỉnh:  
    $v_1 = -0.030 \times \frac{80}{200} = \mathbf{-0.012\text{ m}}$.  
    $v_2 = -0.030 \times \frac{120}{200} = \mathbf{-0.018\text{ m}}$.  
    $\sum v = -0.012 - 0.018 = \mathbf{-0.030\text{ m}} = -f_h$.
  - Chênh cao bình sai:  
    $h_1^{BS} = +1.150 - 0.012 = \mathbf{+1.138\text{ m}}$.  
    $h_2^{BS} = -0.420 - 0.018 = \mathbf{-0.438\text{ m}}$.
  - Cao độ mốc định vị $C$:  
    $$H_C = H_M + h_1^{BS} = 30.500 + 1.138 = \mathbf{31.638\text{ m}}$$
  - Kiểm tra mốc $N$:  
    $$H_N = 31.638 - 0.438 = \mathbf{31.200\text{ m}} \quad (\text{Khớp 100\%})$$
