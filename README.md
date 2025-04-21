# 2206010_PrakAI_CF-Fuzzy

Komentar Perubahan
CF :
Saat menambahkan 5 gejala baru nilai CF nya berubah menjadi lebih tinggi jika pada dan gejala sesuai. Saat mengubah demam menjadi 0.2 pada gejala user maka, nilai CF akan menurun karena tidak mendekati dengan nilai pada pengetahuan pakar.

Fuzzy :
Suhu 22°C masuk kategori "dingin" (nilai keanggotaan tinggi)
Kelembapan 75% masuk kategori "lembab" (juga tinggi)
Dua aturan relevan akan aktif:
rule3: dingin OR lembab → kipas tinggi
rule10: dingin AND lembab → kipas rendah
Karena aturan rule3 pakai OR (lebih longgar) dan rule10 pakai AND (lebih ketat), maka hasil akhirnya adalah kombinasi dari dua output fuzzy:
Sedikit kontribusi dari "rendah"
Kontribusi dari "tinggi"
Fuzzy logic akan defuzzify (mengubah fuzzy ke nilai crisp), dan memberikan output kecepatan kipas yang kompromi.
