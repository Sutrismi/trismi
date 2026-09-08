<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes" />
    <title>Lumpia Kukus Kuah Korea 🇰🇷</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700;800;900&display=swap" rel="stylesheet" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" />
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: #faf0ed;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            padding: 16px 12px 30px;
        }

        .container {
            max-width: 480px;
            width: 100%;
            background: #ffffff;
            border-radius: 40px 40px 28px 28px;
            box-shadow: 0 20px 60px rgba(180, 50, 30, 0.15);
            overflow: hidden;
            padding: 22px 20px 30px;
            border: 1px solid rgba(200, 70, 50, 0.12);
            position: relative;
        }

        .text-red {
            color: #c0392b;
        }
        .bg-red-soft {
            background: #fce8e5;
        }
        .border-red {
            border-color: #e6b8b0;
        }

        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 14px;
        }
        .header h1 {
            font-size: 1.6rem;
            font-weight: 800;
            color: #a62c24;
            line-height: 1.2;
            letter-spacing: -0.5px;
        }
        .header h1 small {
            display: block;
            font-size: 0.7rem;
            font-weight: 400;
            color: #7a4a3e;
            letter-spacing: 0.3px;
            margin-top: 2px;
        }
        .badge-flag {
            background: #fff5f2;
            padding: 6px 14px;
            border-radius: 60px;
            border: 1px solid #f0cdc4;
            font-size: 0.8rem;
            font-weight: 600;
            color: #b5312a;
            display: flex;
            align-items: center;
            gap: 6px;
            white-space: nowrap;
        }
        .badge-flag i {
            color: #d43f31;
        }

        .carousel {
            display: flex;
            gap: 12px;
            overflow-x: auto;
            padding: 10px 0 16px;
            scrollbar-width: thin;
            scrollbar-color: #d67a6b #f7e3df;
            -webkit-overflow-scrolling: touch;
        }
        .carousel::-webkit-scrollbar {
            height: 4px;
        }
        .carousel::-webkit-scrollbar-thumb {
            background: #d67a6b;
            border-radius: 20px;
        }
        .carousel-item {
            flex: 0 0 120px;
            background: white;
            border-radius: 28px;
            padding: 10px 8px 10px;
            box-shadow: 0 4px 12px rgba(190, 70, 50, 0.08);
            border: 1px solid #fad7ce;
            text-align: center;
        }
        .carousel-item img {
            width: 100%;
            aspect-ratio: 1/1;
            object-fit: cover;
            border-radius: 40px;
            background: #fceae7;
            display: block;
            margin-bottom: 4px;
            border: 2px solid #fff;
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.04);
        }
        .carousel-item span {
            font-weight: 600;
            font-size: 0.7rem;
            color: #4d2c22;
            display: block;
        }

        .produk-utama {
            background: linear-gradient(145deg, #fff7f4, #fdeeea);
            border-radius: 48px 48px 32px 32px;
            padding: 20px 16px 18px;
            margin: 4px 0 18px;
            border: 1px solid #fad7ce;
            box-shadow: 0 6px 0 #d9b0a5;
        }
        .produk-flex {
            display: flex;
            gap: 16px;
            align-items: center;
            flex-wrap: wrap;
        }
        .produk-gambar {
            flex: 0 0 110px;
        }
        .produk-gambar img {
            width: 100%;
            aspect-ratio: 1/1;
            object-fit: cover;
            border-radius: 60px 30px 60px 30px;
            border: 4px solid white;
            box-shadow: 0 12px 18px rgba(160, 60, 40, 0.15);
            background: #f5dbd3;
        }
        .produk-info {
            flex: 1;
            min-width: 140px;
        }
        .produk-info h3 {
            font-size: 1.4rem;
            font-weight: 800;
            color: #871f18;
            line-height: 1.2;
        }
        .produk-info .sub {
            font-size: 0.75rem;
            color: #79443a;
            background: rgba(255, 255, 240, 0.7);
            padding: 4px 14px;
            border-radius: 40px;
            display: inline-block;
            margin: 6px 0 8px;
            border: 1px solid #f0cbc2;
        }
        .harga-badge {
            background: #a62c24;
            color: white;
            padding: 8px 20px;
            border-radius: 60px;
            font-weight: 700;
            font-size: 1.4rem;
            display: inline-block;
            box-shadow: 0 4px 0 #631b16;
            letter-spacing: 0.5px;
        }
        .harga-badge small {
            font-size: 0.75rem;
            font-weight: 400;
            margin-right: 4px;
        }

        .order-section {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 12px 16px;
            margin: 14px 0 16px;
            background: #fefaf8;
            padding: 12px 18px;
            border-radius: 60px;
            border: 1px solid #f0cdc4;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.02);
        }
        .order-section label {
            font-weight: 700;
            color: #5a342b;
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.95rem;
        }
        .order-section label i {
            color: #b5312a;
        }
        .qty-control {
            display: flex;
            align-items: center;
            gap: 6px;
            margin-left: auto;
        }
        .qty-control button {
            background: #f5e1db;
            border: none;
            width: 38px;
            height: 38px;
            border-radius: 40px;
            font-size: 1.4rem;
            font-weight: 700;
            color: #6d3128;
            cursor: pointer;
            transition: 0.12s;
            box-shadow: 0 2px 0 #dbb6ab;
            display: inline-flex;
            align-items: center;
            justify-content: center;
        }
        .qty-control button:active {
            transform: scale(0.92);
            background: #dcc0b7;
        }
        .qty-control span {
            font-size: 1.7rem;
            font-weight: 800;
            min-width: 44px;
            text-align: center;
            color: #431f19;
        }

        .btn-pesan {
            background: #c0392b;
            border: none;
            color: white;
            font-weight: 700;
            font-size: 1.2rem;
            padding: 18px 10px;
            border-radius: 80px;
            width: 100%;
            box-shadow: 0 8px 0 #782b20;
            transition: 0.08s linear;
            cursor: pointer;
            letter-spacing: 0.5px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            margin: 6px 0 4px;
        }
        .btn-pesan:active {
            transform: translateY(4px);
            box-shadow: 0 4px 0 #782b20;
        }
        .btn-pesan i {
            font-size: 1.2rem;
        }

        .payment-box {
            background: #fef6f3;
            border-radius: 32px;
            padding: 18px 18px 16px;
            margin: 18px 0 12px;
            border: 2px dashed #c0392b;
            display: none;
            transition: 0.25s;
        }
        .payment-box.show {
            display: block;
            animation: fadeSlide 0.35s ease;
        }
        @keyframes fadeSlide {
            0% {
                opacity: 0;
                transform: translateY(-10px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .payment-box .bank {
            background: #1a3c5e;
            color: white;
            padding: 12px 16px;
            border-radius: 60px;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 12px;
            flex-wrap: wrap;
            margin-bottom: 14px;
            font-size: 0.85rem;
        }
        .payment-box .bank i {
            font-size: 1.5rem;
        }
        .payment-box .bank span {
            word-break: break-all;
            font-size: 0.85rem;
            letter-spacing: 0.3px;
        }
        .payment-box .total-harga {
            font-size: 1.6rem;
            font-weight: 800;
            color: #871f18;
            background: white;
            padding: 6px 20px;
            border-radius: 60px;
            display: inline-block;
            border: 1px solid #dbb6ab;
            margin-top: 4px;
        }
        .payment-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 8px;
        }
        .payment-row .label-total {
            font-weight: 600;
            color: #431f19;
            font-size: 0.95rem;
        }

        .upload-area {
            margin: 16px 0 14px;
            display: flex;
            flex-direction: column;
            gap: 8px;
        }
        .upload-area label {
            background: white;
            padding: 12px 16px;
            border-radius: 60px;
            border: 1px solid #dbb6ab;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 12px;
            color: #431f19;
            cursor: pointer;
            transition: 0.12s;
        }
        .upload-area label:active {
            background: #f5e1db;
        }
        .upload-area input {
            display: none;
        }
        .upload-area .file-name {
            font-weight: 400;
            font-size: 0.8rem;
            color: #6e3f34;
            margin-left: 4px;
            overflow: hidden;
            text-overflow: ellipsis;
            white-space: nowrap;
            max-width: 160px;
        }

        .btn-selesai {
            background: #2c7a4a;
            border: none;
            color: white;
            font-weight: 700;
            padding: 15px;
            border-radius: 60px;
            width: 100%;
            box-shadow: 0 5px 0 #1b4f30;
            transition: 0.07s;
            cursor: pointer;
            font-size: 1rem;
            margin: 8px 0 4px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
        }
        .btn-selesai:active {
            transform: translateY(4px);
            box-shadow: 0 2px 0 #1b4f30;
        }

        .wa-contact {
            background: #25a55b;
            color: white;
            padding: 15px 18px;
            border-radius: 60px;
            text-align: center;
            font-weight: 700;
            font-size: 1rem;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 14px;
            margin: 18px 0 6px;
            border: 1px solid #1d8a4a;
            box-shadow: 0 4px 0 #16703b;
            transition: 0.07s;
            cursor: pointer;
            text-decoration: none;
            color: white;
        }
        .wa-contact:active {
            transform: translateY(4px);
            box-shadow: 0 1px 0 #16703b;
        }
        .wa-contact i {
            font-size: 1.7rem;
        }

        .footer-note {
            text-align: center;
            font-size: 0.7rem;
            color: #8b6b61;
            margin-top: 18px;
            border-top: 1px solid #f0dbd4;
            padding-top: 16px;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 6px;
            flex-wrap: wrap;
        }
        .footer-note i {
            color: #c0392b;
        }

        @media (max-width: 420px) {
            .container {
                padding: 16px 14px 24px;
            }
            .produk-flex {
                flex-direction: column;
                align-items: center;
                text-align: center;
            }
            .produk-gambar {
                flex: 0 0 140px;
            }
            .order-section {
                flex-direction: column;
                align-items: stretch;
                border-radius: 32px;
                padding: 14px 16px;
            }
            .qty-control {
                margin-left: 0;
                justify-content: center;
            }
            .header h1 {
                font-size: 1.3rem;
            }
            .badge-flag {
                font-size: 0.7rem;
                padding: 4px 10px;
            }
            .payment-box .bank {
                font-size: 0.75rem;
                padding: 10px 14px;
            }
            .payment-box .bank span {
                font-size: 0.75rem;
            }
            .upload-area .file-name {
                max-width: 100px;
            }
        }
        @media (max-width: 360px) {
            .produk-info h3 {
                font-size: 1.1rem;
            }
            .harga-badge {
                font-size: 1.1rem;
                padding: 6px 14px;
            }
            .btn-pesan {
                font-size: 1rem;
                padding: 14px 10px;
            }
        }
    </style>
</head>
<body>

    <div class="container" id="app">

        <div class="header">
            <h1>
                Lumpia Kukus
                <small>Kuah Korea • Sehat</small>
            </h1>
            <div class="badge-flag">
                <i class="fas fa-utensils"></i> Odeng
            </div>
        </div>

        <!-- ===== CAROUSEL MAKANAN REALISTIS ===== -->
        <div class="carousel">
            <div class="carousel-item">
                <img src="https://images.unsplash.com/photo-1591343395082-e1200878b9a5?w=200&h=200&fit=crop&crop=center&auto=format" alt="Tteokbokki" />
                <span>🌶️ Tteokbokki</span>
            </div>
            <div class="carousel-item">
                <img src="https://images.unsplash.com/photo-1633945274405-b6c2421e5a8d?w=200&h=200&fit=crop&crop=center&auto=format" alt="Lumpia Sayur Kukus" />
                <span>🥬 Lumpia Kukus</span>
            </div>
            <div class="carousel-item">
                <img src="https://images.unsplash.com/photo-1559314809-0d155014e29e?w=200&h=200&fit=crop&crop=center&auto=format" alt="Odeng Kuah" />
                <span>🍲 Odeng Kuah</span>
            </div>
            <div class="carousel-item">
                <img src="https://images.unsplash.com/photo-1601050690597-df0568f70950?w=200&h=200&fit=crop&crop=center&auto=format" alt="Korean Food" />
                <span>🥢 Korean Food</span>
            </div>
            <div class="carousel-item">
                <img src="https://images.unsplash.com/photo-1586190848861-99aa4a171e90?w=200&h=200&fit=crop&crop=center&auto=format" alt="Ramen" />
                <span>🍜 Ramen</span>
            </div>
        </div>

        <!-- ===== PRODUK UTAMA ===== -->
        <div class="produk-utama">
            <div class="produk-flex">
                <div class="produk-gambar">
                    <img src="https://images.unsplash.com/photo-1633945274405-b6c2421e5a8d?w=300&h=300&fit=crop&crop=center&auto=format" alt="Lumpia Sayur Kukus" />
                </div>
                <div class="produk-info">
                    <h3>Lumpia Odeng<br />Kuah Korea</h3>
                    <div class="sub"><i class="fas fa-star" style="color:#c0392b;"></i> Sehat • Paper bowl</div>
                    <div class="harga-badge"><small>Rp</small>15.000</div>
                </div>
            </div>
        </div>

        <!-- ===== ORDER SECTION ===== -->
        <div class="order-section">
            <label><i class="fas fa-shopping-bag"></i> Jumlah</label>
            <div class="qty-control">
                <button id="decreaseQty" aria-label="kurangi"><i class="fas fa-minus"></i></button>
                <span id="qtyDisplay">1</span>
                <button id="increaseQty" aria-label="tambah"><i class="fas fa-plus"></i></button>
            </div>
        </div>

        <!-- ===== TOMBOL PESAN ===== -->
        <button class="btn-pesan" id="btnPesan">
            <i class="fas fa-hand-holding-heart"></i> Pesan Sekarang
        </button>

        <!-- ===== PAYMENT BOX ===== -->
        <div class="payment-box" id="paymentBox">
            <div class="bank">
                <i class="fas fa-university"></i>
                <span>BRI • 629701022194533 • SUTRISMI AMBARWATI</span>
            </div>

            <div class="payment-row">
                <span class="label-total"><i class="fas fa-receipt"></i> Total:</span>
                <span class="total-harga" id="totalHarga">Rp 15.000</span>
            </div>

            <div class="upload-area">
                <label for="buktiBayar">
                    <i class="fas fa-cloud-upload-alt"></i>
                    Upload Bukti Transfer
                    <span class="file-name" id="fileName">(belum ada file)</span>
                </label>
                <input type="file" id="buktiBayar" accept="image/*" />
            </div>

            <button class="btn-selesai" id="btnSelesai">
                <i class="fas fa-check-circle"></i> Selesai & Kirim Bukti
            </button>
        </div>

        <!-- ===== KONTAK WA ===== -->
        <a href="https://wa.me/6285704332235?text=Halo%20saya%20sudah%20pesan%20Lumpia%20Kuah%20Korea" target="_blank" class="wa-contact" id="waContact">
            <i class="fab fa-whatsapp"></i> Hubungi WA 0857-0433-2235
        </a>

        <div class="footer-note">
            <i class="fas fa-heart"></i> Korean Food Sehat • Paper bowl menarik
            <span style="margin:0 4px;">•</span>
            <i class="fas fa-flag" style="color:#c0392b;"></i> Merah Putih
        </div>

    </div>

    <script>
        (function() {
            'use strict';

            const qtyDisplay = document.getElementById('qtyDisplay');
            const decreaseBtn = document.getElementById('decreaseQty');
            const increaseBtn = document.getElementById('increaseQty');
            const btnPesan = document.getElementById('btnPesan');
            const paymentBox = document.getElementById('paymentBox');
            const totalHargaSpan = document.getElementById('totalHarga');
            const fileInput = document.getElementById('buktiBayar');
            const fileNameSpan = document.getElementById('fileName');
            const btnSelesai = document.getElementById('btnSelesai');
            const waContact = document.getElementById('waContact');

            const HARGA = 15000;
            let qty = 1;

            function updateQtyDisplay() {
                qtyDisplay.textContent = qty;
            }

            function updateTotalHarga() {
                const total = qty * HARGA;
                totalHargaSpan.textContent = 'Rp ' + total.toLocaleString('id-ID');
            }

            function showPaymentBox() {
                if (!paymentBox.classList.contains('show')) {
                    paymentBox.classList.add('show');
                    setTimeout(() => {
                        paymentBox.scrollIntoView({ behavior: 'smooth', block: 'center' });
                    }, 100);
                }
                updateTotalHarga();
            }

            decreaseBtn.addEventListener('click', function() {
                if (qty > 1) {
                    qty--;
                    updateQtyDisplay();
                    if (paymentBox.classList.contains('show')) {
                        updateTotalHarga();
                    }
                }
            });

            increaseBtn.addEventListener('click', function() {
                qty++;
                updateQtyDisplay();
                if (paymentBox.classList.contains('show')) {
                    updateTotalHarga();
                }
            });

            btnPesan.addEventListener('click', function() {
                showPaymentBox();

                const originalHtml = btnPesan.innerHTML;
                btnPesan.innerHTML = '<i class="fas fa-spinner fa-pulse"></i> Memproses...';
                btnPesan.style.background = '#2c7a4a';
                btnPesan.style.boxShadow = '0 8px 0 #1b4f30';
                btnPesan.disabled = true;

                setTimeout(() => {
                    btnPesan.innerHTML = '<i class="fas fa-check-circle"></i> Pesanan Dibuat';
                    btnPesan.style.background = '#1f8a4a';
                }, 800);

                setTimeout(() => {
                    btnPesan.innerHTML = originalHtml;
                    btnPesan.style.background = '#c0392b';
                    btnPesan.style.boxShadow = '0 8px 0 #782b20';
                    btnPesan.disabled = false;
                }, 2200);
            });

            fileInput.addEventListener('change', function(e) {
                if (fileInput.files.length > 0) {
                    const name = fileInput.files[0].name;
                    const displayName = name.length > 25 ? name.slice(0, 22) + '...' : name;
                    fileNameSpan.textContent = '📎 ' + displayName;
                } else {
                    fileNameSpan.textContent = '(belum ada file)';
                }
            });

            btnSelesai.addEventListener('click', function() {
                if (fileInput.files.length === 0) {
                    alert('⚠️ Harap upload bukti pembayaran terlebih dahulu.');
                    return;
                }

                const total = qty * HARGA;
                const confirmMsg = '✅ Pesanan Anda telah kami terima!\n' +
                    '📦 Produk: Lumpia Odeng Kuah Korea\n' +
                    '🔢 Jumlah: ' + qty + ' porsi\n' +
                    '💰 Total: Rp ' + total.toLocaleString('id-ID') + '\n\n' +
                    '📞 Silakan hubungi kontak WA untuk konfirmasi pesanan.';

                alert(confirmMsg);

                const originalSelesai = btnSelesai.innerHTML;
                btnSelesai.innerHTML = '<i class="fas fa-check"></i> Terkirim';
                btnSelesai.style.background = '#1f6a3a';
                setTimeout(() => {
                    btnSelesai.innerHTML = originalSelesai;
                    btnSelesai.style.background = '#2c7a4a';
                }, 1500);
            });

            waContact.addEventListener('click', function(e) {
                console.log('Kontak WA diklik');
            });

            updateQtyDisplay();

        })();
    </script>

</body>
</html>
