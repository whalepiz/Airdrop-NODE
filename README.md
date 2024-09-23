# Hemi Miner Incentivized Testnet

![image](https://github.com/user-attachments/assets/996c7d95-8be3-457b-a920-270fc337c6e1)
> HHemi là Giao thức Bitcoin-Ethereum Modular, Hemi Labs đã huy động được 15 triệu đô la trong vòng gọi vốn Seed do Binance Labs Fund dẫn đầu.
 
#

* Đối với các bạn không chạy Node, thì có thể tham gia chương trình kiếm  Point [TRUY CẬP](https://points.absinthe.network/hemi/) : Nhập mã giới thiệu: `2c19e0ca`
* Bạn cũng có thể Miner  bằng trình duyệt web trên Windows tại đây:: https://pop-miner.hemi.xyz/

## Cài đặt Miner trên Linux
**1. Download Binaries**
```bash
wget https://github.com/hemilabs/heminetwork/releases/download/v0.4.3/heminetwork_v0.4.3_linux_amd64.tar.gz
```

**2. Extract Binaries**
```bash
tar -xvf heminetwork_v0.4.3_linux_amd64.tar.gz && rm heminetwork_v0.4.3_linux_amd64.tar.gz && cd heminetwork_v0.4.3_linux_amd64
```

## Wallet
**1. Tạo ví tBTC**
```bash
./keygen -secp256k1 -json -net="testnet" > ~/popm-address.json
```

**2. Lấy thông tin ví tBTC**
```bash
cat $HOME/popm-address.json
```
* Lưu lại thông Wallet
* `pubkey_hash` là địa chỉ tBTC của bạn
* `private_key` là để bạn có thể nhập ví vào Metamask

**3. Nạp tBTC vào ví**
* Các bạn vào Discord Faucet nhé [Discord](https://discord.gg/hemixyz) 
* Kiểm tra tBTC đã vào ví chưa rồi làm bước tiếp theo

## Khởi chạy Miner
*Tạo screen 
```bash
screen -S hemi
```

```bash
export POPM_BTC_PRIVKEY= nhập private_key của bạn
export POPM_STATIC_FEE=50
export POPM_BFG_URL=wss://testnet.rpc.hemi.network/v1/ws/public
./popmd
```

**. Node hoạt động**


![image](https://github.com/user-attachments/assets/76dc9867-a0b3-4d11-9baf-cd1d5a94f695)



# Kiểm tra points
*  Hiện tại, khoản thanh toán token tHEMI đóng vai trò là điểm khai thác Hemi PoP. Bạn sẽ nhận được token tHEMI cho mỗi khối bạn khai thác bằng Hemi Pop Node của mình
*  Để xem số dư tHEMI của bạn, bạn có thể cần thêm địa chỉ hợp đồng 0x4200000000000000000000000000000000000042dưới dạng "mã thông báo tùy chỉnh" vào ví metamask của mình trên Mạng Hemi Sepolia.
*  Bạn cũng có thể nhập private_keysố dư tHEMI tại đây để kiểm tra: https://pop-miner.hemi.xyz/
   Việc đạt được tHEMI bị trì hoãn ngay bây giờ, bạn có thể kiểm tra sau
