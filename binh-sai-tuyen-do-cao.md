# Bình sai đường chuyền độ cao (Leveling network adjustment)

**1. Bản chất trong một câu.**  
Bình sai đường chuyền độ cao là quy trình triệt tiêu mâu thuẫn hình học (sai số khép) bằng cách phân bổ lượng sai lệch ngược dấu vào từng đoạn đo tỉ lệ thuận với chiều dài hoặc số trạm máy.

**2. Vì sao cần nó.**  
Trong thực tế đo đạc luôn có sai số ngẫu nhiên tích lũy; nếu không bình sai, khi tính độ cao từ mốc đầu đến mốc cuối sẽ không bao giờ khớp với giá trị gốc đã biết, tạo ra sự mâu thuẫn cao độ nghiêm trọng giữa các hạng mục công trình liền kề.

**3. Nguyên lý nền.**  
- Điều kiện ràng buộc hình học tuyến phù hợp: Tổng chênh cao thực tế giữa hai mốc gốc phải bằng hiệu cao độ gốc: $\sum h_{lý\_thuyết} = H_{cuối} - H_{đầu}$ (Chương 4, Mục 4.2.2.1).  
- Nguyên lý số bình phương nhỏ nhất Gauss: Phân bổ số hiệu chỉnh tỉ lệ nghịch với trọng số đo (tức tỉ lệ thuận với chiều dài cạnh $D_i$ hoặc số trạm đo $n_i$) (Chương 2, Mục 2.4).  
- Bảo toàn tổng số hiệu chỉnh: $\sum v_{hi} = -f_h$.

**4. Mô hình hóa.**  
- Giả thiết: Sai số khép $f_h$ hoàn toàn là sai số ngẫu nhiên (đã kiểm tra thỏa mãn điều kiện giới hạn $|f_h| \le |f_{hcp}|$).  
- Điều kiện mất hiệu lực: Tuyến đo bị sai số thô bạo (đọc nhầm số mét, ghi nhầm dấu) hoặc mốc gốc bị lún/chuyển dịch làm $|f_h| > |f_{hcp}|$. Khi đó nghiêm cấm bình sai, bắt buộc phải đo lại ngoài thực địa.

**5. Suy công thức từ nguyên lý.**  
Quy trình 3 bước chuẩn mực (Slide 197):

**(a) Bước 1: Tính sai số khép độ cao $f_h$ và so sánh giới hạn:**  
- Với đường chuyền độ cao phù hợp (nối mốc đầu $A$ sang mốc cuối $B$):  
  $$f_h = \sum h_{đo} - (H_{cuối} - H_{đầu}) \quad (\text{Đơn vị: m hoặc mm})$$  
- Với đường chuyền khép kín (đi từ $A$ rồi quay về lại $A$):  
  $$f_h = \sum h_{đo} \quad (\text{vì } H_{cuối} = H_{đầu})$$  
- Tiêu chuẩn cho phép đối với lưới độ cao kỹ thuật (Slide 196). Nếu đề đã cho $f_{hcp}$ thì dùng đúng số đề cho, ví dụ bài tập trang 67 cho $\pm 100$ mm:  
  $$f_{hcp} = \pm 50\sqrt{L} \text{ (mm, với } L = \sum D_i \text{ tính bằng km)}$$  
  $$\text{hoặc } f_{hcp} = \pm 10\sqrt{N} \text{ (mm, với } N = \sum n_i \text{ là tổng số trạm đo)}$$  
- Điều kiện nghiệm thu: $|f_h| \le |f_{hcp}|$ (ĐẠT).

**(b) Bước 2: Tính số hiệu chỉnh $v_{hi}$ và chênh cao bình sai $h_i^{BS}$:**  
- Số hiệu chỉnh phân bổ ngược dấu với sai số khép:  
  - Theo chiều dài cạnh: $v_{hi} = - \frac{f_h}{\sum D_i} \cdot D_i$  
  - Theo số trạm máy: $v_{hi} = - \frac{f_h}{N} \cdot n_i$  
- Kiểm tra bắt buộc: $\sum v_{hi} = -f_h$.  
- Chênh cao sau bình sai:  
  $$h_i^{BS} = h_{đo, i} + v_{hi} \quad (\text{Kiểm tra: } \sum h_i^{BS} = H_{cuối} - H_{đầu})$$

**(c) Bước 3: Tính độ cao bình sai các điểm trong tuyến:**  
- Tính truyền từ mốc đầu:  
  $$H_i = H_{i-1} + h_i^{BS} \quad (\text{với } H_0 = H_{đầu})$$  
- Kiểm tra điểm cuối cùng: Điểm tính cuối cùng bắt buộc phải trùng khít tuyệt đối với $H_{cuối}$.

**6. Kiểm tra bằng trực giác.**  
- Đoạn đường càng dài (nhiều trạm máy hơn) thì nguy cơ tích lũy sai số càng lớn $\Rightarrow$ nhận số hiệu chỉnh $v_{hi}$ có độ lớn lớn hơn.  
- Nếu đo tổng thể bị "dư" chênh cao ($f_h > 0$) thì số hiệu chỉnh phải mang dấu âm ($v_{hi} < 0$) để kéo tổng chênh cao tụt xuống cho khớp với mốc chuẩn.  
- Ngược lại, nếu đo bị "thiếu" ($f_h < 0$) thì số hiệu chỉnh phải mang dấu dương ($v_{hi} > 0$).

**7. Bẫy khi thi.**  
- **Nhầm lẫn mốc đầu và mốc cuối**: Lấy $(H_{đầu} - H_{cuối})$ thay vì $(H_{cuối} - H_{đầu})$. Khi đó dấu của $f_h$ bị đảo ngược, dẫn đến cộng thêm sai số thay vì triệt tiêu sai số.
- **Quên đổi đơn vị chiều dài $L$ khi tính $f_{hcp}$**: Công thức $f_{hcp} = \pm 50\sqrt{L}$ yêu cầu $L$ tính bằng **km**, kết quả cho ra **mm**. Ví dụ tổng tuyến dài $520$ m thì $L = 0.520$ km, $f_{hcp} = \pm 50\sqrt{0.520} \approx \pm 36$ mm. Nếu thay nguyên số $520$ vào căn sẽ ra $1140$ mm (sai lệch nghiêm trọng).
- **Làm tròn số hiệu chỉnh gây lệch tổng**: Sau khi làm tròn milimét, nếu $\sum v_{hi} \neq -f_h$, phải cộng hoặc trừ $1$ mm vào đoạn có chiều dài lớn nhất để đảm bảo tổng số hiệu chỉnh triệt tiêu hoàn toàn sai số khép.

**8. Liên kết.**  
- Kiến thức trước: Đo thủy chuẩn trạm máy đơn lẻ (Chương 3); lý thuyết sai số và nguyên lý bình sai trực tiếp Bessel (Chương 2).  
- Kiến thức sau: Bình sai lưới tam giác và đường chuyền kinh vĩ tọa độ $(X, Y)$ (Chương 4); bình sai lưới quan trắc lún nhiều chu kỳ (Chương 7).

**9. Tự kiểm tra.**  
- **Bản chất**: Tại sao khi bình sai, số hiệu chỉnh $v_{hi}$ luôn mang dấu ngược lại với sai số khép $f_h$?  
  *Đáp*: Vì sai số khép thể hiện lượng chênh lệch thừa (nếu dương) hoặc thiếu (nếu âm) của kết quả đo so với giá trị thực tế. Muốn đưa kết quả đo về đúng giá trị chuẩn, ta phải trừ bớt lượng thừa hoặc bù vào lượng thiếu, do đó $v_{hi} = -f_h \cdot \frac{D_i}{\sum D_i}$.
- **Áp dụng (trích bảng tính Slide 198)**: Tuyến đo gồm 6 đoạn nối từ mốc $A$ ($H_A = 55.216$ m) đến mốc $B$ ($H_B = 50.000$ m). Tổng chiều dài $L = 520$ m. Tổng chênh cao đo $\sum h_{đo} = -5.192$ m. Tính $f_h$ và đánh giá độ chính xác?  
  *Đáp*: $H_{cuối} - H_{đầu} = 50.000 - 55.216 = -5.216$ m.  
  $f_h = \sum h_{đo} - (H_{cuối} - H_{đầu}) = -5.192 - (-5.216) = +0.024\text{ m} = +24\text{ mm}$.  
  $f_{hcp} = \pm 50\sqrt{0.520} \approx \pm 36.05$ mm. Vì $|+24| \le 36.05$ mm nên tuyến đo ĐẠT yêu cầu.
- **Bẫy (trích bài tập trang 67 giáo trình)**: Đặt máy tại điểm $A$, ngắm mia tại hai mốc gốc $N_1$ và $N_2$ thu được $h_{AN1} = -0.225$ m và $h_{AN2} = -0.765$ m. Khi lập tuyến tính từ $N_1 \rightarrow A \rightarrow N_2$, chênh cao đoạn đầu $h_{N1A}$ bằng bao nhiêu?  
  *Đáp*: $h_{N1A} = -h_{AN1} = -(-0.225) = +0.225$ m. Nếu lấy nguyên giá trị $-0.225$ m thì sai vì chiều tuyến đo là từ $N_1$ đến $A$.

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 67, 108–113 (Mục 4.2.1, 4.2.2); slide bài giảng trên lớp `2f9972b2c1bf41e118ae.jpg` (Slide 197), `17d072edc1e041be18f1.jpg` (Slide 198), `0a5b7c7ccf714f2f1660.jpg` (Slide 199), `08483a76897b0925506a.jpg` (Slide 201).
