# Máy kinh vĩ và Phương pháp đo góc (Theodolite and angle measurement)

**1. Bản chất trong một câu.**  
Đo góc trong trắc địa là việc chiếu các hướng ngắm thực địa lên một hình tròn chia độ nằm ngang (đo góc bằng) hoặc mặt phẳng thẳng đứng (đo góc đứng) thông qua hệ trục quay quang học của máy kinh vĩ.

**2. Vì sao cần nó.**  
Mọi công trình xây dựng (nhà cao tầng, cầu, đường giao thông) đều được khống chế bởi các góc ngoặt và phương hướng; nếu không có máy kinh vĩ để định vị góc bằng và góc đứng, các trục định vị cột, tim tường sẽ bị vẹo lệch, và độ thẳng đứng của nhà cao tầng sẽ bị nghiêng đổ.

**3. Nguyên lý nền.**  
- Khái niệm góc bằng $\beta$ (horizontal angle): Là góc phẳng nhị diện tạo bởi hai mặt phẳng thẳng đứng đi qua hai hướng ngắm từ trạm máy đến hai mục tiêu (Chương 3, Mục 3.1.1.1).  
- Khái niệm góc đứng $V$ (vertical angle): Là góc nghiêng giữa trục ngắm quang học và mặt phẳng nằm ngang (Chương 3, Mục 3.1.1.2).  
- Hệ thống 4 trục hình học cơ bản của máy kinh vĩ quang cơ (Chương 3, Mục 3.1.1.4):  
  - $VV_1$: Trục quay đứng của thân máy.  
  - $LL_1$: Trục ống thủy dài của bàn độ ngang.  
  - $HH_1$: Trục quay ngang của ống kính ngắm.  
  - $CC_1$: Trục ngắm quang học (nối quang tâm kính vật và giao điểm màng dây chữ thập).

**4. Mô hình hóa.**  
- Giả thiết: Trục quay đứng $VV_1$ hoàn toàn trùng với phương dây dọi; các trục quang học chuyển động quay không có ma sát cơ học; bàn độ được chia vạch chính xác.  
- Điều kiện mất hiệu lực: Các trục hình học bị va đập làm lệch góc (xuất hiện sai số góc ngắm $2c$, sai số trục quay $i$, hoặc sai số chỉ tiêu $MO$), hoặc đặt máy trên nền đất yếu/gió lớn làm rung lắc bọt thủy.

**5. Suy công thức từ nguyên lý.**  

**(a) 4 điều kiện hình học & kiểm nghiệm máy kinh vĩ (Mục 3.1.3, trang 43–46):**  
1. **$LL_1 \perp VV_1$**: Trục ống thủy dài vuông góc trục đứng máy.  
   - Kiểm nghiệm: Cân bọt thủy vào giữa, quay máy $180^\circ$. Nếu bọt thủy vẫn ở giữa là đạt; nếu lệch thì chỉnh ốc cân bọt thủy một nửa, ốc chân máy một nửa.  
2. **$CC_1 \perp HH_1$**: Trục ngắm vuông góc trục quay ống kính.  
   - Nếu không vuông góc sinh ra **sai số ngắm (sai số $2c$)**.  
   - Kiểm nghiệm: Ngắm điểm $M$ ở hai vị trí bàn độ Thuận kính ($L$) và Đảo kính ($R$).  
     $$2c = |L - (R \pm 180^\circ)|$$  
   - **Biện pháp triệt tiêu**: Đo ở 2 vị trí bàn độ $L$ và $R$ rồi lấy trung bình: $\beta = \frac{\beta_L + \beta_R}{2}$. Khi đảo kính, sai số $2c$ đổi dấu nên tự triệt tiêu 100%.  
3. **$HH_1 \perp VV_1$**: Trục quay ống kính vuông góc trục đứng máy. Khi ống kính quay thì trục ngắm vạch ra một mặt phẳng thẳng đứng.  
4. **Dây đứng màng dây chữ thập phải song song trục đứng $VV_1$**.

**(b) Đo góc bằng phương pháp đơn giản (ngắm 2 hướng $A$ và $B$):**  
- Nửa lần đo thuận kính (L): $\beta_L = b_L - a_L$ (số đọc hướng phải trừ hướng trái).  
- Nửa lần đo đảo kính (R): $\beta_R = b_R - a_R$.  
- Kiểm tra sai số: $|\beta_L - \beta_R| \le 2c_{cp}$ (thường $\le 45''$).  
- Trị số 1 lần đo: $\beta = \frac{\beta_L + \beta_R}{2}$.

**(c) Đo góc đứng và sai số chỉ tiêu $MO$ (Index error):**  
- Sai số chỉ tiêu $MO$: Là số đọc trên bàn độ đứng khi trục ngắm nằm ngang chuẩn.  
  $$MO = \frac{L + R - 360^\circ}{2} \quad (\text{hoặc } \frac{L + R - 180^\circ}{2} \text{ tùy loại máy})$$  
- Góc đứng $V$:  
  $$V = L - MO = MO - R + 180^\circ$$  
- Lấy trung bình hai vị trí bàn độ triệt tiêu hoàn toàn sai số $MO$.

**6. Kiểm tra bằng trực giác.**  
- Góc bằng luôn là hiệu giữa hướng bên phải và hướng bên trái ($\beta = b - a$). Nếu $b < a$ thì cộng thêm $360^\circ$ vào $b$ trước khi trừ.  
- Góc đứng: Ngắm lên thì $V > 0$, ngắm xuống thì $V < 0$.  
- Khi đảo kính $180^\circ$, ống kính bị lật ngược từ dưới lên trên và bàn độ quay nửa vòng tròn, do đó các sai số lệch góc đối xứng tự động bù trừ lẫn nhau.

**7. Bẫy khi thi.**  
- **Nhầm lẫn số đọc hướng và góc bằng**: Các số đọc trên bàn độ ($a, b$) chỉ là hướng ngắm. Góc bằng là hiệu số giữa hai hướng: $\beta = b - a$.  
- **Quên cộng $360^\circ$ khi số đọc hướng bên phải nhỏ hơn hướng bên trái**: Ví dụ hướng $A$ là $350^\circ$, hướng $B$ là $20^\circ \implies \beta = (20^\circ + 360^\circ) - 350^\circ = 30^\circ$.  
- **Nhầm dấu của sai số chỉ tiêu $MO$**: Phải nhớ $V = L - MO$, nếu $MO$ mang dấu âm thì trừ cho âm thành cộng.

**8. Liên kết.**  
- Kiến thức trước: Khái niệm góc phương vị, góc định hướng (Chương 1).  
- Kiến thức sau: Đo cao lượng giác (Chương 3, Mục 3.3.6); bình sai góc đường chuyền kinh vĩ (Chương 4, Mục 4.1.5); bố trí góc thiết kế công trình (Chương 6).

**9. Tự kiểm tra.**  
- **Bản chất**: Vì sao khi đo góc bằng máy kinh vĩ, người ta bắt buộc phải đo ở cả hai vị trí bàn độ Thuận kính (L) và Đảo kính (R)?  
  *Đáp*: Vì thao tác đảo kính và quay thân máy $180^\circ$ làm cho sai số trục ngắm $2c$ và sai số độ nghiêng trục quay $HH_1$ đổi dấu ngược lại. Khi lấy trung bình cộng của hai nửa lần đo, các sai số hệ thống hình học này sẽ tự động triệt tiêu lẫn nhau hoàn toàn.  
- **Áp dụng**: Tại trạm máy $O$, ngắm hướng $A$ có số đọc $L_A = 0^\circ 12' 30''$, $R_A = 180^\circ 12' 00''$. Ngắm hướng $B$ có $L_B = 45^\circ 36' 40''$, $R_B = 225^\circ 36' 20''$. Tính góc bằng $\beta$?  
  *Đáp*: $\beta_L = 45^\circ 36' 40'' - 0^\circ 12' 30'' = 45^\circ 24' 10''$.  
  $\beta_R = 225^\circ 36' 20'' - 180^\circ 12' 00'' = 45^\circ 24' 20''$.  
  Trị số góc bằng: $\beta = \frac{\beta_L + \beta_R}{2} = 45^\circ 24' 15''$.  
- **Bẫy**: Đo góc đứng một mục tiêu được $L = 105^\circ 20' 00''$ và $R = 254^\circ 40' 00''$. Tính sai số $MO$ và góc đứng $V$?  
  *Đáp*: Giả sử máy có thang độ $0^\circ \div 360^\circ$ với điều kiện $L + R = 360^\circ$:  
  $MO = \frac{105^\circ 20' + 254^\circ 40' - 360^\circ}{2} = \frac{360^\circ 00' - 360^\circ}{2} = 0^\circ 00'$.  
  $V = 105^\circ 20' - 90^\circ = +15^\circ 20'$ (hoặc tùy cấu tạo thang độ của máy).

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 37–51 (Mục 3.1.1 đến 3.1.6).
