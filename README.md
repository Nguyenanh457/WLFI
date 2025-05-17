WLFI
world liberty financial
// SPDX-Mã định danh giấy phép: MIT

pragma độ rắn ^0.8.20;

nhập nhập nhập "@openzeppelin/contracts/access/Ownab "@openzeppelin/contracts/token/ERC20/

// Hợp đồng bổ sung để quản lý giá và khóa t

hợp đồng WLFIManagement có thể sở hữu {

// Địa chỉ hợp đồng WLFI gốc trên Ethere

IERC20 công khai wlfiToken = IERC20(0xdA5e1

// Danh sách giá dự toán (1.5 USD đến 7

uint256[] bảng giá công khai;

// Thông tin khóa token cho các ví lớn

cấu trúc LockInfo {

số lượng uint256;

// Số lượng to

uint256 khóaCho đến khi;

// Thời gian m

}

// Mapping lưu trữ thông tin khóa token mapping(address => LockInfo) public lock

// Danh sách các ví lớn được quản trị vi address[] public largeWallets;

D để quy đổi giá dự toán từ USD sang ETH

.001 ETH, 5 đô la Mỹ = 0,001667 ETH, 7 đô la Mỹ = 0,002

10^18 vi)

// 1,5 đô la Mỹ (~0,0005 ETH)

// 3,0 đô la Mỹ (~0,001 ETH)

// 5,0 đô la Mỹ (~0,001667 ETH)

// 7,0 đô la Mỹ (~0,002333 ETH)

trị bằng ETH)

lượt (uint256[] bộ nhớ) {

lý trên Ethereum

t) public onlyOwner {

địa chỉ ví hợp lệ");

chiều dài; i++) {

llet, "Ví đã được thêm vào");
