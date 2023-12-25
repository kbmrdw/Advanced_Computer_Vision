# Advanced_Computer_Vision
## Tên đề tài: CONTENT-BASED IMAGE RETRIEVAL
## Giới thiệu bài toán
Tìm kiếm ảnh theo nội dung (Content Based Images Retrieval - CBIR) hay truy vấn theo nội dung ảnh (Query Based Image Content - QBIC) là một ứng dụng của thị giác máy tính đối với bài toán tìm kiếm ảnh. “Dựa vào nội dung ảnh (Content Based)” nghĩa là việc tìm kiếm sẽ phân tích nội dung thực sự của các bức ảnh. Nội dung ảnh ở đây được thể hiện bằng màu sắc, hình dạng, kết cấu (texture), các đặc trưng cục bộ (local features), … hay bất cứ thông tin nào có từ chính nội dung ảnh.
- **Input:** 1 tấm ảnh chứa đối tượng cần tìm kiếm
- **Output:** Top 10 bức ảnh tương đồng với input

### **Dataset**: [corel_images](https://www.kaggle.com/datasets/elkamel/corel-images)
- Bộ dữ liệu gồm 1000 ảnh được chia vào 10 nhóm, mỗi nhóm gồm 100 ảnh, mỗi ảnh chứa một hoặc nhiều đối tượng của nhóm đó.
- Tiến hành chia các ảnh trong bộ dữ liệu thành 2 phần, mỗi phần có số nhóm giống như danh sách nhóm gốc theo tỷ lệ 9/15
  - **Database:** chiếm 9/10 tổng số ảnh => có tổng 900 ảnh với 90 ảnh trên mỗi nhóm.
  - **Query:** chiếm 1/10 tổng số ảnh => có tổng 100 ảnh với 10 ảnh trên mỗi nhóm.

###



## Phương pháp trích xuất đặc trưng
- Color Histogram
- Histogram of oriented gradients (HOG)
- Resnet50

## Phương pháp so sánh
- Cosine similarity
- So sánh tuần tự để chọn ra TOP-K
- Gom nhóm bằng K-Nearest Neighbor

## Phương pháp đánh giá
- Precision at k (P@K)
- Recall at k (R@K)
- Average Precision (AP)
- Mean Average Precision (MAP)

***Code demo:*** https://github.com/kbmrdw/Advanced_Computer_Vision/blob/main/Code/demo.ipynb

