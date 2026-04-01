

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Klasifikasi Sekolah FLS3N Kota Tegal</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/PapaParse/5.4.1/papaparse.min.js"></script>
    <style>
        body { font-family: 'Inter', sans-serif; background-color: #f3f4f6; }
        .glass-card {
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
        }
    </style>
</head>
<body class="text-gray-800 p-4 md:p-8">

    <div class="max-w-6xl mx-auto">
        <header class="mb-8 text-center">
            <h1 class="text-3xl font-bold text-blue-700 mb-2">Klasifikasi Sekolah FLS3N & LDI Kota Tegal</h1>
            <p class="text-gray-600">Berdasarkan Asal Kecamatan (Pemetaan Otomatis dari Nama Sekolah)</p>
        </header>

        <!-- Upload Section -->
        <div class="glass-card p-6 mb-8 text-center border-t-4 border-blue-500">
            <h2 class="text-xl font-semibold mb-4">Mulai Klasifikasi Data Anda</h2>
            <p class="text-sm text-gray-500 mb-4">Pilih file CSV "Pendaftar FLS3N" Anda. Data diproses secara lokal di browser Anda.</p>
            
            <label class="block w-full max-w-md mx-auto relative cursor-pointer">
                <input type="file" id="csvFileInput" accept=".csv" class="hidden">
                <div class="bg-blue-50 hover:bg-blue-100 border-2 border-dashed border-blue-300 rounded-lg p-6 transition duration-300">
                    <svg class="mx-auto h-12 w-12 text-blue-400 mb-3" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"></path>
                    </svg>
                    <span id="fileNameDisplay" class="text-blue-600 font-medium">Klik untuk memilih file .csv</span>
                </div>
            </label>
        </div>

        <!-- Loading State -->
        <div id="loading" class="hidden text-center py-8">
            <div class="animate-spin rounded-full h-12 w-12 border-b-2 border-blue-700 mx-auto"></div>
            <p class="mt-4 text-gray-600">Memproses dan mengklasifikasi data...</p>
        </div>

        <!-- Results Section -->
        <div id="resultsContainer" class="hidden">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-8">
                <!-- Summary Cards -->
                <div class="glass-card p-4 border-l-4 border-red-500">
                    <h3 class="text-sm text-gray-500 font-bold uppercase">Tegal Timur</h3>
                    <p id="countTimur" class="text-3xl font-bold text-gray-800">0</p>
                    <p class="text-xs text-gray-400">Peserta</p>
                </div>
                <div class="glass-card p-4 border-l-4 border-yellow-500">
                    <h3 class="text-sm text-gray-500 font-bold uppercase">Tegal Barat</h3>
                    <p id="countBarat" class="text-3xl font-bold text-gray-800">0</p>
                    <p class="text-xs text-gray-400">Peserta</p>
                </div>
                <div class="glass-card p-4 border-l-4 border-green-500">
                    <h3 class="text-sm text-gray-500 font-bold uppercase">Tegal Selatan</h3>
                    <p id="countSelatan" class="text-3xl font-bold text-gray-800">0</p>
                    <p class="text-xs text-gray-400">Peserta</p>
                </div>
                <div class="glass-card p-4 border-l-4 border-blue-500">
                    <h3 class="text-sm text-gray-500 font-bold uppercase">Margadana</h3>
                    <p id="countMargadana" class="text-3xl font-bold text-gray-800">0</p>
                    <p class="text-xs text-gray-400">Peserta</p>
                </div>
            </div>

            <!-- Detailed Tables Grid -->
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
                <!-- Tegal Timur -->
                <div class="glass-card overflow-hidden">
                    <div class="bg-red-500 text-white p-3 font-semibold">Kecamatan Tegal Timur</div>
                    <div class="p-0 max-h-96 overflow-y-auto">
                        <table class="w-full text-left text-sm">
                            <thead class="bg-gray-50 sticky top-0">
                                <tr>
                                    <th class="p-3 border-b">Nama Sekolah</th>
                                    <th class="p-3 border-b text-center w-24">Jml Peserta</th>
                                </tr>
                            </thead>
                            <tbody id="tableTimur" class="divide-y divide-gray-100"></tbody>
                        </table>
                    </div>
                </div>

                <!-- Tegal Barat -->
                <div class="glass-card overflow-hidden">
                    <div class="bg-yellow-500 text-white p-3 font-semibold">Kecamatan Tegal Barat</div>
                    <div class="p-0 max-h-96 overflow-y-auto">
                        <table class="w-full text-left text-sm">
                            <thead class="bg-gray-50 sticky top-0">
                                <tr>
                                    <th class="p-3 border-b">Nama Sekolah</th>
                                    <th class="p-3 border-b text-center w-24">Jml Peserta</th>
                                </tr>
                            </thead>
                            <tbody id="tableBarat" class="divide-y divide-gray-100"></tbody>
                        </table>
                    </div>
                </div>

                <!-- Tegal Selatan -->
                <div class="glass-card overflow-hidden">
                    <div class="bg-green-500 text-white p-3 font-semibold">Kecamatan Tegal Selatan</div>
                    <div class="p-0 max-h-96 overflow-y-auto">
                        <table class="w-full text-left text-sm">
                            <thead class="bg-gray-50 sticky top-0">
                                <tr>
                                    <th class="p-3 border-b">Nama Sekolah</th>
                                    <th class="p-3 border-b text-center w-24">Jml Peserta</th>
                                </tr>
                            </thead>
                            <tbody id="tableSelatan" class="divide-y divide-gray-100"></tbody>
                        </table>
                    </div>
                </div>

                <!-- Margadana -->
                <div class="glass-card overflow-hidden">
                    <div class="bg-blue-500 text-white p-3 font-semibold">Kecamatan Margadana</div>
                    <div class="p-0 max-h-96 overflow-y-auto">
                        <table class="w-full text-left text-sm">
                            <thead class="bg-gray-50 sticky top-0">
                                <tr>
                                    <th class="p-3 border-b">Nama Sekolah</th>
                                    <th class="p-3 border-b text-center w-24">Jml Peserta</th>
                                </tr>
                            </thead>
                            <tbody id="tableMargadana" class="divide-y divide-gray-100"></tbody>
                        </table>
                    </div>
                </div>
            </div>

            <!-- Unclassified -->
            <div class="mt-6 glass-card overflow-hidden border border-gray-200">
                <div class="bg-gray-700 text-white p-3 font-semibold">Perlu Dicek Manual (Nama Kelurahan Tidak Ditemukan)</div>
                <div class="p-0 max-h-64 overflow-y-auto">
                    <table class="w-full text-left text-sm">
                        <thead class="bg-gray-50 sticky top-0">
                            <tr>
                                <th class="p-3 border-b">Nama Sekolah</th>
                                <th class="p-3 border-b text-center w-24">Jml Peserta</th>
                            </tr>
                        </thead>
                        <tbody id="tableLainnya" class="divide-y divide-gray-100"></tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Mapping keywords (Kelurahan & Known Schools) to Kecamatan in Kota Tegal
        const keywordMapping = {
            "Tegal Timur": ["MANGKUKUSUMAN", "SLEROK", "MINTARAGEN", "PANGGUNG", "KEJAMBON", "USAMAH", "MUHAMMADIYAH 1", "THI", "AL IRSYAD", "MUTIARA", "PANCASILA", "SD IHSANIYAH 1 TEGAL", "SD AISYIYAH CAHAYA INSAN"],
            "Tegal Barat": ["KRATON", "TEGALSARI", "CAMPAKA", "DEBONG LOR", "KEMANDUNGAN", "MUARAREJA", "PEKAUMAN", "PESURUNGAN KIDUL", "PIASAN", "TRITUNGGAL", "IKHSANIYAH", "MA MUR", "SD THHK" , "SDPIUS TEGAL", "SD GLOBAL INBYRA", "SD IHSANIYAH GAJAHMADA TEGAL", "SD PUTRA WACANA"],
            "Tegal Selatan": ["BANDUNG", "DEBONG KIDUL", "DEBONG KULON", "DEBONG TENGAH", "KALINYAMAT WETAN", "KETUREN", "RANDUGUNTING", "TUNON", "KECANDAN", "SD IT BINA IMAN DAN AMAL SHALEH ASSALAM"],
            "Margadana": ["MARGADANA", "KRANDON", "CABAWAN", "KALIGANGSA", "KALINYAMAT KULON", "PESURUNGAN LOR", "SUMURPANGGANG", "MANGUNJAWA"]
        };

        document.getElementById('csvFileInput').addEventListener('change', function(e) {
            const file = e.target.files[0];
            if (!file) return;

            document.getElementById('fileNameDisplay').textContent = file.name;
            document.getElementById('loading').classList.remove('hidden');
            document.getElementById('resultsContainer').classList.add('hidden');

            Papa.parse(file, {
                header: true,
                skipEmptyLines: true,
                complete: function(results) {
                    processData(results.data);
                }
            });
        });

        function getKecamatan(schoolName) {
            if (!schoolName) return "Lainnya";
            const upperName = schoolName.toUpperCase();
            
            for (const [kecamatan, keywords] of Object.entries(keywordMapping)) {
                for (const keyword of keywords) {
                    if (upperName.includes(keyword)) {
                        return kecamatan;
                    }
                }
            }
            return "Lainnya";
        }

        function processData(data) {
            const schoolStats = {
                "Tegal Timur": {},
                "Tegal Barat": {},
                "Tegal Selatan": {},
                "Margadana": {},
                "Lainnya": {}
            };

            const participantCounts = {
                "Tegal Timur": 0,
                "Tegal Barat": 0,
                "Tegal Selatan": 0,
                "Margadana": 0,
                "Lainnya": 0
            };

            // Aggregate data
            data.forEach(row => {
                // Adjust property name based on standard CSV columns, checking variations
                const schoolName = row.Sekolah || row.sekolah || row['Nama Sekolah']; 
                if (!schoolName) return; // Skip if no school name

                const kecamatan = getKecamatan(schoolName);
                
                if (!schoolStats[kecamatan][schoolName]) {
                    schoolStats[kecamatan][schoolName] = 0;
                }
                schoolStats[kecamatan][schoolName]++;
                participantCounts[kecamatan]++;
            });

            // Update UI
            updateDashboard(schoolStats, participantCounts);
        }

        function renderTableRows(statsObject, tableId) {
            const tbody = document.getElementById(tableId);
            tbody.innerHTML = '';
            
            // Sort schools by name
            const sortedSchools = Object.keys(statsObject).sort();
            
            if (sortedSchools.length === 0) {
                tbody.innerHTML = `<tr><td colspan="2" class="p-4 text-center text-gray-400 italic">Tidak ada data</td></tr>`;
                return;
            }

            sortedSchools.forEach(school => {
                const tr = document.createElement('tr');
                tr.className = "hover:bg-gray-50";
                tr.innerHTML = `
                    <td class="p-3 font-medium text-gray-700">${school}</td>
                    <td class="p-3 text-center bg-gray-50 text-gray-600 font-semibold">${statsObject[school]}</td>
                `;
                tbody.appendChild(tr);
            });
        }

        function updateDashboard(schoolStats, participantCounts) {
            // Update counts
            document.getElementById('countTimur').textContent = participantCounts["Tegal Timur"];
            document.getElementById('countBarat').textContent = participantCounts["Tegal Barat"];
            document.getElementById('countSelatan').textContent = participantCounts["Tegal Selatan"];
            document.getElementById('countMargadana').textContent = participantCounts["Margadana"];

            // Render tables
            renderTableRows(schoolStats["Tegal Timur"], 'tableTimur');
            renderTableRows(schoolStats["Tegal Barat"], 'tableBarat');
            renderTableRows(schoolStats["Tegal Selatan"], 'tableSelatan');
            renderTableRows(schoolStats["Margadana"], 'tableMargadana');
            renderTableRows(schoolStats["Lainnya"], 'tableLainnya');

            // Show results
            document.getElementById('loading').classList.add('hidden');
            document.getElementById('resultsContainer').classList.remove('hidden');
        }
    </script>
</body>
</html>