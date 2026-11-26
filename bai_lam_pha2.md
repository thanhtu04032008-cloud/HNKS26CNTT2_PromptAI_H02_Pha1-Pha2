# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 05
- **Họ tên:** Lê Đặng Thanh Tú
- **Lớp:** CNTT2
- **Link repository Pha2:** https://github.com/thanhtu04032008-cloud/HNKS26CNTT2_PromptAI_H02_Pha1-Pha2.git
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt vé xem phim ra JSON

**KET QUA AI**

```text
[\
&#x20; {\
&#x20;   "loai_ve": "P2D",\
&#x20;   "ngay_chieu": "2026-12-24",\
&#x20;   "ve_nguoi_lon": 2,\
&#x20;   "ve_tre_em": 1,\
&#x20;   "loai_ghe": "thuong",\
&#x20;   "ghi_chu": null\
&#x20; },\
&#x20; {\
&#x20;   "loai_ve": "P3D",\
&#x20;   "ngay_chieu": "2027-01-01",\
&#x20;   "ve_nguoi_lon": 3,\
&#x20;   "ve_tre_em": 0,\
&#x20;   "loai_ghe": null,\
&#x20;   "ghi_chu": "1 người hay chóng mặt, cần ngồi gần lối ra"\
&#x20; },\
&#x20; {\
&#x20;   "loai_ve": "GOLD",\
&#x20;   "ngay_chieu": null,\
&#x20;   "ve_nguoi_lon": 4,\
&#x20;   "ve_tre_em": 0,\
&#x20;   "loai_ghe": "doi",\
&#x20;   "ghi_chu": "1 bạn đi xe lăn"\
&#x20; }\
]
```

**Link trò chuyện:** https://chatgpt.com/share/6b079e20-fb00-83ec-933c-6452af5e9862

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
**1. Tiền người lớn**

- Số lượng: 5 người.
- Giá vé P3D: 130.000 đồng/vé.

Phép tính:

\\(5 \times 130.000 = 650.000\\) đồng.

**2. Tiền trẻ em**

Trẻ em cao từ 1 m đến 1,3 m được tính bằng 70% giá vé người lớn.

\- Trẻ cao 1,1 m:

\\(130.000 \times 70\\% = 91.000\\) đồng.

\- Trẻ cao 1,25 m:

\\(130.000 \times 70\\% = 91.000\\) đồng.

\- Bé cao 0,9 m: Dưới 1 m, ngồi cùng người lớn nên được miễn phí.

Tổng tiền trẻ em:

\\(91.000 + 91.000 + 0 = 182.000\\) đồng.

**3. Tiền vé trước giảm giá**

Tiền vé trước giảm = Tiền người lớn + Tiền trẻ em.

\\(650.000 + 182.000 = 832.000\\) đồng.

**4. Mức giảm giá nhóm và tiền vé sau giảm**

Nhóm có 5 người lớn, đủ điều kiện giảm 10% trên tổng tiền vé người lớn và trẻ em.

\- Mức giảm:

\\(832.000 \times 10\\% = 83.200\\) đồng.

\- Tiền vé sau giảm:

\\(832.000 - 83.200 = 748.800\\) đồng.

**5. Phụ thu khu ghế ưu tiên**

Dữ liệu không quy định phụ thu khu ghế ưu tiên.

Vì vậy, không có khoản phụ thu này trong phép tính: **0 đồng**.

**6. Tổng tiền phải trả**

- Tiền vé sau giảm: 748.800 đồng.
- Tiền 3 combo: \\(3 \times 75.000 = 225.000\\) đồng.
- Combo không được giảm giá.

Tổng tiền:

\\(748.800 + 225.000 + 0 = 973.800\\) đồng.

Tổng thanh toán: 973.800 đồng

[RESULT: 973800 đồng]
```

**Link trò chuyện:** https://chatgpt.com/share/6b079e87-d5f0-83ec-ac68-d6d10f77f230

### b) Kiểm tra kết quả AI

Kết quả đúng. Các bước áp dụng đúng giá P3D, mức 70% cho trẻ 1,1m và 1,25m, miễn phí cho trẻ 0,9m, giảm 10% trên tiền vé vì nhóm có đủ 5 người lớn, và cộng phụ thu 225.000 đồng không giảm giá. Tổng đúng là **973.800 đồng**

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{\
&#x20; "loai_su_co": "loi_ky_thuat",\
&#x20; "so_khach": 4,\
&#x20; "so_suat_bi_loi": 2,\
&#x20; "tom_tat": "4 khách, 2 suất liên tiếp tại phòng 3 đều mất tiếng hơn 15 phút giữa phim."\
}
```

**Link trò chuyện:** https://chatgpt.com/share/6b07a01e-f548-83ec-83da-0ac06fbe0d99

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí | Điểm | Minh chứng | Đề xuất sửa |
| -------- | ---- | ---------- | ----------- |

\| **Đúng thông tin (50%)** | **0/5** | **Sai cả hai nội dung:**
```

**Link trò chuyện:** https://chatgpt.com/share/6b07a056-a428-83ec-8e67-8b5f0217109d
