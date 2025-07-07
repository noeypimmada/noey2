# # รายการของลูปต่าง ๆ
loops = [
    ("range(1, 101)", range(1, 101)),
    ("range(7, 77, 7)", range(7, 77, 7)),
    ("range(20, 1, -2)", range(20, 1, -2)),
    ("range(2, 18, 3)", range(2, 18, 3)),
    ("range(55, 0, -11)", range(55, 0, -11)),
    ("range(1, 0)", range(1, 0)),
]

# ทดสอบแต่ละลูป
for desc, r in loops:
    count = 0
    last_i = None
    for i in r:
        last_i = i
        count += 1

    print(f"ลูป {desc}")
    print(f" → ทำงานทั้งหมด {count} รอบ")
    if count > 0:
        print(f" → ค่าของ i รอบสุดท้ายคือ {last_i}")
    else:
        print(f" → ค่าของ i ไม่มี (ลูปไม่ทำงานเลย)")
    print("-" * 40)
