# Quan trắc lún công trình (Settlement monitoring)

**1. Bản chất trong một câu.**  
Quan trắc lún công trình là việc đo lặp lại độ cao của các mốc gắn trên kết cấu móng theo các chu kỳ thời gian định kỳ bằng phương pháp thủy chuẩn hình học độ chính xác cao nhằm theo dõi độ võng, độ nghiêng và tốc độ biến dạng của công trình.

**2. Vì sao cần nó.**  
Mọi công trình xây dựng đều lún do tải trọng nén chặt các lớp đất bên dưới; nếu không quan trắc, kỹ sư không thể phát hiện hiện tượng lún lệch (differential settlement) - nguyên nhân hàng đầu gây nứt gãy dầm cột, nghiêng nhà, kẹt thang máy và nguy cơ sập đổ công trình trong giai đoạn thi công cũng như sử dụng.

**3. Nguyên lý nền.**  
- Định luật cơ học đất về quá trình cố kết (consolidation) và biến dạng lún theo thời gian dưới áp lực tải trọng công trình (Kiến thức Cơ học đất & Nền móng).  
- Phương pháp đo thủy chuẩn hình học chính xác cao từ giữa với khoảng cách từ máy đến mia rất ngắn ($< 25$ m – 30 m) và cân bằng nghiêm ngặt khoảng cách máy – mia để triệt tiêu sai số góc $i$ (Chương 3, Mục 3.3.4).  
- Hệ thống mốc khống chế độc lập: Mốc chuẩn cơ sở (datum benchmark) chôn sâu vào tầng đất tốt không chịu ảnh hưởng của hố móng và tải trọng công trình (Chương 7, Mục 7.1).

**4. Mô hình hóa.**  
- Giả thiết: Cụm mốc chuẩn cơ sở (tối thiểu 3 mốc) hoàn toàn ổn định tuyệt đối qua các chu kỳ đo; mốc đo lún gắn chặt đồng khối với cột bê tông/tường móng của công trình.  
- Điều kiện mất hiệu lực: Mốc chuẩn bị lún do nằm quá gần hố móng sâu, hoặc đầu mốc lún bị va chạm, cong vênh bởi máy móc thi công tại hiện trường.

**5. Suy công thức từ nguyên lý.**  

**(a) Xác định độ cao mốc lún ở từng chu kỳ:**  
- Chu kỳ ban đầu (chu kỳ 0 - đo ngay khi đổ bê tông móng/sàn hầm): Xác định độ cao gốc $H_0$ của mốc quan trắc $P$.  
- Chu kỳ thứ $k$ (sau khi xây thêm các tầng hoặc theo mốc thời gian $\Delta t$): Đo thủy chuẩn từ mốc chuẩn xác định độ cao $H_k$.

**(b) Các chỉ tiêu tính toán biến dạng lún:**  
1. **Độ lún chu kỳ (Incremental settlement):**  
   $$\Delta S_k = H_k - H_{k-1} \quad (\text{Đơn vị: mm})$$  
2. **Độ lún tích lũy (Cumulative settlement):**  
   $$S_k = H_k - H_0 \quad (\text{Đơn vị: mm, quy ước dấu: lún xuống } S < 0)$$  
3. **Tốc độ lún trung bình (Settlement rate):**  
   $$v = \frac{|\Delta S_k|}{\Delta t} \quad (\text{Đơn vị: mm/ngày hoặc mm/tháng})$$  
4. **Độ lún lệch tương đối giữa hai móng lân cận $A$ và $B$ (Differential settlement ratio):**  
   $$\Delta S_{AB} = \frac{|S_A - S_B|}{L_{AB}} \quad (\text{với } L_{AB} \text{ là khoảng cách tim cột } A-B)$$

**(c) Tiêu chuẩn ổn định lún:**  
Công trình được coi là ổn định lún nếu tốc độ lún suy giảm dần và không vượt quá $0.01$ mm/ngày (đối với đất cát) hoặc $0.04$ mm/ngày (đối với đất sét) theo tiêu chuẩn TCVN 9360:2012.

**6. Kiểm tra bằng trực giác.**  
- Tải trọng thi công tăng lên (xây thêm tầng): Độ lún tích lũy $S_k$ phải tăng dần theo thời gian.  
- Sau khi cất nóc và đưa vào sử dụng: Tốc độ lún $v$ phải giảm dần tiệm cận về 0 (đường cong cố kết đất tắt dần). Nếu tốc độ lún tăng đột ngột, đất nền đang bị phá hoại trượt hoặc có sự cố rò rỉ nước ngầm xói mòn.  
- Nếu $S_A \approx S_B$: Công trình lún đều, kết cấu an toàn. Nếu $S_A \gg S_B$: Công trình bị lún lệch, gây biến dạng uốn trong khung nhà.

**7. Bẫy khi thi.**  
- **Nhầm lẫn giữa độ lún chu kỳ $\Delta S_k$ và độ lún tích lũy $S_k$**: Độ lún chu kỳ so với chu kỳ liền trước ($H_k - H_{k-1}$); độ lún tích lũy luôn so với chu kỳ ban đầu móng vừa hoàn thành ($H_k - H_0$).
- **Không kiểm tra độ ổn định của mốc chuẩn cơ sở**: Tin tưởng tuyệt đối vào 1 mốc chuẩn duy nhất. Trong quy chuẩn bắt buộc phải đo khép giữa ít nhất 3 mốc chuẩn cơ sở ở mỗi chu kỳ để kiểm tra xem mốc chuẩn có bị lún theo công trình hay không.
- **Dùng sai loại máy thủy chuẩn**: Trong quan trắc lún công trình đòi hỏi cấp chính xác sub-millimeter (sai số $\le \pm 0.5$ mm/trạm), phải dùng máy thủy chuẩn chính xác cao có bộ đo cực nhỏ (micrometer) và mia Invar (hợp kim không giãn nở nhiệt); không được dùng máy thủy chuẩn kỹ thuật thông thường với mia nhôm rút.

**8. Liên kết.**  
- Kiến thức trước: Thủy chuẩn hình học (Chương 3); đánh giá sai số ngẫu nhiên chuỗi đo (Chương 2); bình sai tuyến đo cao (Chương 4).  
- Kiến thức sau: Đối chiếu với tính toán lún theo lý thuyết cơ học đất; đánh giá an toàn chịu lực của kết cấu bê tông cốt thép trong môn Thi công và Giám sát công trình.

**9. Tự kiểm tra.**  
- **Bản chất**: Vì sao mốc chuẩn cơ sở dùng trong quan trắc lún phải đặt ngoài phạm vi vùng ảnh hưởng của hố móng công trình (thường cách xa $> 30 - 50$ m)?  
  *Đáp*: Vì tải trọng khổng lồ của tòa nhà gây ra vùng ứng suất nén lan truyền trong lòng đất (củ áp lực). Nếu đặt mốc chuẩn bên trong vùng này, mốc chuẩn cũng bị lún xuống theo công trình, làm sai lệch kết quả đo (đo ra độ lún nhỏ hơn thực tế).
- **Áp dụng**: Mốc lún tại chân cột có độ cao chu kỳ ban đầu $H_0 = 15.3452$ m. Ở chu kỳ 3 (xong sàn tầng 5), độ cao đo được là $H_3 = 15.3312$ m. Ở chu kỳ 4 (xong sàn tầng 10 sau đó 30 ngày), độ cao là $H_4 = 15.3222$ m. Tính độ lún tích lũy đến chu kỳ 4 và tốc độ lún giữa chu kỳ 3 và 4?  
  *Đáp*:  
  - Độ lún tích lũy: $S_4 = H_4 - H_0 = 15.3222 - 15.3452 = -0.0230\text{ m} = -23.0$ mm (lún $23.0$ mm).  
  - Độ lún chu kỳ 3–4: $\Delta S = H_4 - H_3 = 15.3222 - 15.3312 = -0.0090\text{ m} = -9.0$ mm.  
  - Tốc độ lún: $v = \frac{9.0\text{ mm}}{30\text{ ngày}} = 0.30$ mm/ngày.
- **Bẫy**: Hai cột kề nhau cách nhau $L = 6.0$ m có độ lún tích lũy lần lượt là $S_A = 20$ mm và $S_B = 35$ mm. Độ lún lệch tương đối giữa hai cột bằng bao nhiêu và có ý nghĩa gì?  
  *Đáp*: $\Delta S_{AB} = \frac{|35 - 20|\text{ mm}}{6000\text{ mm}} = \frac{15}{6000} = \frac{1}{400} = 0.0025$.  
  Độ lún lệch này phản ánh góc xoay của dầm nối giữa hai cột. Nếu vượt quá giới hạn cho phép (thường là $1/500$), dầm sẽ xuất hiện vết nứt xiên do biến dạng trượt và mô men uốn thứ cấp.

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 144–156 (Chương 7).
