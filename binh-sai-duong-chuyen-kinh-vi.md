# Bình sai đường chuyền kinh vĩ mặt bằng (Traverse adjustment)

**1. Bản chất trong một câu.**  
Bình sai đường chuyền kinh vĩ là việc phân bổ các sai số khép góc và sai số khép tọa độ của một chuỗi đa giác đo ngắm vào từng đỉnh và từng cạnh đo để đảm bảo tính khép kín hình học trên mặt bằng.

**2. Vì sao cần nó.**  
Nếu không bình sai góc và cạnh của lưới đường chuyền, đa giác đo đạc trên thực địa sẽ bị hở (đỉnh cuối không trùng điểm gốc), kéo theo bản đồ địa chính bị lệch ranh giới đất đai và tim trục các tòa nhà trong khu đô thị bị xô lệch vị trí.

**3. Nguyên lý nền.**  
- Định lý tổng các góc trong của đa giác lồi phẳng $n$ cạnh: $\sum \beta = (n - 2) \cdot 180^\circ$ (Hình học Euclid).  
- Nguyên lý truyền góc định hướng: Góc định hướng cạnh sau bằng góc định hướng cạnh trước cộng $180^\circ$ trừ góc ngoặt bên phải (Chương 4, Mục 4.1.4.3).  
- Hai bài toán trắc địa cơ bản và điều kiện ràng buộc hình học: Tổng hình chiếu các cạnh lên hệ trục tọa độ phẳng phải bằng hiệu tọa độ điểm mút (Chương 4, Mục 4.1.5).

**4. Mô hình hóa.**  
- Giả thiết: Góc ngoặt $\beta$ được đo bằng máy kinh vĩ với độ chính xác các trạm đo như nhau; chiều dài cạnh $D$ được đo độc lập; sai số ngẫu nhiên là chủ đạo.  
- Điều kiện mất hiệu lực: Đọc nhầm bàn độ góc hoặc nhầm vạch thước đo cạnh gây ra sai số thô bạo khiến sai số khép tương đối $T > 1/2000$. Trường hợp này phải kiểm tra lại hiện trường, không được phép bình sai chia đều.

**5. Suy công thức từ nguyên lý.**  

**(a) Bước 1: Bình sai góc:**  
- Sai số khép góc với đa giác khép kín $n$ đỉnh góc trong:  
  $$f_\beta = \sum \beta_{đo} - (n - 2) \cdot 180^\circ \quad (\text{Đơn vị: phút ' hoặc giây ''})$$  
- Sai số khép góc cho phép cấp kỹ thuật: $f_{\beta cp} = \pm 1' \sqrt{n}$ (hoặc $\pm 2 m_\beta \sqrt{n}$).  
- Điều kiện nghiệm thu: $|f_\beta| \le |f_{\beta cp}|$.  
- Số hiệu chỉnh phân bổ đều cho $n$ góc: $v_\beta = - \frac{f_\beta}{n}$ (Kiểm tra: $\sum v_\beta = -f_\beta$).  
- Góc sau bình sai: $\beta_i^{BS} = \beta_{đo, i} + v_\beta$.

**(b) Bước 2: Tính góc phương vị tọa độ / góc định hướng các cạnh ($\alpha$):**  
- **Theo giáo trình (trang 96–98, công thức 4.1-5 & 4.1-11)** khi góc đo $\beta$ là **góc ngoặt bên trái** theo chiều tiến:  
  $$\alpha_{sau} = \alpha_{trước} + \beta_{trái}^{BS} - 180^\circ \quad (\text{Nếu } > 360^\circ \text{ thì trừ } 360^\circ\text{; nếu } < 0^\circ \text{ thì cộng } 360^\circ)$$  
- Trường hợp đo **góc ngoặt bên phải** theo chiều tiến:  
  $$\alpha_{sau} = \alpha_{trước} + 180^\circ - \beta_{phải}^{BS} \quad (\text{hoặc } \alpha_{sau} = \alpha_{trước} - \beta_{phải}^{BS} + 180^\circ)$$

**(c) Bước 3: Tính số gia tọa độ và bình sai tọa độ:**  
- Số gia tọa độ chưa bình sai: $\Delta X_i = D_i \cdot \cos \alpha_i$; $\Delta Y_i = D_i \cdot \sin \alpha_i$.  
- Sai số khép tọa độ (với đa giác khép kín): $f_x = \sum \Delta X_i$; $f_y = \sum \Delta Y_i$.  
- Sai số khép tuyệt đối: $f_s = \sqrt{f_x^2 + f_y^2}$.  
- Sai số khép tương đối: $T = \frac{f_s}{\sum D_i}$. Đạt yêu cầu nếu $T \le \frac{1}{2000}$ (đồng bằng) hoặc $\le \frac{1}{1000}$ (vùng núi, theo trang 98 giáo trình).  
- Phân bổ số hiệu chỉnh theo chiều dài cạnh (nguyên lý Bowditch, công thức 4.1-14 trang 98):  
  $$v_{xi} = - \frac{f_x}{\sum D_i} \cdot D_i; \quad v_{yi} = - \frac{f_y}{\sum D_i} \cdot D_i$$  
- Số gia bình sai: $\Delta X_i^{BS} = \Delta X_i + v_{xi}$; $\Delta Y_i^{BS} = \Delta Y_i + v_{yi}$.

**(d) Bước 4: Tính tọa độ các đỉnh:**  
$$X_i = X_{i-1} + \Delta X_i^{BS}; \quad Y_i = Y_{i-1} + \Delta Y_i^{BS}$$

**6. Kiểm tra bằng trực giác.**  
- Nếu các góc đo tổng cộng lớn hơn lý thuyết ($f_\beta > 0$), các góc đo đang "bị phình ra", số hiệu chỉnh phải âm ($v_\beta < 0$) để thu nhỏ các góc lại.  
- Sai số khép tương đối $T = f_s / \sum D$ là một phân số có tử số là $1$ (ví dụ $1/3500$). Mẫu số càng lớn thì tuyến đo càng chính xác (mẫu số $3500 > 2000 \Rightarrow$ đạt chất lượng tốt).

**7. Bẫy khi thi.**  
- **Nhầm lẫn công thức truyền góc định hướng giữa góc bên phải và bên trái**:  
  - Góc bên trái (chuẩn giáo trình trang 96–98): $\alpha_{sau} = \alpha_{trước} + \beta_{trái} - 180^\circ$.  
  - Góc bên phải: $\alpha_{sau} = \alpha_{trước} + 180^\circ - \beta_{phải}$.  
  Dùng sai công thức sẽ làm đảo lộn toàn bộ phương hướng các cạnh tiếp theo.
- **Quên dấu âm trong số hiệu chỉnh**: Số hiệu chỉnh luôn mang dấu ngược lại với sai số khép ($v_{xi} = -f_x \cdot \dots$). Nhiều sinh viên quên dấu trừ dẫn đến nhân đôi sai số khép.
- **Lẫn lộn trục $X$ và $Y$ khi tính số gia**: Trong trắc địa, $\Delta X = D \cdot \cos \alpha$ và $\Delta Y = D \cdot \sin \alpha$. Không bấm ngược $\sin$ cho $X$ và $\cos$ cho $Y$.

**8. Liên kết.**  
- Kiến thức trước: Đo góc bằng bằng phương pháp đo góc đơn (Chương 3, Mục 3.1.4); hai bài toán trắc địa cơ bản (Chương 4, Mục 4.1.4).  
- Kiến thức sau: Lập lưới ô vuông xây dựng và bố trí các trục định vị công trình (Chương 6).

**9. Tự kiểm tra.**  
- **Bản chất**: Tại sao trong đường chuyền kinh vĩ, ta phải bình sai góc trước rồi mới tính bình sai tọa độ?  
  *Đáp*: Vì sai số góc ảnh hưởng trực tiếp đến góc định hướng của toàn bộ các cạnh phía sau theo cấp số nhân; nếu không hiệu chỉnh góc trước thì mọi số gia tọa độ $\Delta X = D \cos \alpha$ và $\Delta Y = D \sin \alpha$ đều bị sai lệch phương hướng ngay từ đầu.
- **Áp dụng**: Tuyến đường chuyền khép kín có $n = 4$ đỉnh, tổng các góc đo trong là $\sum \beta_{đo} = 360^\circ 02'$. Tính sai số khép góc $f_\beta$ và số hiệu chỉnh $v_\beta$ cho mỗi góc?  
  *Đáp*: $\sum \beta_{lt} = (4 - 2) \cdot 180^\circ = 360^\circ 00'$.  
  $f_\beta = 360^\circ 02' - 360^\circ 00' = +2' = +120''$.  
  Số hiệu chỉnh cho mỗi góc: $v_\beta = -\frac{f_\beta}{4} = -\frac{120''}{4} = -30'' = -0.5'$.
- **Bẫy**: Một tuyến đường chuyền có tổng chiều dài $\sum D = 400$ m, sai số khép $f_x = +0.12$ m, $f_y = -0.16$ m. Đánh giá sai số khép tương đối $T$ có đạt yêu cầu cấp kỹ thuật ($T \le 1/2000$) không?  
  *Đáp*: $f_s = \sqrt{0.12^2 + (-0.16)^2} = \sqrt{0.0144 + 0.0256} = \sqrt{0.04} = 0.20$ m.  
  $T = \frac{f_s}{\sum D} = \frac{0.20}{400} = \frac{1}{2000}$.  
  Vì $T = 1/2000 \le 1/2000$ nên tuyến vừa vặn ĐẠT yêu cầu kỹ thuật.

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 95–106 (Mục 4.1.5).
