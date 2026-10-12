# Đề bài và Lời giải chi tiết từ 18 ảnh bài giảng (06/10/2026)

Tài liệu: `study/trac-dia-xay-dung/de-va-loi-giai-anh.md`  
Người lập: Antigravity  
Thời điểm: Tối thứ Hai 12/10/2026 (Phục vụ ôn thi giữa kỳ Trắc địa xây dựng)  
Nguồn dữ liệu gốc: 18 file ảnh chụp bảng và slide tại lớp của TS. Nguyễn Anh Tài (ĐH Kiến trúc TP.HCM).  
Mọi phép tính trong tài liệu này đều đã được kiểm tra độc lập bằng Python.

---

## 1. Slide 130: Thủy chuẩn hình học từ giữa (Câu 3 - Mục 3.1 & 3.2)

- **File ảnh**: `e7ca19ebabe62bb872f7.jpg`, `ed334518f615764b2f04.jpg`
- **Vị trí đề thi**: Câu 3 (tổng 3.0 điểm, trong đó 3.1 được 0.5 điểm, 3.2 được 0.5 điểm).
- **Đề bài chép nguyên văn**:
  > Đặt máy thủy chuẩn ở giữa hai điểm $M$ và $N$. Dựng mia thẳng đứng tại $M$ và $N$.
  > Đọc số trên mia sau tại $M$: chỉ giữa $a = 1000$ mm.
  > Đọc số trên mia trước tại $N$: chỉ giữa $b = 1000 + ZZ$ mm ($ZZ$ là số thứ tự riêng của sinh viên).
  > Biết cao độ mốc chuẩn $M$ là $H_M = 12.500$ m.
  > - **Câu 3.1 (0.5 điểm)**: Tính chênh cao giữa $M$ và $N$ ($h_{MN}$).
  > - **Câu 3.2 (0.5 điểm)**: Tính độ cao điểm $N$ ($H_N$).

### Lời giải chi tiết:

1. **Câu 3.1: Tính chênh cao $h_{MN}$**
   - Công thức thủy chuẩn từ giữa:
     $$h_{MN} = a - b \quad (\text{mia sau trừ mia trước})$$
   - Thay số theo $ZZ$:
     $$h_{MN} = 1000 - (1000 + ZZ) = -ZZ \text{ (mm)}$$
   - Đổi đơn vị sang mét (chia cho 1000):
     $$h_{MN} = -\frac{ZZ}{1000} \text{ (m)}$$

2. **Câu 3.2: Tính độ cao điểm $N$ ($H_N$)**
   - Công thức truyền độ cao:
     $$H_N = H_M + h_{MN}$$
   - Thay số:
     $$H_N = 12.500 + \left(-\frac{ZZ}{1000}\right) = 12.500 - \frac{ZZ}{1000} \text{ (m)}$$

### Bảng tra số mẫu cho các giá trị $ZZ$ (Kiểm tra bằng Python):

| $ZZ$ | Số đọc mia sau $a$ (mm) | Số đọc mia trước $b$ (mm) | Chênh cao $h_{MN}$ (mm) | Chênh cao $h_{MN}$ (m) | Độ cao $H_N$ (m) |
|:---:|:---:|:---:|:---:|:---:|:---:|
| **10** | 1000 | 1010 | $-10$ | $-0.010$ | $12.490$ |
| **20** | 1000 | 1020 | $-20$ | $-0.020$ | $12.480$ |
| **30** | 1000 | 1030 | $-30$ | $-0.030$ | $12.470$ |
| **45** | 1000 | 1045 | $-45$ | $-0.045$ | $12.455$ |

- **Nhận xét kiểm tra**: Vì $a < b$ (số đọc trước lớn hơn số đọc sau), điểm $N$ nằm thấp hơn điểm $M$, chênh cao $h_{MN}$ bắt buộc phải mang dấu âm ($-$). Lấy $b - a$ là sai bản chất và mất điểm.

---

## 2. Slide 131: Đánh giá độ chính xác & Sai số đọc mia (Câu 3 - Mục 3.3 & 3.4)

- **File ảnh**: `8062724fc142411c1853.jpg`
- **Vị trí đề thi**: Câu 3 (3.3 được 1.0 điểm, 3.4 được 1.0 điểm).
- **Đề bài chép nguyên văn**:
  > - **Câu 3.3 (1.0 điểm)**: Nếu sai số đọc số trên mia là $m_{đọc} = \pm 0.5$ mm, hãy tính sai số trung phương xác định chênh cao $h_{MN}$?
  > - **Câu 3.4 (1.0 điểm)**: Nếu yêu cầu sai số trung phương xác định chênh cao $h_{MN} \le \pm 5$ mm thì người đo phải đọc số với sai số đọc số $m_{đọc}$ là bao nhiêu?

### Lời giải chi tiết:

1. **Câu 3.3: Tính sai số trung phương chênh cao $m_h$**
   - Chênh cao được tính bởi hàm số hai đại lượng đo độc lập: $h_{MN} = a - b$.
   - Theo định luật truyền sai số trung phương của Gauss:
     $$m_{hMN} = \sqrt{m_a^2 + m_b^2}$$
   - Vì đo cùng loại mia và cùng điều kiện đọc số nên $m_a = m_b = m_{đọc} = 0.5$ mm:
     $$m_{hMN} = \sqrt{m_{đọc}^2 + m_{đọc}^2} = m_{đọc}\sqrt{2} = 0.5 \times \sqrt{2} \approx \pm 0.707 \text{ (mm)}$$

2. **Câu 3.4: Bài toán ngược tìm sai số đọc số cho phép $m_{đọc}$**
   - Điều kiện đề bài: $m_{hMN} \le \pm 5$ mm.
   - Thay công thức $m_{hMN} = m_{đọc}\sqrt{2}$ vào bất đẳng thức:
     $$m_{đọc}\sqrt{2} \le 5 \implies m_{đọc} \le \frac{5}{\sqrt{2}} \approx 3.536 \text{ (mm)}$$
   - **Kết luận**: Người đo phải đọc số trên mia với sai số trung phương tối đa là $m_{đọc} \le \pm 3.536$ mm (hoặc làm tròn an toàn là $\pm 3.5$ mm).

- **Kiểm tra Python**:
  - `0.5 * math.sqrt(2) = 0.70710678...` mm $\rightarrow$ làm tròn $0.707$ mm.
  - `5.0 / math.sqrt(2) = 3.5355339...` mm $\rightarrow$ làm tròn $3.536$ mm.
- **Lưu ý bẫy thi**: Quên nhân hoặc chia $\sqrt{2}$ (nghĩ rằng $m_h = m_{đọc}$) sẽ bị trừ toàn bộ 2 điểm của mục 3.3 và 3.4.

---

## 3. Slide 145 & 146: Đo cao lượng giác không thể tới chân mia (Câu 2 - 2.0 điểm)

- **File ảnh**: `df15d3386035e06bb924.jpg` (Slide 145 - Đề bài), `080ffa3e4933c96d9022.jpg` (Slide 146 - Hướng dẫn công thức)
- **Vị trí đề thi**: Câu 2 (2.0 điểm).
- **Đề bài chép nguyên văn**:
  > Xác định chiều cao công trình $h_{CĐ}$ (từ chân $C$ đến đỉnh $Đ$) bằng phương pháp đo cao lượng giác khi không thể tới chân mia.
  > Đặt máy kinh vĩ tại trạm 1:
  > - Khoảng cách ngang từ máy đến công trình: $D_1 = ZZ + 25$ (m).
  > - Góc đứng ngắm đỉnh $Đ$: $V_Đ = +15^\circ ZZ'$.
  > - Góc đứng ngắm chân $C$: $V_C = -20^\circ 30'$.
  > - Chiều cao gương/tiêu ngắm: ngắm sát chân và sát đỉnh nên $L_1 = L_2 = 0$.
  > - Tính chiều cao công trình $h_{CĐ}$.

### Hướng dẫn và Lời giải chi tiết:

1. **Bản chất công thức (Slide 146)**:
   - Cao độ đỉnh: $H_Đ = H_{trạm} + i + D_1 \tan V_Đ - L_1$.
   - Cao độ chân: $H_C = H_{trạm} + i + D_1 \tan V_C - L_2$.
   - Vì ngắm sát điểm nên $L_1 = L_2 = 0$. Chiều cao công trình là hiệu cao độ:
     $$h_{CĐ} = H_Đ - H_C = (H_{trạm} + i + D_1 \tan V_Đ) - (H_{trạm} + i + D_1 \tan V_C)$$
     $$h_{CĐ} = D_1 \cdot (\tan V_Đ - \tan V_C)$$
   - *Ghi chú trên Slide 146*: "Nếu đề bài không cho chiều cao máy $i$, sinh viên chọn $i$ bất kỳ hoặc lập luận $i$ bị triệt tiêu khi lấy hiệu số".

2. **Quy trình bấm máy tính**:
   - Đổi phút sang độ thập phân:
     $$V_Đ = 15^\circ + \frac{ZZ}{60}^\circ = \left(15 + \frac{ZZ}{60}\right)^\circ$$
     $$V_C = -20^\circ 30' = -20.5^\circ \implies \tan(-20.5^\circ) \approx -0.373885$$
   - Hiệu tang góc:
     $$\Delta \tan = \tan V_Đ - \tan V_C = \tan\left(15 + \frac{ZZ}{60}\right)^\circ - (-0.373885) = \tan\left(15 + \frac{ZZ}{60}\right)^\circ + 0.373885$$
   - Chiều cao công trình:
     $$h_{CĐ} = (ZZ + 25) \times \left[\tan\left(15 + \frac{ZZ}{60}\right)^\circ + 0.373885\right] \text{ (m)}$$

### Bảng tra số mẫu theo $ZZ$ (Kiểm tra chính xác bằng Python):

| $ZZ$ | $D_1$ (m) | $V_Đ$ | $\tan V_Đ$ | $V_C$ | $\tan V_C$ | $\Delta \tan = \tan V_Đ - \tan V_C$ | Chiều cao $h_{CĐ}$ (m) |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **10** | 35.000 | $+15^\circ 10' \approx 15.1667^\circ$ | $0.27107$ | $-20.5^\circ$ | $-0.37388$ | $0.64495$ | **22.573** |
| **15** | 40.000 | $+15^\circ 15' = 15.2500^\circ$ | $0.27263$ | $-20.5^\circ$ | $-0.37388$ | $0.64652$ | **25.861** |
| **20** | 45.000 | $+15^\circ 20' \approx 15.3333^\circ$ | $0.27419$ | $-20.5^\circ$ | $-0.37388$ | $0.64808$ | **29.164** |
| **25** | 50.000 | $+15^\circ 25' \approx 15.4167^\circ$ | $0.27575$ | $-20.5^\circ$ | $-0.37388$ | $0.64964$ | **32.482** |
| **30** | 55.000 | $+15^\circ 30' = 15.5000^\circ$ | $0.27732$ | $-20.5^\circ$ | $-0.37388$ | $0.65121$ | **35.817** |

- **Cảnh báo lỗi**:
  - Không được bấm $\tan(V_Đ - V_C)$, phải tính riêng $\tan V_Đ$ và $\tan V_C$.
  - Góc $V_C$ ngắm chúc xuống nên mang dấu âm; trừ cho số âm thành cộng.

---

## 4. Slide 196 & 197: Lý thuyết và Quy trình bình sai tuyến thủy chuẩn phù hợp

- **File ảnh**: `9b07742bc72647781e37.jpg` (Slide 196), `2f9972b2c1bf41e118ae.jpg`, `f0b6ee9d5d90ddce8481.jpg`, `f16b054cb741371f6e50.jpg` (Slide 197)
- **Nội dung lý thuyết cốt lõi**:
  1. **Hạn sai khép độ cao kỹ thuật ($f_{hcp}$)**:
     - Theo chiều dài toàn tuyến $L$ (địa hình đồng bằng / đồi thoải):
       $$f_{hcp} = \pm 50\sqrt{L} \quad (\text{mm, với } L = \frac{\sum D_i}{1000} \text{ tính bằng km})$$
     - Theo tổng số trạm máy $N$ (địa hình dốc, số trạm $> 25$ trạm/km):
       $$f_{hcp} = \pm 10\sqrt{N} \quad (\text{mm, với } N = \sum n_i \text{ là tổng số trạm})$$
  2. **Quy trình 3 bước bình sai tuyến phù hợp (Slide 197)**:
     - **Bước 1**: Tính sai số khép độ cao $f_h = \sum h_{đo} - (H_{cuối} - H_{đầu})$. Kiểm tra $|f_h| \le |f_{hcp}|$ (Đạt).
     - **Bước 2**: Tính số hiệu chỉnh cho từng đoạn:
       - Theo chiều dài: $v_{hi} = -\frac{f_h}{\sum D_i} \cdot D_i$.
       - Theo số trạm: $v_{hi} = -\frac{f_h}{N} \cdot n_i$.
       - Kiểm tra bù trừ: $\sum v_{hi} = -f_h$.
       - Chênh cao bình sai: $h_i^{BS} = h_{đo, i} + v_{hi}$ (Kiểm tra: $\sum h_i^{BS} = H_{cuối} - H_{đầu}$).
     - **Bước 3**: Tính cao độ bình sai lần lượt: $H_i = H_{i-1} + h_i^{BS}$. Kiểm tra mốc cuối phải khớp tuyệt đối $H_{cuối}$.

---

## 5. Slide 198: Bài toán bình sai theo chiều dài cạnh (Tuyến 6 đoạn, $\sum D = 520$ m)

- **File ảnh**: `17d072edc1e041be18f1.jpg`, `95b98a983995b9cbe084.jpg`, `f0f8badf09d2898cd0c3.jpg`
- **Số liệu đề bài**:
  - Tuyến đo từ mốc $A$ ($H_A = 55.216$ m) qua các điểm $KV1, KV2, KV3, KV4, KV5$ đến mốc $B$ ($H_B = 50.000$ m).
  - Chiều dài 6 đoạn: $D = [75, 77, 80, 95, 105, 88]$ m. Tổng $\sum D = 520$ m $= 0.520$ km.
  - Chênh cao đo: $h_{đo} = [-0.204, +0.345, +0.265, +0.410, -2.460, -3.548]$ m. Tổng $\sum h_{đo} = -5.192$ m.

### Lời giải và Kiểm tra toán học độc lập (Python):

1. **Kiểm tra sai số khép**:
   - Hiệu cao độ gốc: $\Delta H_{gốc} = H_B - H_A = 50.000 - 55.216 = -5.216$ m.
   - Sai số khép: $f_h = \sum h_{đo} - \Delta H_{gốc} = -5.192 - (-5.216) = +0.024$ m $= +24$ mm.
   - Hạn sai cho phép:
     $$f_{hcp} = \pm 50\sqrt{0.520} \approx \pm 50 \times 0.72111 \approx \pm 36.06 \text{ mm}$$
   - Đánh giá: $|f_h| = 24 \text{ mm} \le 36.06 \text{ mm} \implies$ **Tuyến đo ĐẠT chuẩn kỹ thuật**.

2. **Bảng bình sai chi tiết (Slide 198)**:

| Đoạn | Cự ly $D_i$ (m) | Chênh cao $h_{đo,i}$ (m) | Số hiệu chỉnh $v_i$ (m) | Chênh cao bình sai $h_i^{BS}$ (m) | Điểm | Độ cao bình sai $H$ (m) |
|:---|:---:|:---:|:---:|:---:|:---|:---:|
| | | | | | **A** | **55.216** |
| $A - KV1$ | 75 | $-0.204$ | $-0.003$ | $-0.207$ | $KV1$ | $55.009$ |
| $KV1 - KV2$ | 77 | $+0.345$ | $-0.004$ | $+0.341$ | $KV2$ | $55.350$ |
| $KV2 - KV3$ | 80 | $+0.265$ | $-0.004$ | $+0.261$ | $KV3$ | $55.611$ |
| $KV3 - KV4$ | 95 | $+0.410$ | $-0.004$ | $+0.406$ | $KV4$ | $56.017$ |
| $KV4 - KV5$ | 105 | $-2.460$ | $-0.005$ | $-2.465$ | $KV5$ | $53.552$ |
| $KV5 - B$ | 88 | $-3.548$ | $-0.004$ | $-3.552$ | **B** | **50.000** |
| **Tổng** | **520** | **-5.192** | **-0.024** | **-5.216** | | *(Khớp 100%)* |

- **Nhận xét kiểm tra phép tính**:
  - Giá trị tính chưa làm tròn của $v$: $[-0.00346, -0.00355, -0.00369, -0.00438, -0.00485, -0.00406]$.
  - Khi làm tròn đến milimét: $v = [-0.003, -0.004, -0.004, -0.004, -0.005, -0.004]$. Tổng đúng bằng $-0.024$ m.
  - Điểm cuối $H_B = 53.552 - 3.552 = 50.000$ m, trùng khít tuyệt đối với mốc gốc $B$.

---

## 6. Slide 199: Bài toán bình sai theo số trạm máy ($N = 340$ trạm)

- **File ảnh**: `131b7826cb2b4b75123a.jpg`, `0a5b7c7ccf714f2f1660.jpg`, `2a5ebe6b0d668d38d477.jpg`
- **Số liệu đề bài**:
  - Tuyến đo gồm 4 đoạn qua vùng sườn dốc hiểm trở với số trạm máy lần lượt:
    $$n_1 = 105, \quad n_2 = 60, \quad n_3 = 95, \quad n_4 = 80 \implies N = \sum n_i = 340 \text{ trạm}$$
  - Sai số khép tính được: $f_h = +0.067$ m $= +67$ mm.

### Lời giải và Ghi chú kiểm tra toán học với slide:

1. **Kiểm tra hạn sai cho phép theo số trạm**:
   $$f_{hcp} = \pm 10\sqrt{N} = \pm 10\sqrt{340} \approx \pm 10 \times 18.439 \approx \pm 184.4 \text{ mm}$$
   Vì $|f_h| = 67 \text{ mm} \le 184.4 \text{ mm} \implies$ **Tuyến đo ĐẠT**.

2. **Phân bổ số hiệu chỉnh $v_i = -\frac{f_h}{N} \cdot n_i$**:
   - Đoạn 1: $v_1 = -0.067 \times \frac{105}{340} \approx -0.02069 \text{ m} \rightarrow$ Làm tròn: **$-0.021$ m** ($-21$ mm).
   - Đoạn 2: $v_2 = -0.067 \times \frac{60}{340} \approx -0.01182 \text{ m} \rightarrow$ Làm tròn: **$-0.012$ m** ($-12$ mm).
   - Đoạn 3: $v_3 = -0.067 \times \frac{95}{340} \approx -0.01872 \text{ m} \rightarrow$ Làm tròn: **$-0.019$ m** ($-19$ mm).
   - Đoạn 4: $v_4 = -0.067 \times \frac{80}{340} \approx -0.01576 \text{ m}$.
     - *Ghi chú toán học quan trọng*: Nếu làm tròn toán học thông thường thì $-0.01576$ sẽ thành $-0.016$. Nhưng nếu lấy $-0.016$ thì tổng số hiệu chỉnh sẽ là $-0.021 - 0.012 - 0.019 - 0.016 = -0.068 \neq -0.067$.
     - **Do đó, trên slide thầy Tài đã cố ý làm tròn đoạn 4 là $-0.015$ m** để bảo toàn nguyên tắc bắt buộc:
       $$\sum v_i = -0.021 - 0.012 - 0.019 - 0.015 = -0.067 \text{ m} = -f_h$$

---

## 7. Slide 200 & 201: Bài tập xác định độ cao mốc công trình A

- **File ảnh**: `c04f6796d49b54c50d8a.jpg` (Slide 200 - Đề bài), `08483a76897b0925506a.jpg`, `8a23921c2111a14ff800.jpg` (Slide 201 - Lời giải)
- **Đề bài chép nguyên văn**:
  > Để xác định độ cao mốc công trình $A$ (cốt $\pm 0.000$), người ta đặt máy tại $A$ ngắm mia tại hai mốc gốc độ cao $N_1$ và $N_2$.
  > - Độ cao mốc gốc: $H_{N1} = 20.000$ m; $H_{N2} = 19.475$ m.
  > - Khoảng cách đo được: $D_{AN1} = 50$ m; $D_{AN2} = 54$ m $\implies \sum D = 104$ m.
  > - Chênh cao đo được từ máy tại $A$: $h_{AN1} = -0.225$ m ($-225$ mm); $h_{AN2} = -0.765$ m ($-765$ mm).
  > - Tiêu chuẩn cho phép: $f_{hcp} = \pm 100$ mm.
  > - Yêu cầu: Bình sai và tính cao độ mốc công trình $A$.

### Lời giải chi tiết từng bước:

1. **Thiết lập chiều tuyến đo truyền độ cao**:
   - Tuyến đi từ mốc gốc $N_1$ qua điểm công trình $A$ đến mốc gốc $N_2$ ($N_1 \rightarrow A \rightarrow N_2$).
   - **Đoạn 1 ($N_1 \rightarrow A$)**: Vì đề bài cho chênh cao $h_{AN1}$ (từ $A$ đến $N_1$), nên chênh cao theo chiều tuyến là:
     $$h_1 = h_{N1A} = -h_{AN1} = -(-0.225) = +0.225 \text{ m} \quad (D_1 = 50 \text{ m})$$
   - **Đoạn 2 ($A \rightarrow N_2$)**: Chiều đo trùng chiều tuyến nên giữ nguyên:
     $$h_2 = h_{AN2} = -0.765 \text{ m} \quad (D_2 = 54 \text{ m})$$
   - Tổng chênh cao đo toàn tuyến:
     $$\sum h_{đo} = h_1 + h_2 = +0.225 + (-0.765) = -0.540 \text{ m}$$

2. **Tính sai số khép độ cao $f_h$**:
   - Hiệu cao độ hai mốc gốc:
     $$\Delta H_{gốc} = H_{N2} - H_{N1} = 19.475 - 20.000 = -0.525 \text{ m}$$
   - Sai số khép:
     $$f_h = \sum h_{đo} - \Delta H_{gốc} = -0.540 - (-0.525) = -0.015 \text{ m} = -15 \text{ mm}$$
   - So sánh hạn sai:
     $$|f_h| = 15 \text{ mm} \le 100 \text{ mm} = f_{hcp} \implies \textbf{ĐẠT}$$

3. **Phân bổ số hiệu chỉnh $v_{hi}$**:
   - Tổng chiều dài tuyến: $\sum D = 50 + 54 = 104$ m.
   - Đoạn 1: $v_1 = -(-0.015) \times \frac{50}{104} \approx +0.00721 \text{ m} \rightarrow$ **$+0.007$ m** ($+7$ mm).
   - Đoạn 2: $v_2 = -(-0.015) \times \frac{54}{104} \approx +0.00779 \text{ m} \rightarrow$ **$+0.008$ m** ($+8$ mm).
   - Kiểm tra bù trừ: $\sum v = +0.007 + 0.008 = +0.015$ m $= -f_h$ (Thỏa mãn tuyệt đối).

4. **Tính chênh cao bình sai**:
   - $h_1^{BS} = h_1 + v_1 = +0.225 + 0.007 = +0.232$ m.
   - $h_2^{BS} = h_2 + v_2 = -0.765 + 0.008 = -0.757$ m.
   - Kiểm tra: $\sum h^{BS} = +0.232 - 0.757 = -0.525$ m $= \Delta H_{gốc}$.

5. **Xác định độ cao mốc công trình $A$ ($H_A$)**:
   $$H_A = H_{N1} + h_1^{BS} = 20.000 + 0.232 = \mathbf{20.232} \text{ (m)}$$
   - *Kiểm tra tính khép với mốc $N_2$*:
     $$H_{N2} = H_A + h_2^{BS} = 20.232 + (-0.757) = \mathbf{19.475} \text{ (m)} \quad (\text{Khớp 100\% mốc gốc})$$

- **Kiểm tra Python**: Khớp 100% không sai lệch một chữ số nào so với Slide 201 của TS. Nguyễn Anh Tài.

---

## 8. Bảng tổng hợp đối chiếu 18 ảnh bài giảng

| Nhóm bài | Slide | File ảnh | Trạng thái đối chiếu & Phép tính |
|:---|:---:|:---|:---|
| **Thủy chuẩn từ giữa (Câu 3)** | 130 | `e7ca19ebabe62bb872f7.jpg`, `ed334518f615764b2f04.jpg` | Đã chép đủ, Python verified |
| **Sai số đọc mia (Câu 3)** | 131 | `8062724fc142411c1853.jpg` | Đã chép đủ, công thức $\sqrt{2}$, Python verified |
| **Đo cao lượng giác (Câu 2)** | 145, 146 | `df15d3386035e06bb924.jpg`, `080ffa3e4933c96d9022.jpg` | Đã chép đủ, bảng thay số $ZZ$, Python verified |
| **Lý thuyết tuyến đo cao** | 196, 197 | `9b07742bc72647781e37.jpg`, `2f9972b2c1bf41e118ae.jpg`, `f0b6ee9d5d90ddce8481.jpg`, `f16b054cb741371f6e50.jpg` | Đã chép đủ 3 bước và công thức hạn sai |
| **Bình sai theo chiều dài** | 198 | `17d072edc1e041be18f1.jpg`, `95b98a983995b9cbe084.jpg`, `f0f8badf09d2898cd0c3.jpg` | Đã giải bảng 6 đoạn, khớp mốc $B=50.000$ m |
| **Bình sai theo số trạm** | 199 | `131b7826cb2b4b75123a.jpg`, `0a5b7c7ccf714f2f1660.jpg`, `2a5ebe6b0d668d38d477.jpg` | Đã giải, ghi rõ chỗ thầy ép làm tròn đoạn 4 |
| **Bình sai mốc công trình A** | 200, 201 | `c04f6796d49b54c50d8a.jpg`, `08483a76897b0925506a.jpg`, `8a23921c2111a14ff800.jpg` | Đã giải, đổi dấu $h_1 = -h_{AN1}$, $H_A = 20.232$ m |
