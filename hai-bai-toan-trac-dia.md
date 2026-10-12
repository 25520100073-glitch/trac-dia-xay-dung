# Hai bài toán trắc địa cơ bản (Forward and inverse geodetic problems)

**1. Bản chất trong một câu.**  
Hai bài toán trắc địa cơ bản là cầu nối chuyển đổi hai chiều giữa hệ tọa độ phẳng Decartes $(X, Y)$ và các đại lượng đo phân cực ngoài thực địa gồm khoảng cách ngang $S$ và góc định hướng $\alpha$.

**2. Vì sao cần nó.**  
Mọi bản vẽ thiết kế công trình đều sử dụng tọa độ phẳng $(X, Y)$, nhưng máy đo đạc ngoài công trường chỉ đo được góc và khoảng cách; nếu không giải được hai bài toán này, kỹ sư không thể tính tọa độ các điểm đo để vẽ bản đồ (bài toán thuận) và không thể đưa bản vẽ ra thực địa để đào móng, ép cọc (bài toán nghịch).

**3. Nguyên lý nền.**  
- Hệ tọa độ trắc địa phẳng vuông góc: Trục $X$ hướng về phía Bắc địa lý (thẳng đứng), trục $Y$ hướng về phía Đông (nằm ngang), góc quay theo chiều kim đồng hồ từ $0^\circ$ đến $360^\circ$ (khác với hệ trục toán học Descartes) (Chương 1, Mục 1.2).  
- Khái niệm góc định hướng (grid azimuth / bearing) $\alpha_{AB}$: Góc bằng tính từ hướng Bắc của trục tọa độ $X$ theo chiều kim đồng hồ đến hướng đoạn thẳng $AB$ (Chương 1, Mục 1.3).  
- Định lý Pythagoras và các hàm lượng giác lượng giác cơ bản trong tam giác vuông.

**4. Mô hình hóa.**  
- Giả thiết: Trái Đất được coi là mặt phẳng trong phạm vi công trình ($R < 10$ km); hình chiếu các đoạn thẳng lên mặt phẳng ngang không đổi.  
- Điều kiện mất hiệu lực: Tuyến đo trải dài hàng trăm kilômét trên mặt cầu mà không xét đến độ tụ kinh tuyến và độ biến dạng chiếu của phép chiếu Gauss-Krüger/UTM.

**5. Suy công thức từ nguyên lý.**  

**(a) Bài toán thuận (Forward problem):**  
- Cho trước: Tọa độ điểm $A(X_A, Y_A)$, chiều dài cạnh $S_{AB}$, góc định hướng $\alpha_{AB}$.  
- Tìm: Tọa độ điểm $B(X_B, Y_B)$.  
- Các bước:  
  1. Tính số gia tọa độ (coordinate increments):  
     $$\Delta X_{AB} = S_{AB} \cdot \cos \alpha_{AB}$$  
     $$\Delta Y_{AB} = S_{AB} \cdot \sin \alpha_{AB}$$  
  2. Tính tọa độ điểm $B$:  
     $$X_B = X_A + \Delta X_{AB}$$  
     $$Y_B = Y_A + \Delta Y_{AB}$$

**(b) Bài toán nghịch (Inverse problem):**  
- Cho trước: Tọa độ hai điểm $A(X_A, Y_A)$ và $B(X_B, Y_B)$.  
- Tìm: Chiều dài cạnh $S_{AB}$ và góc định hướng $\alpha_{AB}$.  
- Các bước:  
  1. Tính hiệu số tọa độ: $\Delta X = X_B - X_A$; $\Delta Y = Y_B - Y_A$.  
  2. Tính chiều dài cạnh:  
     $$S_{AB} = \sqrt{\Delta X^2 + \Delta Y^2}$$  
  3. Tính góc phương vị phụ (góc phụ) $r$:  
     $$\tan r = \left| \frac{\Delta Y}{\Delta X} \right| \Rightarrow r = \arctan \left| \frac{\Delta Y}{\Delta X} \right| \quad (0^\circ \le r \le 90^\circ)$$  
  4. Chuyển từ góc phụ $r$ sang góc định hướng $\alpha_{AB}$ theo 4 góc phần tư:  
     - Góc phần tư I ($\Delta X > 0, \Delta Y > 0$): $\alpha_{AB} = r$  
     - Góc phần tư II ($\Delta X < 0, \Delta Y > 0$): $\alpha_{AB} = 180^\circ - r$  
     - Góc phần tư III ($\Delta X < 0, \Delta Y < 0$): $\alpha_{AB} = 180^\circ + r$  
     - Góc phần tư IV ($\Delta X > 0, \Delta Y < 0$): $\alpha_{AB} = 360^\circ - r$

**6. Kiểm tra bằng trực giác.**  
- Trong hệ trắc địa, trục $X$ là trục tung (Bắc) và trục $Y$ là trục hoành (Đông). Do đó, hình chiếu lên trục $X$ đi liền với hàm $\cos$ ($\Delta X = S \cos \alpha$) và lên trục $Y$ đi liền với hàm $\sin$ ($\Delta Y = S \sin \alpha$).  
- Khi $\alpha = 0^\circ$ (hướng thẳng Bắc): $\cos 0^\circ = 1, \sin 0^\circ = 0 \Rightarrow \Delta X = S, \Delta Y = 0$ (hoàn toàn trực quan).  
- Khi $\alpha = 90^\circ$ (hướng thẳng Đông): $\Delta X = 0, \Delta Y = S$.

**7. Bẫy khi thi.**  
- **Nhầm lẫn giữa hệ trục Trắc địa và Toán học**: Trong toán học, $\Delta X = S \cos \varphi$ và $\Delta Y = S \sin \varphi$ với góc $\varphi$ tính từ trục hoành ngược chiều kim đồng hồ. Trong trắc địa, góc $\alpha$ tính từ trục $X$ (trục đứng) cùng chiều kim đồng hồ, nên $\Delta X$ ăn theo $\cos \alpha$ và $\Delta Y$ ăn theo $\sin \alpha$. Sinh viên thường hay gán ngược $\sin/\cos$.
- **Xác định sai góc phần tư khi giải bài toán nghịch**: Máy tính bỏ túi luôn trả về hàm $\arctan$ trong khoảng $(-90^\circ, +90^\circ)$. Nếu không xét dấu của $\Delta X$ và $\Delta Y$ để chuyển về góc định hướng $\alpha$, góc tính ra sẽ bị sai lệch $180^\circ$ (ngược hướng hoàn toàn).
- **Lấy ngược điểm đầu và điểm cuối**: Tính $\Delta X = X_A - X_B$ thay vì $X_B - X_A$. Quy tắc bất di bất dịch: Số gia luôn bằng **Cuối trừ Đầu**.

**8. Liên kết.**  
- Kiến thức trước: Hệ tọa độ phẳng và góc phương vị trong trắc địa (Chương 1).  
- Kiến thức sau: Tính chuyền góc định hướng và bình sai tọa độ đường chuyền kinh vĩ (Chương 4); tính góc cực và khoảng cách để bố trí điểm móng công trình ra thực địa (Chương 6).

**9. Tự kiểm tra.**  
- **Bản chất**: Điểm khác biệt mấu chốt giữa quy ước góc trong trắc địa và quy ước góc trong giải tích toán học phẳng là gì?  
  *Đáp*: Trong trắc địa, trục gốc là trục Bắc $X$ (thẳng đứng) và chiều quay dương là cùng chiều kim đồng hồ; trong toán học, trục gốc là trục hoành $X$ (nằm ngang) và chiều quay dương là ngược chiều kim đồng hồ.
- **Áp dụng**: Cho điểm $A(100.00\text{ m}, 200.00\text{ m})$, chiều dài $S_{AB} = 50.00$ m, góc định hướng $\alpha_{AB} = 120^\circ 00'$. Tính tọa độ điểm $B$.  
  *Đáp*: $\Delta X_{AB} = 50 \cdot \cos(120^\circ) = 50 \cdot (-0.5) = -25.00$ m.  
  $\Delta Y_{AB} = 50 \cdot \sin(120^\circ) = 50 \cdot (0.8660) = +43.30$ m.  
  $X_B = 100.00 - 25.00 = 75.00$ m; $Y_B = 200.00 + 43.30 = 243.30$ m.
- **Bẫy**: Cho $A(50, 80)$ và $B(20, 50)$ (đơn vị m). Tính góc định hướng $\alpha_{AB}$.  
  *Đáp*: $\Delta X = 20 - 50 = -30$ m; $\Delta Y = 50 - 80 = -30$ m.  
  Vì $\Delta X < 0, \Delta Y < 0 \Rightarrow$ thuộc góc phần tư III.  
  $\tan r = |-30 / -30| = 1 \Rightarrow r = 45^\circ$.  
  $\alpha_{AB} = 180^\circ + r = 180^\circ + 45^\circ = 225^\circ 00'$. (Nếu bấm máy tính $\arctan(1) = 45^\circ$ mà không cộng $180^\circ$ thì sai).

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 93–94 (Mục 4.1.4.1, 4.1.4.2).
