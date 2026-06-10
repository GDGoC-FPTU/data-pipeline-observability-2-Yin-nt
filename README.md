# Day 10 Lab: Data Pipeline & Data Observability

**Student ID:** AI20K-2A202600645
**Name:** Nguyen Thi Yen

## Mo ta

Xay dung ETL pipeline doc JSON, loai du lieu khong hop le, chuan hoa category,
tinh gia giam 10%, them timestamp quan sat va luu ket qua ra CSV. Bai lab cung
so sanh tac dong cua clean data va garbage data len AI agent.

## Cach chay

```bash
pip install pandas pytest
python solution.py
python generate_garbage.py
python agent_simulation.py
pytest -q
```

## Cau truc thu muc

- `solution.py`: ETL pipeline
- `processed_data.csv`: output cua pipeline
- `experiment_report.md`: bao cao stress test
- `agent_simulation.py`: mo phong agent

## Ket qua

Pipeline doc 5 records, giu lai 3 records hop le va loai 2 records loi. Clean
data giup agent chon Laptop; garbage data khien agent chon outlier Nuclear Reactor.
