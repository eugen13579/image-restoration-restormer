# Image Restoration with Restormer

Đồ án khảo sát và đánh giá mô hình Restormer cho bài toán khử nhòe ảnh chuyển động (*motion deblurring*).

## 1. Mục tiêu

- Tìm hiểu các phương pháp phục hồi ảnh dựa trên học sâu.
- Nghiên cứu kiến trúc Restormer, bao gồm MDTA và GDFN.
- Triển khai suy luận với trọng số pretrained dành cho motion deblurring.
- Đánh giá chất lượng ảnh phục hồi bằng PSNR và SSIM.
- Trình bày kết quả thực nghiệm trong báo cáo LaTeX tiếng Việt.

## 2. Công nghệ sử dụng

- Python
- PyTorch
- OpenCV và NumPy
- scikit-image
- LaTeX

## 3. Mô hình và tài liệu gốc

- Bài báo Restormer: https://openaccess.thecvf.com/content/CVPR2022/html/Zamir_Restormer_Efficient_Transformer_for_High-Resolution_Image_Restoration_CVPR_2022_paper.html
- Mã nguồn chính thức: https://github.com/swz30/Restormer

Mô hình được sử dụng trong đồ án là checkpoint pretrained dành cho bài toán khử nhòe ảnh chuyển động. Vui lòng tham khảo repository chính thức để biết hướng dẫn tải trọng số, cấu hình và các yêu cầu về giấy phép.

## 4. Cấu trúc dự án

- `Restormer/`: mã nguồn và cấu hình mô hình.
- `report/`: source LaTeX của báo cáo.
- `results/`: một số kết quả minh họa đã chọn, nếu có.
- `README.md`: hướng dẫn và thông tin dự án.

## 5. Dữ liệu và trọng số

Dataset GoPro và các checkpoint pretrained không được lưu trực tiếp trong repository này. Hãy tải chúng từ nguồn được tác giả hoặc đơn vị phát hành chỉ định và tuân thủ điều kiện sử dụng tương ứng.

## 6. Kết quả thực nghiệm

Trong lần đánh giá Python đã ghi nhận:

- Số ảnh được đánh giá: 1.111
- PSNR trung bình: 32,9176 dB
- SSIM trung bình: 0,9396

Các chỉ số trên phản ánh kết quả của quy trình đánh giá đã sử dụng trong đồ án. Giao thức tính toán cần được xác minh trước khi đối chiếu trực tiếp với kết quả công bố trong bài báo gốc.

## 7. Báo cáo

Báo cáo được viết bằng LaTeX, trình bày cơ sở lý thuyết, các công trình liên quan, quy trình triển khai, kết quả thực nghiệm và hướng phát triển.

## 8. Ghi nhận nguồn

Restormer được phát triển và công bố bởi các tác giả của công trình nghiên cứu gốc. Mã nguồn, trọng số và dữ liệu của bên thứ ba cần được sử dụng theo giấy phép và điều kiện phân phối tương ứng.