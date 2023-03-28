# NHẬP GIẤY BÁO TỬ #

- Bước 1. Đăng nhập Cổng tiếp nhận dữ liệu Hệ thống thông tin giám định BHYT tại địa chỉ https://gdbhyt.baohiemxahoi.gov.vn bằng tài khoản được cấp.
  - Đăng nhập tài khoản và mật khẩu: [bấm vào đây](https://bsthanh-my.sharepoint.com/:t:/g/personal/laptopxiaomi_bsthanh_onmicrosoft_com/ERTxN1i_KZ9PrFdGWW3ytJABGOz7exkNr6NVr4xWph-gEg?e=dlvluz)
- Bước 2. Chọn chức năng Cấp chứng từ -> Giấy báo tử. Màn hình hiển thị như sau:
  - ![image](https://user-images.githubusercontent.com/82578024/228114044-e78c0d1b-7b44-4c76-a9f8-0d704c0bbdc0.png)
  - ![image](https://user-images.githubusercontent.com/82578024/228114326-1e6ad800-73e9-49db-a7fb-fc3ab7cfad38.png)
- Bước 3. Chọn Thêm mới để tạo mới Giấy báo tử, màn hình hiển thị như sau:
  - ![image](https://user-images.githubusercontent.com/82578024/228114853-c0db882d-64b1-440a-bcbc-3dc417133db2.png)
  - ![image](https://user-images.githubusercontent.com/82578024/228115005-f0487889-808a-4431-a960-a66a25372a42.png)
  - Trong đó, chi tiết các thông tin như mô tả tại mục 2.3 Mô tả cấu trúc dữ liệu, mô tả này nằm trong phần ghi chú:
- Bước 4. Chọn Lưu để lưu lại thông tin đã nhập tại Bước 3 hoặc Lưu & in để lưu lại thông tin đã nhập tại Bước 3 và in Giấy báo tử.

## GHI CHÚ ##

|TT|Chỉ tiêu         |Bắt buộc|Kiểu dữ liệu|Ký tự tối đa|Diễn giải|
|--|--               |--      |--          |--          |--       |
|1 |MA_GBT           |x       |Chuỗi       |18          |Mã giấy báo tử được quản lý tại cơ sở khám chữa bệnh theo quy định của Bộ Y tế, mã gồm 18 ký tự theo định dạng **XXXXX.GBT.96025.YY** Trong đó: **XXXXX** có độ dài 5 ký tự là số thứ tự tăng dần của số giấy chứng sinh đã cấp trong năm tại cơ sở khám chữa bệnh. **GBT**: Là ký tự cố định xác định với các loại giấy khác. **YY**: Độ dài 2 ký tự tương ứng với 2 ký tự cuối của năm cấp giấy. Ví dụ:  **00004.GBT.96025.22**|
|2 |MA_BN            |        |Chuỗi       |255         |Mã bệnh nhân quản lý tại CSKCB|
|3 |MA_HSBA          |        |Chuỗi       |100         |Mã số hồ sơ bệnh án quản lý bệnh nhân tại cơ sở khám chữa bệnh |
|4 |HO_TEN           |x       |Chuỗi       |255         |Họ và tên người bệnh|
|5 |NGAY_SINH        |x       |Chuỗi       |8           |Ngày sinh, định dạng **yyyyMMdd** (nếu không có ngày sinh và tháng sinh thì mặc định là 0101)|
|6 |GIOI_TINH        |x       |Số          |1           |Giới tính, sổ xuống chọn cho phù hợp|
|7 |MA_THE           |        |Chuỗi       |15          |Mã thẻ BHYT do cơ quan BHXH cấp|
|8 |MA_DANTOC        |x       |Chuỗi       |2           |Mã dân tộc, sổ xuống chọn cho phù hợp|  
|9 |MA_QUOCTICH      |x       |Chuỗi       |2           |Mã quốc tịch, sổ xuống chọn cho phù hợp|
|10|DCHI_THUONGTRU   |x       |Chuỗi       |250         |Địa chỉ đường phố, thôn xóm, số nhà thường trú, tự nhập đánh tay|
|11|MATINH_THUONGTRU |x       |Chuỗi       |2           |Mã tỉnh thường trú, sổ xuống chọn cho phù hợp|
|12|MAHUYEN_THUONGTRU|x       |Chuỗi       |3           |Mã huyện thường trú, sổ xuống chọn cho phù hợp|
|13|MAXA_THUONGTRU   |x       |Chuỗi       |5           |Mã xã thường trú, sổ xuống chọn cho phù hợp|
|14|DCHI_HIENTAI     |        |Chuỗi       |255         |Địa chỉ hiện tại|
|15|MATINH_HIENTAI   |        |Chuỗi       |2           |Mã tỉnh theo địa chỉ hiện tại, sổ xuống chọn cho phù hợp|
|16|MAHUYEN_HIENTAI  |        |Chuỗi       |3           |Mã huyện theo địa chỉ hiện tại, sổ xuống chọn cho phù hợp|
|17|MAXA_HIENTAI     |        |Chuỗi       |3           |Mã xã theo địa chỉ hiện tại, sổ xuống chọn cho phù hợp|
|18|LOAI_GIAYTO      |x       |Số          |1           |Loại giấy tờ, sổ xuống chọn cho phù hợp|
|19|SO_GIAYTO        |x       |Chuỗi       |15          |Số tự điền trên loại giấy tờ|
|20|NGAY_CAP         |x       |Chuỗi       |8           |Ngày cấp giấy tờ, định dạng **yyyyMMdd**, sổ xuống chọn cho phù hợp|  
|21|NOI_CAP          |x       |Chuỗi       |250         |Nơi cấp giấy tờ, tự điền|
|22|NGAYGIO_VV       |x       |Chuỗi       |12          |Thời gian vào viện, định dạng **yyyyMMddHHss**, với **yyyy** là năm vào viện, **MM** là tháng vào viện, **dd** là ngày vào viện, **HH** là giờ vào viện, **ss** là phút vào viện, sổ xuống chọn|
|23|NGAY_TV          |x       |Chuỗi       |12          |Thời gian tử vong, định dạng **yyyyMMddHHss**, với **yyyy** là năm tử vong, **MM** là tháng tử vong, dd là ngày tử vong, HH là giờ tử vong, ss là phút tử vong|
|24|TINH_TRANG_TV    |x       |Số          |1           |Tử vong khi đang trên đường đi cấp cứu, có thì check vào, không thì thôi|
|25|NGUYENNHAN_TV    |x       |Chuỗi       |255         |Chẩn đoán Nguyên nhân tử vong ghi trên Giấy báo tử, ghi theo hướng dẫn tại Quyết định số **1921/QĐ-BYT** ngày 12/07/2022 của Bộ Y tế|
|26|NGUOI_THANTHICH  |x       |Chuỗi       |255         |Người thân thích trên giấy báo tử, tự điền|
|27|NGUOI_GHIGIAY    |x       |Chuỗi       |255         |Người lập phiếu trên giấy báo tử, tự điền|
|28|TTRUONG_DVI      |x       |Chuỗi       |255         |Thủ trưởng cơ sở khám chữa bệnh kí giấy báo tử, tự điền|
|29|SO_BAOTU         |x       |Chuỗi       |255         |Số giấy báo tử (Số này có giống số trong mục 1 hay không? hỏi lại)|
|30|QUYEN_SO         |x       |Chuỗi       |50          |Quyển số mấy|
|31|NGAY_CAPGIAYBT   |x       |Chuỗi       |8           |Ngày cấp giấy báo tử, định dạng **yyyyMMdd**, sổ xuống ghi|
|32|SO_BAOTU_BD      |        |Chuỗi       |250         |Số giấy báo tử cấp lần đầu (nếu có)|  
|33|QUYEN_SO_BD      |        |Chuỗi       |50          |Quyển số báo tử cấp lần đầu (nếu có)|
|34|MACSKCB          |x       |Chuỗi       |5           |Mã cơ sở khám bệnh, chữa bệnh nơi bệnh nhân tử vong theo danh mục quy định của Bộ y tế|
|35|DIACHI_CSKCB     |x       |Chuỗi       |255         |Địa chỉ Cơ sở khám chữa bệnh|

- Mục 34 và 35 không thấy nằm ở đâu?
