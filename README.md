# Hopfield Network for Associative Memory

## Giới thiệu

Dự án này trình bày việc **cài đặt, thử nghiệm và đánh giá mạng Hopfield** trong bài toán **bộ nhớ liên kết (Associative Memory)**. Toàn bộ quá trình thực nghiệm được triển khai trong notebook:

```
SOICT_Do_an_tot_nghiep.ipynb
```

Notebook bao gồm các bước:
- Xây dựng và triển khai mô hình **Hopfield Network**
- Huấn luyện mạng với các mẫu dữ liệu đầu vào
- Khôi phục lại các mẫu đã học từ dữ liệu bị nhiễu
- Phân tích và đánh giá hiệu quả của mô hình

Mục tiêu của dự án là minh họa cách **mạng Hopfield có thể lưu trữ và truy hồi thông tin giống như cơ chế bộ nhớ trong não bộ**.

---

# Hopfield Network là gì?

**Hopfield Network** là một dạng **mạng nơ-ron hồi tiếp (Recurrent Neural Network)** được đề xuất bởi **John Hopfield (1982)**. Mạng này được thiết kế để hoạt động như một **hệ thống bộ nhớ liên kết** có khả năng:

- Lưu trữ nhiều mẫu dữ liệu
- Khôi phục lại mẫu gốc từ dữ liệu bị thiếu hoặc bị nhiễu

Hopfield Network hoạt động dựa trên nguyên lý **tối thiểu hóa hàm năng lượng (Energy Function)**. Khi một mẫu dữ liệu được đưa vào mạng, hệ thống sẽ cập nhật trạng thái của các neuron cho đến khi đạt đến **điểm cân bằng (stable state)** tương ứng với một mẫu đã được lưu trữ.

Một số đặc điểm nổi bật của Hopfield Network:

- Mạng fully connected giữa các neuron
- Trọng số đối xứng giữa các kết nối
- Không có kết nối từ neuron đến chính nó
- Có thể hoạt động như một **content-addressable memory**

Ứng dụng của Hopfield Network bao gồm:

- Associative memory
- Pattern completion
- Image denoising
- Optimization problems

---

# Nội dung notebook

File notebook thực hiện các bước chính sau:

1. **Xây dựng Hopfield Network**
2. **Huấn luyện mạng với các mẫu dữ liệu**
3. **Thử nghiệm khả năng khôi phục dữ liệu từ nhiễu**
4. **Phân tích năng lượng của mạng**
5. **Đánh giá hiệu năng và khả năng lưu trữ của mô hình**

Các thí nghiệm được minh họa trực quan bằng biểu đồ và hình ảnh.

---

# Yêu cầu môi trường

Để chạy notebook, cần cài đặt các phần mềm sau:

- **Python 3.8+**
- **Jupyter Notebook** hoặc **Jupyter Lab**

---

# Thư viện sử dụng

Dự án sử dụng các thư viện Python phổ biến trong lĩnh vực khoa học dữ liệu và học máy:

- `numpy` – xử lý tính toán ma trận
- `matplotlib` – trực quan hóa dữ liệu
- `torch` – hỗ trợ xây dựng và thử nghiệm mô hình
- `torchvision` – hỗ trợ dữ liệu hình ảnh
- `seaborn` – trực quan hóa thống kê
- `tqdm` – hiển thị tiến trình chạy
- `scipy` – các phép toán khoa học
- `imageio` – xử lý ảnh
- `requests` – tải dữ liệu từ internet

Cài đặt tất cả thư viện cần thiết bằng lệnh:

```bash
pip install -r requirements.txt
```

---

# Cách chạy dự án

Sau khi cài đặt các thư viện cần thiết, mở notebook bằng Jupyter:

```bash
jupyter notebook
```

Sau đó mở file:

```
SOICT_Do_an_tot_nghiep.ipynb
```

và chạy lần lượt các cell trong notebook để thực hiện toàn bộ quá trình thí nghiệm.

---

# Mục tiêu nghiên cứu

Dự án nhằm mục tiêu:

- Hiểu rõ cơ chế hoạt động của **Hopfield Network**
- Minh họa khả năng **lưu trữ và truy hồi mẫu dữ liệu**
- Phân tích ảnh hưởng của nhiễu đến khả năng khôi phục mẫu
- Thực nghiệm các phương pháp cải thiện hiệu quả của mạng

---

# Tài liệu tham khảo

1. Hopfield, J. J. (1982).  
   *Neural networks and physical systems with emergent collective computational abilities.*

2. Goodfellow, Bengio, Courville.  
   *Deep Learning – MIT Press*

3. Bishop, C.  
   *Pattern Recognition and Machine Learning*
