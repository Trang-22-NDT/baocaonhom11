# 🌾 Hệ thống Truy xuất Nguồn gốc Nông sản - Blockchain

![Version](https://img.shields.io/badge/version-2.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Node](https://img.shields.io/badge/node-%3E%3D14.0.0-brightgreen)

Ứng dụng Blockchain cho chuỗi cung ứng nông sản minh bạch, cho phép truy xuất nguồn gốc từ nông trại đến người tiêu dùng.

## ✨ Tính năng

### 🚜 Cho Nông dân
- ✅ Tạo lô sản phẩm mới
- ✅ Ghi nhận hoạt động chăm sóc (tưới tiêu, bón phân, phun thuốc)
- ✅ Ghi nhận thu hoạch với thông tin số lượng và chất lượng

### 🏭 Cho Doanh nghiệp
- ✅ Kiểm định chất lượng sản phẩm
- ✅ Ghi nhận đóng gói với các loại bao bì khác nhau

### 🚚 Cho Vận chuyển
- ✅ Theo dõi vận chuyển với thông tin nhiệt độ
- ✅ Ghi nhận thời gian xuất phát và đến

### 🏪 Cho Siêu thị
- ✅ Quản lý nhập/xuất kho
- ✅ Theo dõi tình trạng sản phẩm

### 💳 Thanh toán
- ✅ Tạo mã QR thanh toán ngân hàng
- ✅ Ghi nhận giao dịch thanh toán
- ✅ Xem lịch sử thanh toán theo lô

### 👤 Cho Người tiêu dùng
- ✅ Truy xuất nguồn gốc đầy đủ
- ✅ Quét mã QR để xem thông tin sản phẩm
- ✅ Xem timeline đầy đủ từ nông trại đến tay

### 📊 Quản lý
- ✅ Dashboard thống kê
- ✅ Danh sách tất cả lô sản phẩm
- ✅ Kiểm tra tính toàn vẹn blockchain

## 🎨 Giao diện mới (v2.0)

### Cải tiến UI/UX:
- ✨ Modern design với gradient backgrounds
- 🎯 Toast notification system
- ⏳ Loading states cho tất cả actions
- 📱 Fully responsive design
- 🎭 Smooth animations và transitions
- 🌈 CSS Variables design system
- ⚡ Better error handling
- 🔔 Real-time feedback

### Components mới:
- 💬 Toast notifications
- 📊 Stats cards với hover effects
- 🔄 Loading spinners
- ⏱️ Beautiful timeline for traceability
- 🎨 Card hover effects
- 📱 Mobile-first responsive design

## 🚀 Cài đặt

### Yêu cầu
- Node.js >= 14.0.0
- npm >= 6.0.0

### Bước 1: Clone repository
```bash
git clone https://github.com/Trang-22-NDT/baocaonhom11.git
cd baocaonhom11
```

### Bước 2: Cài đặt dependencies
```bash
cd backend
npm install
```

### Bước 3: Chạy server
```bash
npm start
# hoặc với nodemon
npm run dev
```

Server sẽ chạy tại: http://localhost:3000

## 📁 Cấu trúc dự án

```
baocaonhom11/
├── backend/
│   ├── blockchain.js      # Blockchain logic
│   ├── server.js          # Express server & API
│   └── package.json       
├── frontend/
│   ├── index.html         # Main UI
│   ├── trace.html         # Traceability page
│   ├── app.js             # Frontend logic
│   └── styles.css         # Modern CSS
├── database/
│   └── chain.json         # Blockchain storage
└── README.md
```

## 🔌 API Endpoints

### Nông dân
- `POST /api/batch` - Tạo lô sản phẩm
- `POST /api/farming/:batchId` - Ghi nhận chăm sóc
- `POST /api/harvest/:batchId` - Ghi nhận thu hoạch

### Doanh nghiệp
- `POST /api/quality/:batchId` - Kiểm định chất lượng
- `POST /api/packaging/:batchId` - Đóng gói

### Vận chuyển & Kho
- `POST /api/transport/:batchId` - Vận chuyển
- `POST /api/warehouse/:batchId` - Nhập/Xuất kho

### Thanh toán
- `POST /api/payment/:batchId` - Ghi nhận thanh toán
- `POST /api/payment/qrcode/:batchId` - Tạo QR thanh toán
- `GET /api/payment/:batchId` - Lịch sử thanh toán

### Truy xuất
- `GET /api/batch/:batchId` - Lấy lịch sử đầy đủ
- `GET /api/qrcode/:batchId` - Tạo QR truy xuất

### Quản lý
- `GET /api/batches` - Danh sách tất cả lô
- `GET /api/statistics` - Thống kê hệ thống
- `GET /api/validate` - Kiểm tra blockchain

## 💻 Công nghệ sử dụng

### Backend
- Node.js
- Express.js
- SHA256 (crypto-js)
- QRCode

### Frontend
- HTML5
- CSS3 (Modern CSS Variables)
- Vanilla JavaScript
- Fetch API

### Blockchain
- Custom implementation
- Proof of Work (PoW)
- SHA-256 hashing
- Immutable ledger

## 🎯 Workflow

```
1. Nông dân tạo lô → Ghi nhận chăm sóc → Thu hoạch
                                ↓
2. Doanh nghiệp kiểm định → Đóng gói
                                ↓
3. Vận chuyển → Nhập kho siêu thị
                                ↓
4. Khách hàng mua → Thanh toán → Quét QR truy xuất
```

## 🔒 Bảo mật

- ✅ Blockchain immutability
- ✅ Hash verification
- ✅ Tamper-proof records
- ✅ Full audit trail
- ✅ Decentralized verification

## 📸 Screenshots

### Dashboard
![Dashboard](https://via.placeholder.com/800x400?text=Dashboard+Screenshot)

### Traceability Timeline
![Timeline](https://via.placeholder.com/800x400?text=Timeline+Screenshot)

### QR Code
![QR](https://via.placeholder.com/400x400?text=QR+Code)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License.

## 👥 Team

- **Nhóm 11** - Báo cáo môn học
- **GitHub**: [Trang-22-NDT](https://github.com/Trang-22-NDT)

## 📧 Contact

For questions or support, please open an issue on GitHub.

---

**Made with ❤️ using Blockchain Technology**

**Last Updated**: January 29, 2026
