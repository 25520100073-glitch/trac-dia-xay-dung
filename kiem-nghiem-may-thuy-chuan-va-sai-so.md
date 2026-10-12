# Kiểm nghiệm máy thủy chuẩn và Các nguồn sai số (Level inspection and Error sources)

**1. Bản chất trong một câu.**  
Kiểm nghiệm máy thủy chuẩn là quy trình kiểm tra và điều chỉnh để trục ngắm quang học hoàn toàn song song với trục ống thủy dài ($CC_1 \parallel LL_1$), nhằm đảm bảo tia ngắm phát ra là một đường nằm ngang tuyệt đối khi bọt nước đã nằm chính giữa.

**2. Vì sao cần nó.**  
Nếu trục ngắm không song song với trục bọt thủy, máy sẽ có **sai số góc $i$** làm tia ngắm luôn bị hất lên hoặc chúc xuống; nếu dẫn tuyến đo dài qua nhiều trạm máy mà không triệt tiêu sai số này, sai lệch cao độ tích lũy sẽ làm nghiêng lệch toàn bộ cao độ sàn và móng công trình.

**3. Nguyên lý nền.**  
- Điều kiện hình học chủ yếu của máy thủy chuẩn: Trục ngắm $CC_1$ phải song song với trục ống thủy dài $LL_1$ (Chương 3, Mục 3.3.3).  
- Nguyên lý triệt tiêu sai số đối xứng: Đặt máy ở chính giữa hai mia ($S_1 = S_2$), độ lệch tia ngắm trên hai mia là bằng nhau nên tự động triệt tiêu khi lấy hiệu $h = a - b$.  
- Ảnh hưởng của độ cong Trái Đất và chiết quang khí quyển: Tia ngắm bị nâng cao so với mặt thủy chuẩn cầu một lượng $f = \frac{D^2}{2R}(1 - k)$ (Chương 1 & Chương 3, Mục 3.3.5.2).

**4. Mô hình hóa.**  
- Giả thiết: Khi cân bọt thủy ống thủy tròn hoặc ống thủy dài, bọt nước nằm đúng vạch chuẩn trung tâm.  
- Điều kiện mất hiệu lực: Máy bị va đập cơ học trong lúc vận chuyển hoặc nhiệt độ môi trường thay đổi đột ngột làm lệch vít quang học, khiến góc $i$ vượt quá hạn sai cho phép ($|i| > 20''$).

**5. Suy công thức từ nguyên lý.**  

**(a) Kiểm nghiệm và xác định sai số góc $i$ của máy thủy chuẩn (Mục 3.3.3, trang 64–65):**  
- **Phương pháp đo 2 trạm (hoặc đo từ giữa rồi đo lệch một bên)**:  
  1. Chọn hai điểm $A$ và $B$ cách nhau khoảng $40 \div 50$ m.  
  2. Đặt máy ở chính giữa ($I_1$): Vì $S_1 = S_2$ nên sai số góc $i$ bị triệt tiêu, chênh cao thực tế giữa hai điểm là:  
     $$h_{thực} = a_1 - b_1$$  
  3. Dời máy đến đặt gần sát điểm $A$ (trạm $I_2$, cách $A$ khoảng $2 \div 3$ m): Đọc số trên mia $A$ là $a_2$, đọc trên mia $B$ là $b_2$.  
     - Vì máy rất gần $A$, số đọc $a_2$ coi như không bị ảnh hưởng bởi góc $i$.  
     - Số đọc đúng về mặt lý thuyết trên mia $B$ phải là:  
       $$b_{đúng} = a_2 - h_{thực}$$  
     - Sai lệch đọc số trên mia $B$ do góc $i$ gây ra là:  
       $$\Delta b = b_2 - b_{đúng}$$  
  4. Trị số sai số góc $i$ (tính bằng giây góc):  
     $$i = \frac{\Delta b}{D_{AB}} \cdot \rho'' \quad (\text{với } \rho'' = 206265'')$$  
  - Tiêu chuẩn: Nếu $|i| \le 20''$ (hoặc $|\Delta b| \le 3 \div 4$ mm trên khoảng cách $50$ m) thì máy đạt chuẩn. Nếu vượt quá phải chỉnh ốc màng dây chữ thập để đưa số đọc trên mia $B$ về đúng $b_{đúng}$.

**(b) 6 nguồn sai số trong đo thủy chuẩn và biện pháp khắc phục (Mục 3.3.5, trang 68):**  

| Nguồn sai số | Bản chất và ảnh hưởng | Biện pháp triệt tiêu / Khắc phục |
|:---|:---|:---|
| **1. Sai số góc $i$** | Tia ngắm nghiêng góc $i$, số đọc mia lệch: $\Delta a = S_1 \tan i$, $\Delta b = S_2 \tan i$. | **ĐẶT MÁY Ở CHÍNH GIỮA HAI MIA ($S_1 = S_2$)** $\implies$ Hai sai số bằng nhau, tự triệt tiêu khi lấy $h = a - b$. |
| **2. Độ cong Trái Đất & chiết quang khí quyển** | Mặt cầu uốn cong và khúc xạ khí quyển làm mia bị đọc cao hơn: $f = \frac{S^2}{2R}(1 - k)$. | **ĐẶT MÁY Ở CHÍNH GIỮA HAI MIA ($S_1 = S_2$)** $\implies$ $f_a = f_b$, tự triệt tiêu hoàn toàn khi lấy hiệu. |
| **3. Sai số do mia bị nghiêng** | Mia nghiêng góc $\theta$, tia ngắm cắt mia ở vị trí cao hơn: $b_{đo} = \frac{b_{thực}}{\cos\theta} > b_{thực}$. **Số đọc LUÔN BỊ TĂNG**. | Gắn bọt thủy tròn trên thân mia; giữ thăng bằng cẩn thận; lắc mia lấy số đọc nhỏ nhất. |
| **4. Sai số do vạch chia và mòn đế mia** | Đế mia bị mòn làm số đọc bị tụt xuống; vạch khắc bị giãn nở nhiệt. | Kiểm định mia trước khi đo; đo tuyến có **số trạm máy chẵn** và tráo mia sau/trước luân phiên. |
| **5. Sai số do lún chân máy và lún cóc đệm** | Máy hoặc mia bị lún xuống nền đất mềm trong quá trình ngắm đọc. | Dùng cóc đệm mia chuyên dụng bằng gang đúc, đạp chân máy vững chắc, thao tác đo nhanh chóng. |
| **6. Sai số ngắm và đọc số của mắt** | Mắt người ước lượng phần mười milimét bị dao động ngẫu nhiên. | Tuân thủ hạn sai: $m_{đọc} \le \frac{m_{h,cp}}{\sqrt{2}}$. |

**6. Kiểm tra bằng trực giác.**  
- Đặt máy ở giữa giống như một chiếc đòn bẩy đối xứng: Nếu tia ngắm ngóc lên một góc $i$, cả đầu sau và đầu trước đều bị ngóc lên một lượng như nhau, hiệu số độ cao không hề bị ảnh hưởng.  
- Khi mia nghiêng, cạnh huyền luôn dài hơn cạnh góc vuông $\implies$ số đọc mia luôn bị tăng lên, không bao giờ bị giảm đi.

**7. Bẫy khi thi.**  
- **Nghĩ rằng đặt máy ở giữa triệt tiêu được mọi sai số**: Đặt máy ở giữa chỉ triệt tiêu được **sai số góc $i$** và **độ cong Trái Đất/chiết quang**. Nó **không thể** triệt tiêu sai số do mia nghiêng, lún máy hay mắt đọc sai.  
- **Trả lời sai câu hỏi mia nghiêng làm số đọc tăng hay giảm**: Luôn nhớ: Mia nghiêng làm số đọc **TĂNG**, do đó khi lắc mia, số đọc **nhỏ nhất** mới là số đọc đúng lúc mia thẳng đứng.

**8. Liên kết.**  
- Kiến thức trước: Cấu tạo máy thủy chuẩn và ống thủy dài (Chương 3, Mục 3.3.2).  
- Kiến thức sau: Đánh giá sai số chuỗi trạm đo (Chương 2, Mục 2.3); bình sai tuyến thủy chuẩn kỹ thuật (Chương 4, Mục 4.2.2); quan trắc độ lún công trình cấp chính xác I và II (Chương 7).

**9. Tự kiểm tra.**  
- **Bản chất**: Tại sao khi đo thủy chuẩn kỹ thuật, quy phạm luôn yêu cầu chênh lệch khoảng cách từ máy đến hai mia sau và trước phải thỏa mãn $|S_1 - S_2| \le 5$ m?  
  *Đáp*: Để đảm bảo điều kiện đặt máy ở giữa được duy trì chặt chẽ, nhờ đó sai số góc $i$ của máy và độ cong Trái Đất giữa hai hướng ngắm triệt tiêu lẫn nhau gần như tuyệt đối, không tích lũy thành sai số hệ thống trên toàn tuyến.  
- **Áp dụng**: Kiểm nghiệm máy thủy chuẩn trên đoạn $AB = 50$ m. Đặt máy ở giữa đo được $h_{thực} = +0.350$ m. Đặt máy gần $A$ đọc được $a_2 = 1.420$ m, $b_2 = 1.076$ m. Tính góc $i$ của máy?  
  *Đáp*: Số đọc đúng trên mia $B$: $b_{đúng} = a_2 - h_{thực} = 1.420 - 0.350 = 1.070$ m $= 1070$ mm.  
  Sai lệch đọc số: $\Delta b = b_2 - b_{đúng} = 1076 - 1070 = +6$ mm.  
  Góc nghiêng: $i = \frac{6\text{ mm}}{50000\text{ mm}} \times 206265'' \approx +24.75''$.  
  Vì $|i| = 24.75'' > 20''$, máy cần phải hiệu chỉnh lại góc $i$.  
- **Bẫy**: Khi đo thủy chuẩn, một kỹ thuật viên lắc mia và ghi lại số đọc lớn nhất. Thao tác này đúng hay sai?  
  *Đáp*: Sai hoàn toàn. Khi lắc mia, vạch mia cắt tia ngắm nằm ngang tạo tam giác vuông mà vị trí thẳng đứng là cạnh góc vuông (ngắn nhất), các vị trí nghiêng là cạnh huyền (dài hơn). Vì vậy phải lấy **số đọc nhỏ nhất**, đó mới là số đọc khi mia thẳng đứng.

---
*Nguồn trích dẫn*: `Tai_lieu HT_Trac dia_XD-T_Tai_2025.pdf`, trang 64–68 (Mục 3.3.3, 3.3.5).
