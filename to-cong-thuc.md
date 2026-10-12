# Tờ công thức cô đọng: Trắc địa xây dựng (Chương 3 & 4)

Quy ước: Số đọc mia tính bằng mm; độ cao và chênh cao tính bằng m (chia 1000). Tờ này dùng để ôn tập cấp tốc trước giờ thi.

---

## 1. Thủy chuẩn hình học & Sai số (Chương 3 & Chương 2)

| Công thức | Ý nghĩa & Điều kiện áp dụng |
|:---|:---|
| $h_{MN} = a - b$ | Thủy chuẩn từ giữa: $a$ (mia sau $M$), $b$ (mia trước $N$). Đổi ra m: chia 1000. |
| $H_N = H_M + h_{MN}$ | Truyền độ cao điểm trước. |
| $m_h = m_{đọc}\sqrt{2}$ | Sai số trung phương chênh cao 1 trạm máy. Bài 1 câu 3: $0.5\sqrt{2} \approx \pm 0.707$ mm. |
| $m_{đọc} \le \frac{m_{h,cp}}{\sqrt{2}}$ | Bài toán ngược tìm sai số đọc mia. Bài 1 câu 4: $5/\sqrt{2} \approx \pm 3.536$ mm. |
| $m_{tuyến} = m_h\sqrt{N} = m_{đọc}\sqrt{2N}$ | Sai số tích lũy toàn tuyến qua $N$ trạm máy độc lập. |
| $D = 100 \cdot (c_t - c_d)$ | Đo cự ly bằng chỉ thị cự (đổi mm ra m: $0.1 \times n$). Mia thẳng đứng, tia ngắm nghiêng góc $V$: $S = 100(c_t - c_d)\cos V$, $D = 100(c_t - c_d)\cos^2 V$. |
| $c_t = 2c_g - c_d$ | Tái dựng chỉ trên khi bị che khuất. Đối xứng: $c_g = (c_t + c_d)/2$. |

---

## 2. Đo cao lượng giác (Chương 3)

| Công thức | Ý nghĩa & Điều kiện áp dụng |
|:---|:---|
| $h = D \tan V + i - l$ | Công thức tổng quát ($V$ là góc đứng, $i$ là chiều cao máy, $l$ là chiều cao ngắm). |
| $h_{CĐ} = D(\tan V_Đ - \tan V_C)$ | Chiều cao công trình không thể tới chân mia ($i$ triệt tiêu, $L_1 = L_2 = 0$). |
| $V = \text{độ} + \frac{\text{phút}}{60}$ | Đổi phút ra độ thập phân. **Ngắm lên $V_Đ > 0$; ngắm xuống $V_C < 0$**. |
| $\Delta \tan = \tan V_Đ - \tan V_C$ | Trừ cho số âm thành cộng: $\tan V_Đ - (-|\tan V_C|) = \tan V_Đ + |\tan V_C|$. |

---

## 3. Máy kinh vĩ & Đo góc (Chương 3)

| Công thức | Ý nghĩa & Điều kiện áp dụng |
|:---|:---|
| $\beta = \frac{\beta_L + \beta_R}{2}$ | Đo góc bằng 2 vị trí bàn độ: Thuận kính (L) và Đảo kính (R) để triệt tiêu sai số $2c$. |
| $2c = \|L - (R \pm 180^\circ)\|$ | Sai số ngắm do trục ngắm không vuông góc trục quay ống kính ($CC_1 \not\perp HH_1$). |
| $MO = \frac{L + R - 360^\circ}{2}$ | Sai số chỉ tiêu bàn độ đứng. Góc đứng: $V = L - MO = MO - R + 180^\circ$. |

---

## 4. Bình sai tuyến thủy chuẩn kỹ thuật (Chương 4)

| Công thức | Ý nghĩa & Điều kiện áp dụng |
|:---|:---|
| $f_h = \sum h_{đo} - (H_{cuối} - H_{đầu})$ | Sai số khép tuyến phù hợp. Tuyến khép kín: $f_h = \sum h_{đo}$ (vì $H_{cuối} = H_{đầu}$). |
| $f_{hcp} = \pm 50\sqrt{L}$ (mm) | Tuyến đo theo chiều dài: $L = \sum D_i / 1000$ (tính bằng **km**). |
| $f_{hcp} = \pm 10\sqrt{N}$ (mm) | Tuyến đo vùng dốc hiểm trở theo tổng số trạm máy $N = \sum n_i$. |
| $v_{hi} = -\frac{f_h}{\sum D_i} \cdot D_i$ | Phân bổ số hiệu chỉnh theo cự ly ($v_{hi} = -\frac{f_h}{N} \cdot n_i$ theo số trạm). **Kiểm tra: $\sum v_{hi} = -f_h$**. |
| $h_i^{BS} = h_{đo, i} + v_{hi}$ | Chênh cao bình sai. Kiểm tra: $\sum h^{BS} = H_{cuối} - H_{đầu}$. |
| $H_i = H_{i-1} + h_i^{BS}$ | Độ cao bình sai các điểm. Điểm cuối phải trùng khít tuyệt đối với $H_{cuối}$. |
| $h_{N1A} = -h_{AN1}$ | **Đổi chiều đoạn đầu khi tính mốc công trình $A$ từ trạm máy ngắm 2 mốc $N_1, N_2$!** |

---

## 5. Kinh vĩ & Tọa độ phẳng (Chương 4)

| Công thức | Ý nghĩa & Điều kiện áp dụng |
|:---|:---|
| $\alpha_{sau} = \alpha_{trước} + \beta_{trái} - 180^\circ$ | Truyền góc định hướng khi đo góc ngoặt bên **Trái** (trang 96–98 giáo trình). |
| $\alpha_{sau} = \alpha_{trước} + 180^\circ - \beta_{phải}$ | Truyền góc định hướng khi đo góc ngoặt bên **Phải**. |
| $\Delta X = D \cdot \cos\alpha; \quad \Delta Y = D \cdot \sin\alpha$ | Bài toán thuận: Trục $X$ hướng Bắc (đi với $\cos$), trục $Y$ hướng Đông (đi với $\sin$). |
| $D = \sqrt{\Delta X^2 + \Delta Y^2}; \quad r = \arctan\|\frac{\Delta Y}{\Delta X}\|$ | Bài toán nghịch: Xét dấu $\Delta X, \Delta Y$ để chuyển về góc định hướng $\alpha$ (I: $r$, II: $180^\circ-r$, III: $180^\circ+r$, IV: $360^\circ-r$). |
| $1/T = \frac{\sqrt{f_x^2 + f_y^2}}{\sum D} \le \frac{1}{2000}$ | Sai số khép tương đối đường chuyền kinh vĩ khống chế mặt bằng. |

---

## 6. Check-list 5 bẫy trừ điểm nặng nhất trong phòng thi:
1. **Quên $\sqrt{2}$**: Tính sai số chênh cao luôn là $m_h = m_{đọc}\sqrt{2}$.
2. **Ngược dấu thủy chuẩn**: $h = a - b$ (Sau trừ Trước), không lấy $b - a$.
3. **Quên đổi đơn vị**: Chia 1000 khi đổi mm sang m; đổi cự ly $\sum D$ sang km trước khi bấm $50\sqrt{L}$.
4. **Bấm nhầm hàm tang**: Bấm $\tan V_Đ - \tan V_C$, tuyệt đối không bấm $\tan(V_Đ - V_C)$.
5. **Mốc công trình $A$**: Đổi dấu đoạn đầu $h_{N1A} = -h_{AN1}$, không để nguyên số âm!
