TRANSFER LEARNING AND DATA AUGMENTATION.

Transfer learning.
Có 2 loại transfer learning:
- Feature Extractor: Sau khi lấy ra các feature của ảnh bằng convnet, thì ta sẽ dùng linear classifier, linear SVM, softmax classifier để phân loại ảnh. Có nghĩa là các feature của ảnh sẽ trở thành input của các giải thuật classifier. 
- Fine tuning: Sau khi có được Feature Images bằng ConvNet. Ta sẽ coi đây là input của một CNN khác bằng cách thêm các ConvNet và FC.

Accuracy của Feature Extractor không bằng Fine Tuning. Điều này đồng nghĩa với việc thời gian train của Fine Tuning cũng lâu hơn. Lý do là trong Feature Extractor chỉ lấy các đặc điểm output của ConvNet làm input cho classifier, trong khi Fine Tuning có một giai đoạn trainning lại phần ConvNet nên có độ chính xác cao hơn.

Ngoài transfer learning, có một ký thuật nữa để giải quyết vấn đề thiếu dữ liệu cho việc trainning model đó là data augmentation. Đây là kỹ thuật tạo ra thêm dữ liệu từ lượng dữ liệu mà ta đang có. Một số kỹ thuật Augmanetation phố biến như:
- Flip: Lật ảnh theo chiều dọc hoặc ngang
- Rotation: Xoay ảnh theo một góc bất kỳ.
- Scale: Phóng to hoặc thu nhỏ ảnh.
- Crop: Cắt một vùng ảnh, sau đó resize ảnh về kích thước ban đầu.



