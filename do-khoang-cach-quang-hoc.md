# Đo khoảng cách quang học và Thước thép (Distance measurement and Stadia tachymetry)

**1. Bản chất trong một câu.**  
Đo khoảng cách trong trắc địa là việc xác định độ dài đoạn thẳng nằm ngang nối giữa hai điểm bằng phương pháp cơ học trực tiếp (thước thép) hoặc phương pháp quang học gián tiếp (dây thị cự trên màng chỉ thập).

**2. Vì sao cần nó.**  
Góc và khoảng cách là hai thành phần cấu thành tọa độ của mọi điểm đo đạc; nếu không đo được khoảng cách ngang chính xác, ta không thể cắm ranh đất, không thể đào móng đúng kích thước bản vẽ thiết kế, và không thể tính được khối lượng đào đắp san nền.

**3. Nguyên lý nền.**  
- Tam giác đồng dạng trong hệ thống quang học ống kính: Tỉ số giữa tiêu cự kính vật và khoảng cách giữa hai chỉ thị cự trên màng dây chữ thập là một hằng số máy cố định $K = \frac{f}{p} = 100$ (Chương 3, Mục 3.2.4.1).  
- Khoảng cách nghiêng $S$ và khoảng cách ngang $D$: $D = S \cdot \cos V$ (Hệ thức lượng giác).  
- Tính chất đối xứng của màng dây chữ thập: Chỉ giữa $c_g$ nằm chính xác ở trung điểm giữa chỉ trên $c_t$ và chỉ dưới $c_d$.

**4. Mô hình hóa.**  
- Giả thiết: Mia đo được dựng thẳng đứng vuông góc với mặt đất; hệ số máy $K = 100$ chuẩn xác; hằng số cộng $C = 0$ đối với ống kính ngắm điều quang trong.  
- Điều kiện mất hiệu lực: Mia bị nghiêng so với phương thẳng đứng làm khoảng chắn trên mia $n = c_t - c_d$ bị giãn dài ra, hoặc khoảng cách đo quá xa ($D > 150$ m) làm vạch mia bị mờ nhòe không phân biệt được vạch milimét.

**5. Suy công thức từ nguyên lý.**  

**(a) Đo khoảng cách bằng dây thị cự (Mục 3.2.4, trang 59–60):**  
- Khi trục ngắm nằm ngang ($V = 0^\circ$):  
  $$D = K \cdot (c_t - c_d) = 100 \cdot (c_t - c_d)$$  
  - Trong đó: $c_t, c_d$ là số đọc chỉ trên và chỉ dưới (tính bằng m).  
  - Nếu đọc theo milimét trên mia: $n = c_t - c_d$ (mm) $\implies D = 100 \times \frac{n}{1000} = 0.1 \times n$ (m).  
- Khi trục ngắm nghiêng một góc đứng $V$:  
  $$D = K \cdot (c_t - c_d) \cdot \cos^2 V = 100 \cdot (c_t - c_d) \cdot \cos^2 V$$

**(b) Tính chất đối xứng và tái dựng số đọc bị mất (Bài tập trang 67):**  
- Điều kiện kiểm tra đọc số:  
  $$c_g = \frac{c_t + c_d}{2} \iff 2c_g - (c_t + c_d) = 0 \quad (\text{Hạn sai: } \le \pm 2\text{ mm})$$  
- Nếu mất chỉ trên $c_t$ (bị che khuất):  
  $$c_t = 2c_g - c_d \implies D = 100 \times 2 \times (c_g - c_d) = 200 \times (c_g - c_d)$$  
- Nếu mất chỉ dưới $c_d$:  
  $$c_d = 2c_g - c_t \implies D = 100 \times 2 \times (c_t - c_g) = 200 \times (c_t - c_g)$$

**(c) Đo khoảng cách trực tiếp bằng thước thép (Mục 3.2.3, trang 55–58):**  
- Chiều dài thật của đoạn thẳng đo bằng thước thép phải qua 3 số hiệu chỉnh:  
  1. Hiệu chỉnh chiều dài thực của thước (sai số dập mẫu): $\Delta l_k = \frac{D}{l_0} \cdot \Delta l$.  
  2. Hiệu chỉnh nhiệt độ: $\Delta l_t = \alpha \cdot D \cdot (t - t_0)$ (với $\alpha = 1.2 \times 10^{-5} /^\circ\text{C}$).  
  3. Hiệu chỉnh độ nghiêng mặt đất: $\Delta l_h = - \frac{h^2}{2D}$ (với $h$ là chênh cao hai đầu dốc).  
  $$D_{thật} = D_{đo} + \Delta l_k + \Delta l_t + \Delta l_h$$

**6. Kiểm tra bằng trực giác.**  
- Khoảng cách trên thực địa luôn bằng khoảng chênh lệch giữa hai chỉ nhân với $100$. Ví dụ hai chỉ chênh nhau $0.5$ m thì khoảng cách là $50$ m.  
- Chỉ giữa luôn nằm kẹp giữa chỉ trên và chỉ dưới: $c_t > c_g > c_d$.  
- Khi ngắm nghiêng dốc ($V \neq 0$), $\cos^2 V < 1$ làm khoảng cách nằm ngang $D$ luôn nhỏ hơn khoảng cách nghiêng trực tiếp.

**7. Bẫy khi thi.**  
- **Nhầm lẫn đơn vị giữa mm và m**: Lấy $(1975 - 1475) \times 100 = 50000$ m thay vì $50.0$ m. Nhớ chia 1000 để đổi mm ra mét!  
- **Quên nhân hệ số 2 khi tính khoảng cách lúc chỉ có chỉ giữa và chỉ dưới**: Nếu đề chỉ cho $c_g$ và $c_d$, cự ly phải là $200 \times (c_g - c_d)$. Nhiều bạn quên nhân $2$, lấy $(c_g - c_d) \times 100$ làm khoảng cách bị hụt mất một nửa.  
- **Quên bình phương $\cos^2 V$ khi trục ngắm nghiêng**: Công thức thị cự khi ngắm nghiêng có hệ số $\cos^2 V$, không phải $\cos V$.

**8. Liên kết.**  
- Kiến thức trước: Cấu tạo màng dây chữ thập ống kính ngắm (Chương 3, Mục 3.1.1.4).  
- Kiến thức sau: Thủy chuẩn hình học (Chương 3, Mục 3.3); đo vẽ chi tiết địa hình bằng bàn đạc / kinh vĩ (Chương 5); bố trí khoảng cách công trình (Chương 6).

**9. Tự kiểm tra.**  
- **Bản chất**: Tại sao khi trục ngắm nghiêng một góc đứng $V$, khoảng cách ngang lại tỉ lệ với $\cos^2 V$ mà không phải $\cos V$?  
  *Đáp*: Vì có hai lần ảnh hưởng của góc nghiêng: Lần 1 là do mia dựng đứng nên đoạn chắn trên mia bị kéo dài ra tỉ lệ nghịch với $\cos V$ (cần nhân $\cos V$ để đưa về đoạn chắn vuông góc tia ngắm); Lần 2 là do tia ngắm bị nghiêng nên khoảng cách nghiêng phải chiếu về phương ngang (nhân tiếp một lần $\cos V$). Tích hai lần là $\cos^2 V$.  
- **Áp dụng (trích bài tập trang 67 giáo trình)**: Đặt máy tại $A$ ngắm mia tại $N_1$, đọc được 3 chỉ: $c_t = 1975$ mm; $c_g = 1725$ mm; $c_d = 1475$ mm. Tính khoảng cách $D_{AN1}$?  
  *Đáp*: $c_t - c_d = 1975 - 1475 = 500$ mm $= 0.500$ m.  
  $D_{AN1} = 100 \times 0.500 = \mathbf{50.0\text{ m}}$.  
- **Bẫy**: Ngắm mia tại $N_2$ thấy chỉ dưới $c_d = 1995$ mm, chỉ giữa $c_g = 2265$ mm. Sinh viên A tính $D = 100 \times (2.265 - 1.995) = 27.0$ m. Đúng hay sai?  
  *Đáp*: Sai. Đó mới chỉ là nửa khoảng chắn. Chỉ trên là $c_t = 2 \times 2265 - 1995 = 2535$ mm.  
  Khoảng cách đúng là $D = 100 \times (2.535 - 1.995) = 100 \times 0.540 = \mathbf{54.0\text{ m}}$.

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 52–62 (Mục 3.2.1 đến 3.2.6), bài tập trang 67.
