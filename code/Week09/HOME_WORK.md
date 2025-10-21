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
0c79b42c32b6dcdf12c154a29ef90e81b52ff63626db9c871cacbc6525c4c89e
```

### S2: Deploy Oracle , with ADA price = 1$
```

```

### S3: Owner deloy Scripts, minimum ratio = 150%
```

```

### S4: User 1 mint 10 stablecoin , collateral 15 ADA
```

```

### S5: User 1 burn 10 stablecoin, no change ADA price
```

```

## Yêu cầu nâng cao
> User 1 mint 10 stablecoin ( collateral 15 ADA) , User 2 mint 50 stablecoint (collateral 100 ADA) , Ada price down to 0.9, then User2 liquite 10 stablecoin of user 1

### S6: User 1 mint 10 stablecoin ( collateral 15 ADA)
```

```

### S7: User 2 mint 50 stablecoint (collateral 100 ADA)
```

```

### S8: Update Ada Price to 0.9$
```

```

### S9: User 2 liqute colateral UTxO of user 1
```

```