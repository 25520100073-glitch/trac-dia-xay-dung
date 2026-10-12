# Thủy chuẩn hình học (Geometric leveling / Differential leveling)

**1. Bản chất trong một câu.**  
Thủy chuẩn hình học xác định độ chênh lệch độ cao giữa hai điểm bằng cách dùng một tia ngắm nằm ngang chuẩn xác và đọc số chênh lệch trên hai mia đặt thẳng đứng tại các điểm đó.

**2. Vì sao cần nó.**  
Nếu không tạo được tia ngắm nằm ngang độc lập với độ dốc địa hình, ta không thể biết nước sẽ chảy về hướng nào, nền móng có bị nghiêng lệch hay không, và không thể truyền mốc độ cao chuẩn từ mặt biển (hải đồ) vào vị trí thi công công trình.

**3. Nguyên lý nền.**  
- Mặt thủy chuẩn (level surface) là mặt đẳng thế trọng trường, vuông góc với phương dây dọi tại mọi điểm (Chương 1).
- Tia ngắm của máy thủy chuẩn sau khi cân bằng bọt thủy nằm trong mặt phẳng nằm ngang tiếp tuyến với mặt thủy chuẩn (Chương 3).
- Định luật quang học đường ngắm và khoảng cách chỉ thị cự: $D = 100 \cdot (c_{trên} - c_{dưới})$ (Chương 3).

**4. Mô hình hóa.**  
- Giả thiết: Trục đứng máy $VV_1$ thẳng đứng; trục ngắm $CC_1$ song song với trục bọt thủy dài $LL_1$; mia dựng thẳng đứng vuông góc với mặt đất; khoảng cách đo ngắn ($D < 100$ m) để bỏ qua ảnh hưởng của độ cong Trái Đất và chiết quang khí quyển.
- Điều kiện mất hiệu lực: Khoảng cách từ máy đến hai mia chênh lệch nhau quá lớn khi máy chưa hiệu chỉnh sai số góc $i$ (tia ngắm không nằm ngang), hoặc nền đất đặt chân máy/mia bị lún trong quá trình đo.

**5. Suy công thức từ nguyên lý.**  
(a) Chiều đo từ điểm sau (Sau - $A$) đến điểm trước (Trước - $B$). Đặt máy ở giữa, ngắm mia tại $A$ đọc chỉ giữa $a$ (số đọc sau), ngắm mia tại $B$ đọc chỉ giữa $b$ (số đọc trước).  
(b) Từ nguyên lý mặt phẳng ngang chuẩn: Cao độ tia ngắm $H_{tia} = H_A + a$.  
(c) Cao độ điểm $B$ tính theo tia ngắm: $H_B = H_{tia} - b$.  
(d) Hiệu hai đẳng thức để tìm chênh cao $h_{AB}$:  
$$h_{AB} = H_B - H_A = a - b \quad (\text{Thủy chuẩn từ giữa})$$  
(e) Trường hợp thủy chuẩn phía trước (đặt máy tại $A$, đo chiều cao máy $i$, đọc mia tại $B$ là $b$):  
$$h_{AB} = i - b \quad (\text{Thủy chuẩn phía trước})$$

**6. Kiểm tra bằng trực giác.**  
- Nếu $a > b$ (số đọc ở trạm sau lớn hơn số đọc ở trạm trước): Điểm sau thấp hơn, điểm trước nhô cao hơn $\Rightarrow h_{AB} > 0$.  
- Nếu $a = b$: Hai điểm có cùng độ cao tuyệt đối $\Rightarrow h_{AB} = 0$.  
- Khi tăng khoảng cách $D$, tia ngắm bị run và bề rộng vạch mia nhỏ đi, làm sai số đọc số tăng lên tỉ lệ thuận với cự ly.

**7. Bẫy khi thi.**  
- **Lẫn lộn thứ tự Sau và Trước**: Công thức luôn là $h = \text{Sau} - \text{Trước} = a - b$. Lấy nhầm $b - a$ sẽ bị ngược dấu chênh cao dẫn đến tính sai toàn bộ độ cao tuyến.
- **Quên đổi đơn vị khi đọc mia 3 chỉ**: Số đọc mia trong máy thường ghi bằng milimét (mm), nhưng độ cao $H$ và chênh cao $h$ tính toán trong bảng sổ phải quy đổi ra mét (m).
- **Tính sai khoảng cách chỉ thị cự khi mia bị che khuất**: Nếu mất chỉ trên, phải tính $c_{trên} = 2 \cdot c_{giữa} - c_{dưới}$ trước khi nhân hệ số 100; không được lấy $(c_{giữa} - c_{dưới}) \times 100$ trực tiếp mà không nhân 2.

**8. Liên kết.**  
- Kiến thức trước: Khái niệm độ cao tuyệt đối, mặt Geoid (Chương 1); cấu tạo bọt thủy và ống kính ngắm (Chương 3).  
- Kiến thức sau: Đánh giá sai số chuỗi trạm đo (Chương 2); bình sai tuyến thủy chuẩn phù hợp và khép kín (Chương 4); bố trí cốt sàn $+0.000$ (Chương 6); quan trắc lún móng nhà cao tầng (Chương 7).

**9. Tự kiểm tra.**  
- **Bản chất**: Vì sao phương pháp thủy chuẩn từ giữa (đặt máy cách đều hai mia) loại trừ được sai số do góc nghiêng trục ngắm $i$ và độ cong Trái Đất?  
  *Đáp*: Vì khi khoảng cách $S_1 = S_2$, độ lệch do góc $i$ và độ võng Trái Đất gây ra trên hai mia là bằng nhau ($\Delta h_a = \Delta h_b$). Khi lấy hiệu $h = (a + \Delta h_a) - (b + \Delta h_b) = a - b$, các sai số này tự triệt tiêu hoàn toàn.
- **Áp dụng**: Đặt máy ở giữa hai điểm $M$ và $N$. Số đọc chỉ giữa mia sau tại $M$ là $1000$ mm; mia trước tại $N$ là $1450$ mm. Biết $H_M = 12.500$ m. Tính $h_{MN}$ và $H_N$.  
  *Đáp*: $h_{MN} = a - b = 1000 - 1450 = -450\text{ mm} = -0.450\text{ m}$. Độ cao $H_N = H_M + h_{MN} = 12.500 + (-0.450) = 12.050\text{ m}$.
- **Bẫy**: Tại trạm đo từ $A$ đến $B$, người đo đọc mia sau $A$ có chỉ trên $1650$ mm, chỉ dưới $1350$ mm. Mia trước $B$ có chỉ giữa $1200$ mm. Người đó tính khoảng cách $D_{AB} = (1650 - 1350) \times 100 = 30$ m. Phép tính này đúng hay sai?  
  *Đáp*: Sai. Cự ly $30$ m đó chỉ là khoảng cách từ máy đến mia sau $A$ ($D_{MA} = 30$ m), không phải khoảng cách từ $A$ đến $B$ ($D_{AB} = D_{MA} + D_{MB}$).

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 63–68 (Mục 3.3.4, 3.3.5); slide bài giảng trên lớp `e7ca19ebabe62bb872f7.jpg` (Slide 130).
