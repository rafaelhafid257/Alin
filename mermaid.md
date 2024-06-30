<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flowchart dengan Mermaid</title>
    <script type="module">
        import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@9.1.1/dist/mermaid.esm.min.mjs';
        document.addEventListener('DOMContentLoaded', function() {
            mermaid.initialize({ startOnLoad: true });
        });
    </script>
</head>
<body>
    <div class="mermaid">
        graph TD;
        Start --> |User Menentukan| Stasiun_Keberangkatan;
        Stasiun_Keberangkatan --> |User Memilih| Stasiun_Tujuan;
        Stasiun_Tujuan --> |User Menentukan| Tanggal_Keberangkatan;
        Tanggal_Keberangkatan --> |User Menentukan| Jam_Keberangkatan;
        Jam_Keberangkatan --> |User Menentukan| Jumlah_Tiket;
        Jumlah_Tiket --> Selesai;
    </div>
</body>
</html>
