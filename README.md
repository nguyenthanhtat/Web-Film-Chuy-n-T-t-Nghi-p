
## Web Online: https://movienetflixttn.herokuapp.com/

## 1. API dành cho admin

## Admin:

- Đăng ký tài khoản admin: post --> http://localhost:5000/api/auth/admin/register

- Xác thực email đăng ký: get --> http://localhost:5000/api/auth/admin/verify/:userId/:uniqueString

- Đăng nhập tài khoản admin: post --> http://localhost:5000/api/auth/admin/login

- Đăng xuất tài khoản: get --> http://localhost:5000/api/auth/admin/logout

- Xem profile: get --> http://localhost:5000/api/auth/admin/profile

- Chỉnh sửa profile: patch --> http://localhost:5000/api/auth/admin/profile/update

- Refresh token : get --> http://localhost:5000/api/auth/admin/refresh_token

- Thay đổi mật khẩu : patch --> http://localhost:5000/api/auth/admin/changePassword

- Quên mật khẩu tài khoản admin: post --> http://localhost:5000/api/auth/admin/forget

- Link reset mật khẩu khi quên: put --> http://localhost:5000/api/auth/admin/password/reset/:token

- Đăng nhập google tài khoản admin: post --> http://localhost:5000/api/auth/admin/loginGoogle

- Danh sách tài khoản admin: get --> http://localhost:5000/api/auth/admin/getAllAdmin

- Danh sách tài khoản khách hàng: get --> http://localhost:5000/api/auth/admin/getAllCustomer

- Xem chi tiết tài khoản khách hàng: get --> http://localhost:5000/api/auth/admin/getDetailCustomer/:id

- Chỉnh sửa thông tin tài khoản khách hàng: patch --> http://localhost:5000/api/auth/admin/customerAccount/:id/update/info

- Danh sách khách hàng chưa check email đăng ký: get --> http://localhost:5000/api/auth/admin/getAllCustomerUncheck

## Upload:

- Upload ảnh người dùng : post --> http://localhost:5000/api/uploadImageUser

- Xóa ảnh người dùng trên cloud : post --> http://localhost:5000/api/destroyImageUser

- Upload video phim : post --> http://localhost:5000/api/uploadVideoFilm

- Xóa video phim trên cloud : post --> http://localhost:5000/api/destroyVideoFilm

- Upload ảnh đạo diễn : post --> http://localhost:5000/api/uploadImageDirector

- Xóa ảnh đạo diễn trên cloud : post --> http://localhost:5000/api/destroyImageDirector

- Upload ảnh phim : post --> http://localhost:5000/api/uploadImageFilm

- Xóa ảnh phim : post --> http://localhost:5000/api/destroyImageFilm

- Upload ảnh hình thức thanh toán : post --> http://localhost:5000/api/uploadImagePayment

- Xóa ảnh hình thức thanh toán : post --> http://localhost:5000/api/destroyImagePayment

## Director:

- Xem thông tin tất cả đạo diễn: get --> http://localhost:5000/api/director/all

- Xem thông tin chi tiết đạo diễn: get --> http://localhost:5000/api/director/:id

- Thêm mới thông tin đạo diễn : post --> http://localhost:5000/api/director/add

- Chỉnh sửa thông tin đạo diễn : patch --> http://localhost:5000/api/director/update/:id

- Xóa thông tin đạo diễn : delete --> http://localhost:5000/api/director/delete/:id

## Category

- Xem tất cả thể loại phim : get --> http://localhost:5000/api/category/all

- Tạo thêm 1 thể loại phim: post --> http://localhost:5000/api/category/add

- Cập nhập thể loại phim: put --> http://localhost:5000/api/category/update/:id

- Xóa thể loại phim: delete --> http://localhost:5000/api/category/delete/:id

## Film

- Xem thông tin tất cả bộ phim: get --> http://localhost:5000/api/film/all

- Thêm thông tin bộ phim: post --> http://localhost:5000/api/film/add

- Chỉnh sửa thông tin bộ phim: patch --> http://localhost:5000/api/film/update/:id

- Xóa bộ phim : delete --> http://localhost:5000/api/film/delete/:id

- Thông tin chi tiết của bộ phim và thông tin đánh giá của bộ phim: get --> http://localhost:5000/api/film/detail/:id

- Tìm bộ phim theo đạo diễn: get --> http://localhost:5000/api/film/find/director/:id

- Thêm một tập phim: post --> http://localhost:5000/api/film/:id/addEpisode

- Cập nhập tập phim: patch --> http://localhost:5000/api/film/update/:filmId/updateEpisode/:episodeId

- Xóa 1 tập phim: delete --> http://localhost:5000/api/film/delete/:filmId/deleteEpisode/:episodeId

- Danh sách phim tìm theo categoryId: get --> http://localhost:5000/api/film/find/category/:categoryId

## Favourite

- Xem danh sách yêu thích của toàn bộ người dùng: get --> http://localhost:5000/api/favourite/all

## Rating

- Xem đánh giá của toàn bộ người dùng: get --> http://localhost:5000/api/rating/all

## Comment

- Xem tất cả bình luận: get --> http://localhost:5000/api/comment/all

- Xem bình luận của bộ phim: get --> http://localhost:5000/api/comment/get/:filmId

- Lấy thùng rác chứa những bình luận đã bị xóa: get --> http//localhost:5000/api/comment/bin

- Khôi phục lại comment đã bị xóa: patch --> http://localhost:5000/api/comment/:id/restore

- Xóa hẳn comment nếu ở trong thùng rác quá 7 ngày: delete --> http://localhost:5000/api/comment/bin/delete

## Payment

- Xem tất cả hình thức thanh toán: get --> http://localhost:5000/api/modeOfPayment/all

- Xem chi tiết hình thức thanh toán: get --> http://localhost:5000/api/modeOfPayment/:id

- Thêm hình thức thanh toán mới: post --> http://localhost:5000/api/modeOfPayment/add

- Chỉnh sửa hình thức thanh toán: patch --> http://localhost:5000/api/modeOfPayment/update/:id

- Xóa hình thức thanh toán: delete --> http://localhost:5000/api/modeOfPayment/delete/:id

## Feedback

- Xem tất cả feedback: get --> http://localhost:5000/api/feedback/all

- Trả lời feedback của khách hàng: post --> http://localhost:5000/api/feedback/response/:id

## Bill

- Lấy ra toàn bộ hóa đơn: get -> http://localhost:5000/api/bill/all

- Lấy ra danh sách hóa đơn theo mã khách hàng: get -> http://localhost:5000/api/bill/:userId/listBill

## Statistics

- Thống kê những người dùng đăng ký gần đây (3 ngày) : get -> http://localhost:5000/api/statistics/registeredUser/recently

- Thống kê doanh thu từng tháng: get -> http://localhost:5000/api/statistics/revenue/monthly

## 2. API dành cho khách hàng

## Upload:

- Upload ảnh người dùng : post --> http://localhost:5000/api/uploadImageUser

- Xóa ảnh người dùng trên cloud : post --> http://localhost:5000/api/destroyImageUser

## Customer:

- Đăng ký tài khoản khách hàng: post --> http://localhost:5000/api/auth/customer/register

- Xác thực email đăng ký: get --> http://localhost:5000/api/auth/admin/verify/:userId/:uniqueString

- Đăng nhập tài khoản khách hàng : post --> http://localhost:5000/api/auth/customer/login

- Đăng xuất tài khoản: get --> http://localhost:5000/api/auth/customer/logout

- Xem profile: get --> http://localhost:5000/api/auth/customer/profile

- Chỉnh sửa profile: patch --> http://localhost:5000/api/auth/customer/profile/update

- Refresh token : get --> http://localhost:5000/api/auth/customer/refresh_token

- Thay đổi mật khẩu : patch --> http://localhost:5000/api/auth/customer/changePassword

- Thay đổi mật khẩu mới khi đăng ký bằng email hoặc facebook : patch --> http://localhost:5000/api/auth/customer/newPassword

- Quên mật khẩu tài khoản khách hàng: post --> http://localhost:5000/api/auth/customer/forget

- Link reset mật khẩu khi quên: put --> http://localhost:5000/api/auth/customer/password/reset/:token

- Đăng nhập google tài khoản khách hàng: post --> http://localhost:5000/api/auth/customer/loginGoogle

## Director:

- Xem thông tin tất cả đạo diễn: get -->http://localhost:5000/api/director/all

- Xem thông tin chi tiết đạo diễn: get --> http://localhost:5000/api/director/:id

## Category

- Xem tất cả thể loại phim : get --> http://localhost:5000/api/category/all

## Film

- Lựa chọn phim cho trẻ em hoặc người lớn : post --> http://localhost:5000/api/film/selectForAdultOrChild

- Danh sách phim của người lớn : get --> http://localhost:5000/api/film/adult

- Danh sách phim của trẻ em: get --> http://localhost:5000/api/film/kid

- Thoát khỏi chế độ xem phim cho trẻ em: post --> http://localhost:5000/api/film/kid/exit

- Thông tin chi tiết của bộ phim và thông tin đánh giá của bộ phim: get --> http://localhost:5000/api/film/detail/:id

- Hiển thị toàn bộ phim người lớn theo từng thể loại: get --> http://localhost:5000/api/film/adult/eachCategory

- Hiển thị toàn bộ phim trẻ em theo từng thể loại: get --> http://localhost:5000/api/film/kid/eachCategory

- Tìm bộ phim theo đạo diễn: get --> http://localhost:5000/api/film/find/director/:id

## Favourite

- Xem danh sách yêu thích của người dùng: get --> http://localhost:5000/api/favourite/getList

- Thêm và xóa bộ phim trong danh sách yêu thích: post --> http://localhost:5000/api/favourite/add/:idFilm

- Xóa toàn bộ phim khỏi danh sách yêu thích: delete --> http://localhost:5000/api/favourite/delete/

## Rating

- Đánh giá sao cho bộ phim: post --> http://localhost:5000/api/rating/add/:filmId

## Comment

- Xem bình luận của bộ phim: get --> http://localhost:5000/api/comment/get/:filmId

- Bình luận bộ phim: post --> http://localhost:5000/api/comment/add/:filmId

- Chỉnh sửa bình luận: patch --> http://localhost:5000/api/comment/update/:id

- Xóa mềm bình luận: patch --> http://localhost:5000/api/comment/softDelete/:id

## Payment

- Xem tất cả hình thức thanh toán: get --> http://localhost:5000/api/modeOfPayment/all

- Xem chi tiết hình thức thanh toán: get --> http://localhost:5000/api/modeOfPayment/:id

## Bill

- Xem lịch sử hóa đơn của khách hàng: get --> http://localhost:5000/api/bill/history

- Kiểm tra phim có xem được không: --> http://localhost:5000/api/bill/checkCanWatchFilm/:filmId

- Tạo hóa đơn cho Paypal: --> http://localhost:5000/api/bill/Paypal/create/

## 3. API không cần đăng nhập

## Feedback

- Khách hàng gửi feedback : post --> http://localhost:5000/api/feedback/send
#� �W�e�b�-�F�i�l�m�-�C�h�u�y�-�n�-�T�-�t�-�N�g�h�i�-�p�
�
�
