# Homework assignment 05

## Yêu cầu cơ bản (đạt mức điểm B)
- Thực hiện các thao tác: **mint**, **burn**, **liquidity** (stablecoin) giống demo.
- Ghi lại TxHash của các giao dịch vào file `HOME_WORK.md`.

## Yêu cầu nâng cao (đạt mức điểm A)
Push phần code thay đổi lên repo và ghi lại kết quả (TxHash) vào file `HOME_WORK.md`. Thực hiện 2 nâng cấp sau:

1. Giảm rủi ro thanh lý (Liquidation risk)
    - Vấn đề: Khi giá trị tài sản thế chấp giảm dưới ngưỡng, người dùng mất toàn bộ phần dư thừa (50% collateral) và phần này hoàn toàn thuộc về liquidator — gây thiệt hại lớn cho người dùng.
    - Yêu cầu cải thiện: 
      - Giới hạn phần thưởng cho liquidator ở mức tối đa **2%** của giá trị dư thừa.
      - Phần dư thừa vượt quá 2% phải **trả lại cho chủ sở hữu ban đầu**.

2. Thêm phí cho nhà phát triển (Developer fee)
    - Vấn đề: Hiện tại hệ thống không trả phí cho nhà phát triển; chỉ liquidator được hưởng.
    - Yêu cầu cải thiện:
      - Áp dụng một khoản phí nhỏ **0.1%** khi thực hiện các hành động: **mint**, **burn**, **liquidate**.
      - Phí này chuyển về địa chỉ developer để hỗ trợ bảo trì và phát triển.

---
# Kết quả

## Yêu cầu cơ bản

### Mint Oracle's NFT
```
7b1262e3ec743b364b915e273248da7a9881b3b9138ec403bbe5e351104aaf9b
```

### S2: Deploy Oracle
```
b2a8c75ad60ffbae4a578ff1039fd3d741964d64d73a9d65d74765a6ba8329b5
```

### S3: Owner deploy Scripts
```
bb20099eeec6192eeb66168bca6752ed6e95c93ca30804178efe99c467ae88dd
```

### S4: User mint 10 USDP
```
a48c7ac978adde9324e763cc107aa6d1b8675303b89b6a848bfa42ab929e5f64 
```

### S5: User burn 10 USDP
```
cd293094fcb753f3ea34f5d807b63c05f62c06607faeaaa48941e71030f72e22
```

### S6: User 1 mint 10 stable coin usdp
```
ce2aa140f188db2e792282af97a7d5a8f75578d1c5e9d2b227aaf59ec0c47087
```

### S7: User 2 mint 5 stable coin usdp
```
7049169580002ca9bb1dc75ce5630b4eba7331c849801bdf73d586f86048a58d
```

### S8: Oracle update price down to 0.9 = 90 cent
```
cb3a885298efae9aa60d8856fa7e4eb34a4eadb6706be2afa466ef5d0d023c70
```

### S9: User 2 liquite utxo user 1
```
48ca6c8229ef2d022a86fd52abeb145c410cc99d1f2952a289ec77eec1b2bb81
```