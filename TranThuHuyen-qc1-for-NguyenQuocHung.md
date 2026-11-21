# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên): Nguyen Quoc Hung    Người kiểm (học viên): Trần Thu Huyền  
Ngày: 21/11/2026    Phiên bản guideline: Road v1.0  
File được kiểm: `NguyenQuocHung-front.zip`, `NguyenQuocHung-fisheye.zip` (không có manifest)  
Số ảnh kiểm: 6 (A05–A09, B04)    Số nhãn đã xem (shape + tag): 90

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | 6 | 0 | nặng |
| QC1-02 đủ L1, R1 | bỏ sót | 12 | 0 xác nhận (4 chờ lead) | nặng |
| QC1-03 position | sai thuộc tính / thừa | 10 | 0 phát hiện | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | 10 | 0 phát hiện | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | 10 | 0 phát hiện | chính |
| QC1-06 style, color, kind | sai thuộc tính | 10 | 0 phát hiện | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | 25 | 0 phát hiện | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | 21 | 0 phát hiện | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | 31 | 0 phát hiện | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | 10 | 0 phát hiện | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | 5 | 1 | chính |
| QC1-12 file | lỗi file | 2 ZIP | 0 | nhẹ / nặng |

## Danh sách lỗi / điểm cần xác nhận
| # | Mã | Ảnh | Nhãn (label, vị trí) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1 | QC1-02 | A06 | lane, thiếu R1 | nặng* | Lint báo thiếu; xác nhận vạch R1 có nhìn thấy và phân biệt được với mép đường không. |
| 2 | QC1-02 | A07 | lane, thiếu L1 | nặng* | Lint báo thiếu; xác nhận vạch L1 có nhìn thấy không. |
| 3 | QC1-02 | A08 | lane, thiếu L1 | nặng* | Lint báo thiếu; xác nhận vạch L1 có nhìn thấy không. |
| 4 | QC1-02 | A09 | lane, thiếu R1 | nặng* | Lint báo thiếu; xác nhận vạch R1 có nhìn thấy không. |
| 5 | QC1-11 | B04 | traffic_sign, tâm box khoảng (1064,172) | chính | `edge_zone=false`; tâm box vượt ngưỡng 80% bán kính, cần bật edge_zone. |

* Bốn mục QC1-02 người kiểm (Trần Thu Huyền) cần đối chiếu ảnh gốc; nếu còn mơ hồ thì hỏi coach/giảng viên trước khi chốt là lỗi nặng. A05 cũng bị lint báo thiếu L1/R1 nhưng ảnh không thấy vạch sơn nên không tính lỗi. Box dưới 8 px ở A03/A07/A10 không bắt buộc, không tính lỗi.

## Ca mơ hồ
| Ảnh | Câu hỏi cho coach/giảng viên | Lời đáp của coach/giảng viên (nếu có) |
| --- | --- | --- |
| A06, A07, A08, A09 | Các vạch L1/R1 bị lint báo thiếu có nhìn thấy rõ để bắt buộc gán không? | Chờ xác nhận |

## Quyết định
Lỗi nặng đã xác nhận: 0; QC1-02 chờ xác nhận: 4. Lỗi chính đã xác nhận: 1 / 90 = 1.1%. Lỗi nhẹ: 0. Ca chờ coach/giảng viên: 4.  
Quyết định: Chưa chốt. Người kiểm (Trần Thu Huyền) đối chiếu ảnh gốc; vẫn mơ hồ và hỏi coach/giảng viên. Chỉ ghi Hold khi đã hỏi và đang chờ phản hồi.
