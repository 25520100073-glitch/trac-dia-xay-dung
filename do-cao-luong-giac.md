# Đo cao lượng giác (Trigonometric leveling)

**1. Bản chất trong một câu.**  
Đo cao lượng giác xác định chênh cao và chiều cao vật thể thông qua giải tam giác vuông dựa trên khoảng cách nằm ngang và góc nghiêng của tia ngắm (góc đứng).

**2. Vì sao cần nó.**  
Khi địa hình quá dốc (sườn đồi, hố sâu) hoặc điểm cần đo nằm trên cao không thể dựng mia thẳng đứng (đỉnh tháp, đỉnh cột, góc mái nhà, dầm cầu), máy thủy chuẩn quang học bị mất tác dụng vì tia ngắm không thể vượt qua chướng ngại vật; chỉ có đo cao lượng giác mới giải quyết được.

**3. Nguyên lý nền.**  
- Hệ thức lượng giác trong tam giác vuông: Cạnh đối = Cạnh kề $\times \tan(\text{góc đối})$ (Toán học cơ sở).  
- Khái niệm góc đứng $V$ (vertical angle): góc hợp bởi tia ngắm nghiêng và mặt phẳng nằm ngang qua trục quay ống kính (Chương 3, Mục 3.1.1.2).  
- Chiều cao tia ngắm tại trạm đặt máy: $H_{ngắm} = H_{trạm} + i$ với $i$ là chiều cao máy (instrument height).

**4. Mô hình hóa.**  
- Giả thiết: Trục quay ống kính máy kinh vĩ/toàn đạc nằm ngang; khoảng cách ngang $D$ được đo chính xác; tia ngắm truyền thẳng trong không khí.  
- Điều kiện mất hiệu lực: Khoảng cách $D > 300$ m mà không hiệu chỉnh độ cong Trái Đất và độ khúc xạ khí quyển ($f = \frac{D^2}{2R}(1-k)$), hoặc đo khi trời nắng gắt làm tia ngắm bị khúc xạ uốn cong bất thường sát mặt đất.

**5. Suy công thức từ nguyên lý.**  
(a) **Trường hợp tổng quát (dựng được mia tại điểm đo $B$):**  
- Đặt máy tại $A$ (cao độ $H_A$, chiều cao máy $i$). Ngắm điểm trên mia tại $B$ với chiều cao ngắm $l$, góc đứng $V$, khoảng cách ngang $D$.  
- Tam giác vuông tạo bởi tia ngắm: Chênh lệch từ trục máy đến điểm ngắm là $\Delta h = D \cdot \tan V$.  
- Cao độ điểm $B$: $H_B = H_A + i + D \cdot \tan V - l$.  
- Chênh cao $h_{AB}$:  
$$h_{AB} = H_B - H_A = D \cdot \tan V + i - l \quad (\text{Đơn vị: m})$$

(b) **Trường hợp đặc biệt: Xác định chiều cao công trình không thể tới chân mia (Slide 145–146):**  
- Cần đo chiều cao đoạn $CD$ (từ chân $C$ lên đỉnh $D$). Máy đặt tại Trạm 1 cách công trình khoảng cách ngang $D$.  
- Ngắm đỉnh $D$ góc đứng $V_D$: Cao độ đỉnh $H_D = H_1 + i + D \cdot \tan V_D$.  
- Ngắm chân $C$ góc đứng $V_C$: Cao độ chân $H_C = H_1 + i + D \cdot \tan V_C$.  
- Chiều cao công trình $h_{CD} = H_D - H_C$:  
$$h_{CD} = (H_1 + i + D \cdot \tan V_D) - (H_1 + i + D \cdot \tan V_C) = D \cdot (\tan V_D - \tan V_C) \quad (\text{Đơn vị: m})$$  
*Nhận xét cốt lõi*: Đại lượng $H_1$ và $i$ triệt tiêu hoàn toàn. Chiều cao công trình độc lập với độ cao mốc và chiều cao máy!

**6. Kiểm tra bằng trực giác.**  
- Khi ngắm lên dốc ($V > 0 \Rightarrow \tan V > 0$): Điểm ngắm cao hơn máy.  
- Khi ngắm xuống dốc ($V < 0 \Rightarrow \tan V < 0$): Điểm ngắm thấp hơn máy.  
- Nếu ngắm nằm ngang ($V = 0 \Rightarrow \tan 0 = 0$): Trở về công thức đo cao hình học $h = i - l$.  
- Với chiều cao công trình $h_{CD}$: Nếu đỉnh $D$ ngắm chếch lên ($V_D > 0$) và chân $C$ ngắm chếch xuống ($V_C < 0$), thì $\tan V_D > 0$ và $\tan V_C < 0 \Rightarrow \tan V_D - \tan V_C = |\tan V_D| + |\tan V_C| > 0$, chiều cao công trình bằng tổng hai khoảng chênh lệch trên và dưới đường chân trời.

**7. Bẫy khi thi.**  
- **Dùng nhầm góc thiên đỉnh $Z$ thay vì góc đứng $V$**: Máy toàn đạc thường hiển thị góc thiên đỉnh $Z$ ($Z = 0^\circ$ ở thiên đỉnh). Nếu dùng máy có bàn độ đứng thiên đỉnh thì $V = 90^\circ - Z$ (hoặc $V = Z - 90^\circ$ tùy vị trí bàn độ). Dùng nhầm $Z$ vào hàm $\tan$ sẽ cho kết quả sai hoàn toàn.
- **Sai dấu của góc ngắm chúc xuống $V_C$**: Khi ngắm xuống, $V_C$ mang dấu âm (ví dụ $V_C = -20^\circ 30'$). Công thức có dấu trừ: $D[\tan V_D - \tan V_C] = D[\tan V_D - (- \tan |V_C|)] = D[\tan V_D + \tan |V_C|]$. Nhiều sinh viên bấm máy tính thành dấu trừ làm chiều cao công trình bị hụt đi một nửa.
- **Lúng túng khi đề bài không cho chiều cao máy $i$**: Trong bài toán đo chiều cao công trình gián tiếp, nhiều sinh viên dừng lại không làm vì đề không cho $i$. Cần nhớ rằng $i$ bị triệt tiêu khi lấy hiệu hai cao độ.

**8. Liên kết.**  
- Kiến thức trước: Cấu tạo bàn độ đứng máy kinh vĩ, kiểm nghiệm sai số chỉ tiêu $MO$ (Chương 3, Mục 3.1.3.5); đo khoảng cách bằng dây thị cự hoặc thước thép.  
- Kiến thức sau: Đo vẽ địa hình vùng đồi núi (Chương 5); kiểm tra độ thẳng đứng và độ nghiêng của cột/nhà cao tầng (Chương 6, Chương 7).

**9. Tự kiểm tra.**  
- **Bản chất**: Vì sao khi xác định chiều cao công trình từ xa bằng phương pháp đo góc đứng hai điểm đỉnh và chân, ta không cần biết chiều cao đặt máy $i$?  
  *Đáp*: Vì cả hai tia ngắm đều xuất phát từ cùng một tâm trục quay của máy (cùng cao độ tia ngắm $H_{tia} = H_1 + i$). Chiều cao công trình là hiệu cao độ giữa hai điểm ngắm, nên đại lượng $H_{tia}$ bị trừ triệt tiêu.
- **Áp dụng (ví dụ tự chọn, không phải số của đề)**: Từ trạm máy 1 cách chân công trình khoảng cách ngang $D = 35$ m, đo ngắm đỉnh $D$ có góc đứng $V_D = +15^\circ 30'$, ngắm chân $C$ có góc đứng $V_C = -20^\circ 30'$. Tính chiều cao công trình $h_{CD}$.  
  *Đáp*: $\tan(15^\circ 30') \approx 0.27732$; $\tan(-20^\circ 30') \approx -0.37388$.  
  $h_{CD} = 35 \cdot [0.27732 - (-0.37388)] = 35 \cdot (0.27732 + 0.37388) = 35 \cdot 0.65120 = 22.792$ m.
- **Bẫy**: Một sinh viên tính $h_{CD} = 35 \cdot \tan(15^\circ 30' - (-20^\circ 30')) = 35 \cdot \tan(36^\circ) \approx 25.43$ m. Kết quả này đúng hay sai?  
  *Đáp*: Hoàn toàn sai. $\tan(A) - \tan(B) \neq \tan(A - B)$. Phải tính giá trị $\tan$ của từng góc rồi mới trừ cho nhau.

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 69–70 (Mục 3.3.6); slide bài giảng trên lớp `df15d3386035e06bb924.jpg` (Slide 145), `080ffa3e4933c96d9022.jpg` (Slide 146).
