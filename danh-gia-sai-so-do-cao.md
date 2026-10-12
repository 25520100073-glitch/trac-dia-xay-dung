# Đánh giá sai số đo cao và truyền sai số (Error propagation in leveling)

**1. Bản chất trong một câu.**  
Định luật truyền sai số xác định độ dao động ngẫu nhiên (sai số trung phương) của chênh cao kết quả dựa trên sự tích lũy sai số của từng số đọc thành phần trên mia.

**2. Vì sao cần nó.**  
Một con số đo đạc trên thực địa chỉ có ý nghĩa khi đi kèm với mức độ tin cậy của nó; nếu không biết sai số trung phương, ta không thể chọn loại máy thủy chuẩn phù hợp, không biết cần đọc mia cẩn thận đến mức nào, và không thể nghiệm thu công trình theo tiêu chuẩn kỹ thuật.

**3. Nguyên lý nền.**  
- Khái niệm sai số trung phương (root mean square error / standard error) $m = \sqrt{\frac{\sum \Delta_i^2}{n}}$ (Chương 2, Mục 2.2.2).  
- Định luật truyền sai số của Gauss cho hàm số tuyến tính các đại lượng đo độc lập $y = k_1 x_1 + k_2 x_2 + \dots$:  
  $$m_y = \sqrt{k_1^2 m_1^2 + k_2^2 m_2^2 + \dots} \quad (\text{Chương 2, Mục 2.3})$$  
- Nguyên tắc đồng ảnh hưởng (principle of equal influence): Khi nhiều nguồn sai số cùng đóng góp vào một kết quả, giải pháp kinh tế nhất là phân bổ để mức ảnh hưởng của từng nguồn là xấp xỉ nhau (Chương 2, Mục 2.5).

**4. Mô hình hóa.**  
- Giả thiết: Các lần đọc số trên mia sau và mia trước là các biến ngẫu nhiên độc lập, tuân theo phân bố chuẩn Gauss; không có sai số hệ thống thô bạo (máy đã được kiểm nghiệm bọt thủy và hiệu chỉnh góc $i$).  
- Điều kiện mất hiệu lực: Tồn tại sai số hệ thống chưa loại trừ (như vạch mia bị co giãn do nhiệt độ, mia bị nghiêng cùng một chiều, hoặc lún chân máy liên tục theo thời gian). Khi đó sai số tích lũy theo bậc nhất ($n$), không còn tích lũy theo căn bậc hai ($\sqrt{n}$).

**5. Suy công thức từ nguyên lý.**  
(a) Hàm xác định chênh cao của một trạm máy:  
$$h = a - b \quad (a\text{: số đọc mia sau, } b\text{: số đọc mia trước})$$  
(b) Đạo hàm riêng theo từng biến: $\frac{\partial h}{\partial a} = +1$; $\frac{\partial h}{\partial b} = -1$.  
(c) Áp dụng định luật truyền sai số Gauss:  
$$m_h^2 = \left(\frac{\partial h}{\partial a}\right)^2 m_a^2 + \left(\frac{\partial h}{\partial b}\right)^2 m_b^2 = (+1)^2 m_a^2 + (-1)^2 m_b^2 = m_a^2 + m_b^2$$  
(d) Khi dùng cùng một mia và cùng người đo, độ chính xác hai lần đọc là như nhau ($m_a = m_b = m_{đọc}$):  
$$m_h = \sqrt{m_{đọc}^2 + m_{đọc}^2} = m_{đọc}\sqrt{2} \approx 1.414 \cdot m_{đọc} \quad (\text{Đơn vị: mm})$$  
(e) Tuyến đo gồm $N$ trạm máy độc lập có cùng độ chính xác: $h_{tổng} = \sum_{i=1}^N h_i$.  
$$m_{tuyến} = \sqrt{\sum_{i=1}^N m_h^2} = \sqrt{N \cdot m_h^2} = m_h \sqrt{N} = m_{đọc}\sqrt{2N} \quad (\text{Đơn vị: mm})$$

**6. Kiểm tra bằng trực giác.**  
- Đo một trạm máy phải đọc hai lần ($a$ và $b$). Vì hai lần đọc đều có sai số ngẫu nhiên nên sai số của chênh cao luôn lớn hơn sai số của một lần đọc đơn lẻ ($m_h = 1.414 \cdot m_{đọc} > m_{đọc}$).  
- Dấu trừ trong phép tính hiệu $h = a - b$ **không làm giảm** sai số ngẫu nhiên mà làm sai số tăng lên (bình phương hệ số $(-1)^2 = +1$).  
- Số trạm đo tăng gấp 4 lần thì sai số tổng chỉ tăng gấp $\sqrt{4} = 2$ lần (tính chất triệt tiêu một phần của sai số ngẫu nhiên).

**7. Bẫy khi thi.**  
- **Nhầm lẫn giữa dấu trừ trong phép tính và phép tính sai số**: Nghĩ rằng vì $h = a - b$ nên $m_h = m_a - m_b = 0$. Sai số ngẫu nhiên luôn cộng theo bình phương, không bao giờ trừ nhau.
- **Quên nhân hệ số $\sqrt{2}$**: Khi đề bài cho sai số đọc mia là $m_{đọc}$, vội vàng lấy luôn $m_h = m_{đọc}$. Luôn nhớ: một trạm thủy chuẩn gồm hai số đọc $\Rightarrow m_h = \sqrt{2} m_{đọc}$.
- **Nhầm lẫn bài toán thuận và bài toán ngược**:  
  - Bài toán thuận (tìm $m_h$ khi biết $m_{đọc}$): $m_h = m_{đọc}\sqrt{2}$.  
  - Bài toán ngược (tìm $m_{đọc}$ cần thiết để $m_h \le \text{giá trị cho trước}$): $m_{đọc} \le \frac{m_h}{\sqrt{2}} \approx 0.707 \cdot m_h$.

**8. Liên kết.**  
- Kiến thức trước: Các đại lượng đặc trưng cho sai số ngẫu nhiên (Chương 2, Mục 2.2); phép đo thủy chuẩn hình học (Chương 3, Mục 3.3).  
- Kiến thức sau: Công thức tính sai số khép cho phép của tuyến thủy chuẩn theo số trạm $f_{hcp} = \pm 10\sqrt{N}$ mm (Chương 4, Mục 4.2.2); thiết kế lưới quan trắc lún cấp chính xác cao (Chương 7).

**9. Tự kiểm tra.**  
- **Bản chất**: Tại sao sai số trung phương của tổng nhiều trị đo ngẫu nhiên lại tỉ lệ với $\sqrt{N}$ mà không tỉ lệ thuận với $N$?  
  *Đáp*: Vì các sai số ngẫu nhiên có dấu âm và dương xuất hiện với xác suất ngang nhau, nên trong quá trình cộng dồn chúng có xu hướng triệt tiêu lẫn nhau một phần; chỉ có phương sai ($m^2$) mới cộng dồn trực tiếp.
- **Áp dụng (trích đề kiểm tra Slide 131, Câu 3.3)**: Nếu sai số đọc số trên mia là $m_{đọc} = \pm 0.5$ mm, hãy tính sai số trung phương xác định chênh cao $h_{MN}$ trong một trạm đo?  
  *Đáp*: $m_{hMN} = \sqrt{m_a^2 + m_b^2} = m_{đọc}\sqrt{2} = 0.5 \times \sqrt{2} \approx \pm 0.707$ mm.
- **Bẫy (trích đề kiểm tra Slide 131, Câu 3.4)**: Nếu yêu cầu sai số trung phương xác định chênh cao $h_{MN} \le \pm 5$ mm thì người đo phải đọc số với sai số đọc số $m_{đọc}$ tối đa là bao nhiêu?  
  *Đáp*: Từ $m_h = m_{đọc}\sqrt{2} \le 5$ mm $\Rightarrow m_{đọc} \le \frac{5}{\sqrt{2}} \approx \pm 3.536$ mm. (Nếu trả lời là $\pm 5$ mm thì sai vì quên hệ số $\sqrt{2}$).

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 28–32 (Mục 2.2.2, 2.3); slide bài giảng trên lớp `8062724fc142411c1853.jpg` (Slide 131).
