# blockchain_ungdung
# Blockchain Ung Dung Challenges

Danh sách các dự án thực hành trong kho này:
- `challenge-decentralized-staking`
- `challenge-dex`
- `challenge-dice-game`
- `challenge-over-collateralized-lending`
- `challenge-stablecoins`
- `challenge-token-vendor`
- `challenge-tokenization`

## Hướng dẫn chạy (How to run)

Các dự án này đều sử dụng cấu trúc tương tự (Scaffold-ETH). Dưới đây là các bước để chạy môi trường phát triển local:

### 1. Cài đặt
Trước tiên, hãy đảm bảo bạn đã cài đặt NodeJS và Yarn. Sau đó truy cập vào thư mục của dự án bạn muốn chạy và cài đặt các gói phụ thuộc:

```bash
cd <tên-thư-mục-dự-án>
# Ví dụ:
# cd challenge-decentralized-staking

yarn install
```

### 2. Chạy ứng dụng
Để chạy đầy đủ ứng dụng (Blockchain + Backend + Frontend), bạn cần mở 3 cửa sổ Terminal riêng biệt:

**Terminal 1: Khởi chạy Blockchain local**
```bash
yarn chain
```

**Terminal 2: Deploy Smart Contracts**
(Chạy lệnh này sau khi `yarn chain` đã khởi động thành công)
```bash
yarn deploy
```

**Terminal 3: Chạy giao diện Web (Frontend)**
```bash
yarn start
```
Truy cập ứng dụng tại `http://localhost:3000`.

## Kiểm tra (Testing)

Để kiểm tra các logic của Smart Contracts, hãy sử dụng lệnh kiểm thử sau (đây là cách chính để verify bài làm):

```bash
yarn test
```
