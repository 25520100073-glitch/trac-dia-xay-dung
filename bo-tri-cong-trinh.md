# Bố trí công trình ra thực địa (Setting out / Construction staking)

**1. Bản chất trong một câu.**  
Bố trí công trình là quá trình hình học ngược với đo vẽ: chuyển tọa độ và cao độ từ bản vẽ thiết kế ra cắm mốc chuẩn xác trên mặt đất để định vị tim trục, móng cọc và kết cấu thi công.

**2. Vì sao cần nó.**  
Bản vẽ thiết kế dù hoàn hảo đến đâu cũng chỉ nằm trên giấy; nếu không có phương pháp bố trí trắc địa chuẩn xác, công trình sẽ bị xây lệch tim trục, vi phạm ranh chỉ giới xây dựng, và cao độ đáy móng bị đào quá sâu hoặc quá nông gây lãng phí và mất an toàn kết cấu.

**3. Nguyên lý nền.**  
- Bài toán trắc địa nghịch: Từ tọa độ mốc khống chế và tọa độ điểm thiết kế suy ra góc cực $\beta$ và khoảng cách ngang $S$ cần bố trí (Chương 4, Mục 4.1.4.2).  
- Nguyên lý cao độ tia ngắm (instrument collimation height): $H_{tia} = H_{gốc} + a$ (Chương 3, Mục 3.3.4).  
- Nguyên lý triệt tiêu sai số dụng cụ bằng hai vị trí bàn độ (thuận kính và đảo kính) của máy kinh vĩ (Chương 3, Mục 3.1.3).

**4. Mô hình hóa.**  
- Giả thiết: Các mốc khống chế mặt bằng và độ cao thi công ổn định, không bị chấn động bởi xe lu và máy đóng cọc; thước thép/máy đo khoảng cách đã hiệu chuẩn độ dài.  
- Điều kiện mất hiệu lực: Sử dụng mốc giả định không liên kết với hệ tọa độ công trình, hoặc bố trí độ cao khi trời mưa làm lún chân máy thủy chuẩn.

**5. Suy công thức từ nguyên lý.**  

**(a) Bố trí độ cao thiết kế $H_{tk}$ bằng máy thủy chuẩn (Phương pháp cao độ tia ngắm):**  
- Đặt máy thủy chuẩn tại vị trí thuận lợi, dựng mia tại mốc chuẩn độ cao $A$ (đã biết $H_A$), đọc chỉ giữa là $a$.  
- Cao độ tia ngắm nằm ngang của máy:  
  $$H_{tia} = H_A + a \quad (\text{Đơn vị: m})$$  
- Cần cắm mốc cao độ thiết kế $H_{tk}$ tại vị trí cọc $B$. Số đọc thiết kế $b_{tk}$ phải đọc được trên mia dựng tại $B$ là:  
  $$b_{tk} = H_{tia} - H_{tk} = (H_A + a) - H_{tk} \quad (\text{Đơn vị: m hoặc mm})$$  
- Nâng hoặc hạ mia (hoặc đóng cọc lún xuống) cho đến khi chỉ ngang giữa của máy cắt đúng vạch $b_{tk}$, sau đó vạch mực đỏ đánh dấu cốt thiết kế lên cọc/cột.

**(b) Bố trí điểm mặt bằng bằng phương pháp tọa độ cực:**  
- Cho mốc gốc $A(X_A, Y_A)$, hướng chuẩn $AB$ (góc định hướng $\alpha_{AB}$), cần bố trí điểm thiết kế $P(X_P, Y_P)$.  
- Dùng bài toán nghịch tính khoảng cách $S_{AP} = \sqrt{(X_P - X_A)^2 + (Y_P - Y_A)^2}$ và góc định hướng $\alpha_{AP}$.  
- Góc quay cực cần đặt trên máy kinh vĩ tại $A$:  
  $$\beta_{tk} = \alpha_{AP} - \alpha_{AB}$$  
- Đặt máy tại $A$, định hướng về $B$, quay góc $\beta_{tk}$, đo trên hướng ngắm khoảng cách đúng bằng $S_{AP}$ để đóng cọc $P$.

**6. Kiểm tra bằng trực giác.**  
- Khi bố trí độ cao: Nếu cao độ thiết kế $H_{tk}$ cao hơn cao độ mốc gốc ($H_{tk} > H_A$), tia ngắm máy sẽ cắt phần dưới của mia tại cọc $B$, nên số đọc $b_{tk}$ sẽ nhỏ hơn $a$ ($b_{tk} < a$).  
- Ngược lại, nếu cần đào hố móng xuống sâu ($H_{tk} < H_A$), mia phải đưa xuống thấp, tia ngắm cắt phần ngọn của mia $\Rightarrow$ số đọc $b_{tk}$ sẽ rất lớn.

**7. Bẫy khi thi.**  
- **Nhầm công thức tính số đọc thiết kế**: Lấy $b_{tk} = H_{tk} - H_{tia}$ (bị ngược dấu). Nếu $b_{tk}$ tính ra âm có nghĩa là cao độ thiết kế nằm cao hơn cả tia ngắm của máy (không thể đọc mia theo cách dựng đứng bình thường mà phải lật ngược mia).
- **Quên đo hai vị trí bàn độ khi bố trí góc**: Khi quay góc thiết kế $\beta_{tk}$, nếu chỉ quay một lần ở bàn độ trái (thuận kính) thì sai số góc $2C$ và sai số trục quay không được khử. Phải quay cả bàn độ trái và bàn độ phải, chấm hai điểm trên cọc rồi lấy điểm chính giữa.
- **Không kiểm tra lại sau khi cắm mốc (kiểm tra độc lập)**: Sau khi cắm xong điểm $P$, không đo kiểm tra khoảng cách từ $P$ đến một mốc thứ ba khác $C$, làm sót sai số thô bạo.

**8. Liên kết.**  
- Kiến thức trước: Đo góc bằng, đo khoảng cách, thủy chuẩn hình học (Chương 3); hai bài toán trắc địa cơ bản (Chương 4).  
- Kiến thức sau: Dẫn trục lên các tầng cao trong thi công nhà bê tông cốt thép; quan trắc độ biến dạng của móng công trình sau khi xây dựng (Chương 7).

**9. Tự kiểm tra.**  
- **Bản chất**: Tại sao phương pháp cao độ tia ngắm ($H_{tia} = H_A + a$) lại đặc biệt thuận tiện trên công trường xây dựng khi cần bố trí cao độ cho hàng chục cọc móng cùng lúc?  
  *Đáp*: Vì chỉ cần đọc mốc chuẩn một lần duy nhất để xác định $H_{tia}$ cố định; sau đó cao độ thiết kế của mọi điểm bất kỳ đều tính nhanh bằng công thức $b_{tk} = H_{tia} - H_{tk}$ mà không cần di chuyển máy.
- **Áp dụng**: Cần bố trí cốt sàn $+0.000$ (cao độ thiết kế $H_{tk} = 15.500$ m). Máy thủy chuẩn ngắm vào mốc chuẩn độ cao $M$ ($H_M = 14.800$ m) có số đọc chỉ giữa là $1650$ mm. Hỏi số đọc $b_{tk}$ trên mia dựng tại cột nhà phải bằng bao nhiêu để vạch cốt $+0.000$?  
  *Đáp*: $H_{tia} = 14.800 + 1.650 = 16.450$ m.  
  $b_{tk} = H_{tia} - H_{tk} = 16.450 - 15.500 = 0.950\text{ m} = 950$ mm.
- **Bẫy**: Một kỹ sư tính ra $b_{tk} = -300$ mm khi dựng mia bố trí đáy dầm trần nhà. Ý nghĩa của dấu âm này là gì và người đo phải làm thế nào?  
  *Đáp*: Dấu âm có nghĩa là điểm cần đánh dấu cao hơn tia ngắm của máy $300$ mm. Người đo phải lật ngược mia (chân mia tựa lên đáy dầm, ngọn mia quay xuống dưới) và đọc số $300$ mm tại chỉ giữa.

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 128–143 (Chương 6, Mục 6.1, 6.3).
