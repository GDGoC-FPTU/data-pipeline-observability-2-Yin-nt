# Experiment Report: Data Quality Impact on AI Agent

**Student ID:** AI20K-2A202600645
**Name:** Nguyen Thi Yen
**Date:** 2026-06-10

## 1. Ket qua thi nghiem

| Scenario | Agent Response | Accuracy (1-10) | Notes |
|----------|----------------|-----------------|-------|
| Clean Data (`processed_data.csv`) | Agent chon Laptop gia $1200 | 10 | Du lieu da duoc validate va chuan hoa |
| Garbage Data (`garbage_data.csv`) | Agent chon Nuclear Reactor gia $999999 | 1 | Outlier khong hop ly lam sai ket qua |

## 2. Phan tich & nhan xet

### Tai sao Agent tra loi sai khi dung Garbage Data?

Agent chi tim san pham electronics co gia cao nhat, nen outlier Nuclear Reactor
gia 999999 trong Garbage Data duoc xem la lua chon tot nhat du khong phu hop voi
nhu cau mua sam thong thuong. Duplicate ID lam danh tinh ban ghi khong con dang
tin cay. Gia sai kieu nhu "ten dollars" co the gay loi khi tinh toan, con gia tri
null lam thieu thong tin can thiet de loc du lieu. Vi agent tin truc tiep vao
knowledge base, cac van de chat luong nay dan den cau tra loi sai hoac loi xu ly.
Pipeline validate va transform giup loai ban ghi khong hop le, chuan hoa category
va tao du lieu nhat quan truoc khi agent su dung.

## 3. Ket luan

**Quality Data > Quality Prompt?** Dong y. Prompt ro rang khong the bu dap cho
outlier, du lieu thieu hay sai kieu; agent van se suy luan dua tren dau vao sai.
