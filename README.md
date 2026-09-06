<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ระบบโครงสร้างองค์กรและหน้าที่ความรับผิดชอบ - สำนักบริหารเทคโนโลยีสารสนเทศ</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Prompt:wght@300;400;500;600;700&family=Sarabun:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Prompt', 'Sarabun', sans-serif; background-color: #f8fafc; }
        .tab-btn.active { background-color: #1e3a8a; color: #ffffff; border-color: #1e3a8a; }
    </style>
</head>
<body class="text-slate-800 antialiased min-h-screen flex flex-col">

    <!-- Header & Navigation -->
    <header class="bg-slate-900 text-white sticky top-0 z-50 shadow-md">
        <div class="max-w-7xl mx-auto px-4 py-4 flex flex-col sm:flex-row justify-between items-center gap-4">
            <div>
                <h1 class="text-xl sm:text-2xl font-bold tracking-tight text-blue-100">สำนักบริหารเทคโนโลยีสารสนเทศ[cite: 1]</h1>
                <p class="text-xs text-slate-400 mt-1">คำสั่งมอบหมายหน้าที่ความรับผิดชอบ (ลว. 5 กันยายน 2569)[cite: 1]</p>
            </div>
            <!-- Tab Buttons -->
            <div class="flex bg-slate-800 p-1 rounded-xl border border-slate-700">
                <button onclick="switchTab('chart')" id="tab-chart" class="tab-btn active px-4 py-2 rounded-lg text-sm font-medium transition flex items-center gap-2">
                    <span>📊</span> ผังองค์กร & แดชบอร์ด
                </button>
                <button onclick="switchTab('responsibilities')" id="tab-resp" class="tab-btn px-4 py-2 rounded-lg text-sm font-medium text-slate-300 transition flex items-center gap-2">
                    <span>📋</span> หน้าที่ความรับผิดชอบกลุ่มงาน
                </button>
            </div>
        </div>
    </header>

    <!-- Main Content Container -->
    <main class="max-w-7xl mx-auto px-4 py-8 flex-1 w-full">

        <!-- ================= PAGE 1: CHART & DIRECTORY ================= -->
        <div id="page-chart" class="space-y-8">
            
            <!-- Summary Stats -->
            <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
                <div class="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm">
                    <p class="text-xs font-semibold text-slate-400 uppercase">ผู้อำนวยการสำนัก</p>
                    <p class="text-lg font-bold text-slate-800 mt-1">นางสาวมุทิตา ชูประดิษฐ์[cite: 1]</p>
                    <p class="text-xs text-blue-600 mt-0.5">ผู้อำนวยการสำนักบริหารเทคโนโลยีสารสนเทศ[cite: 1]</p>
                </div>
                <div class="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm">
                    <p class="text-xs font-semibold text-slate-400 uppercase">ผู้เชี่ยวชาญกำกับดูแล</p>
                    <p class="text-lg font-bold text-slate-800 mt-1">นายเทวัญ แก้วศักดาศิริ[cite: 1]</p>
                    <p class="text-xs text-blue-600 mt-0.5">นักวิชาการคอมพิวเตอร์เชี่ยวชาญ[cite: 1]</p>
                </div>
                <div class="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm">
                    <p class="text-xs font-semibold text-slate-400 uppercase">กลุ่มงานหลัก & ฝ่ายบริหาร</p>
                    <p class="text-2xl font-bold text-slate-800 mt-1">6 กลุ่มงาน + 1 ฝ่าย[cite: 1]</p>
                    <p class="text-xs text-emerald-600 mt-0.5">ครอบคลุมทุกภารกิจดิจิทัล</p>
                </div>
                <div class="bg-white p-5 rounded-2xl border border-slate-200 shadow-sm">
                    <p class="text-xs font-semibold text-slate-400 uppercase">จำนวนบุคลากรทั้งหมด (Unique)</p>
                    <p class="text-2xl font-bold text-slate-800 mt-1">62 คน</p>
                    <p class="text-xs text-slate-500 mt-0.5">ข้าราชการ/พนักงาน/ลูกจ้าง[cite: 1]</p>
                </div>
            </div>

            <!-- Org Structure Visual & Chart -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
                <!-- Org Chart Card -->
                <div class="lg:col-span-2 bg-white p-6 rounded-2xl border border-slate-200 shadow-sm space-y-6">
                    <h2 class="text-lg font-bold text-slate-800 border-b pb-3">ผังการบริหารงานเชิงโครงสร้าง</h2>
                    
                    <!-- Director -->
                    <div class="text-center p-4 bg-blue-900 text-white rounded-xl shadow-md max-w-md mx-auto">
                        <p class="text-xs text-blue-200">ผู้อำนวยการสำนักบริหารเทคโนโลยีสารสนเทศ[cite: 1]</p>
                        <p class="text-base font-bold">นางสาวมุทิตา ชูประดิษฐ์[cite: 1]</p>
                    </div>

                    <div class="w-0.5 h-6 bg-slate-300 mx-auto"></div>

                    <!-- Senior Expert -->
                    <div class="text-center p-3 bg-slate-100 border border-slate-300 rounded-xl max-w-sm mx-auto">
                        <p class="text-xs text-slate-500">ผู้เชี่ยวชาญกำกับดูแล (นักวิชาการคอมพิวเตอร์เชี่ยวชาญ)[cite: 1]</p>
                        <p class="text-sm font-semibold text-slate-800">นายเทวัญ แก้วศักดาศิริ[cite: 1]</p>
                        <p class="text-xs text-slate-500 mt-1">(กำกับดูแล กลุ่มงานบริหารจัดการระบบคอมพิวเตอร์ฯ & กลุ่มงานบริหารเครือข่ายฯ)[cite: 1]</p>
                    </div>

                    <div class="w-0.5 h-6 bg-slate-300 mx-auto"></div>

                    <!-- Groups List -->
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-3 text-xs">
                        <div class="p-3 bg-slate-50 border rounded-lg">
                            <p class="font-bold text-blue-900">1. กลุ่มงานพัฒนาระบบสารสนเทศ[cite: 1]</p>
                            <p class="text-slate-600">ผอ.: นายนัฐพงษ์ บุญวงศ์[cite: 1]</p>
                        </div>
                        <div class="p-3 bg-slate-50 border rounded-lg">
                            <p class="font-bold text-blue-900">2. กลุ่มงานบริหารจัดการระบบคอมพิวเตอร์และประมวลผล[cite: 1]</p>
                            <p class="text-slate-600">ผอ.: นายไกรรัฐ อาภาบุษยพันธุ์ (รักษาการ)[cite: 1]</p>
                        </div>
                        <div class="p-3 bg-slate-50 border rounded-lg">
                            <p class="font-bold text-blue-900">3. กลุ่มงานบริหารเครือข่ายสื่อสารและความมั่นคงคอมพิวเตอร์[cite: 1]</p>
                            <p class="text-slate-600">ผอ.: นายธนวัต สาธานนท์[cite: 1]</p>
                        </div>
                        <div class="p-3 bg-slate-50 border rounded-lg">
                            <p class="font-bold text-blue-900">4. กลุ่มงานบริการเทคโนโลยีสารสนเทศ[cite: 1]</p>
                            <p class="text-slate-600">ผอ.: นายธนากร ชัยวิชู (รักษาการ)</p>
                        </div>
                        <div class="p-3 bg-slate-50 border rounded-lg">
                            <p class="font-bold text-blue-900">5. กลุ่มงานบริการอิเล็กทรอนิกส์[cite: 1]</p>
                            <p class="text-slate-600">ผอ.: นายธนพัฒน์ บริรักษ์[cite: 1]</p>
                        </div>
                        <div class="p-3 bg-slate-50 border rounded-lg">
                            <p class="font-bold text-blue-900">6. ฝ่ายบริหารทั่วไป[cite: 1]</p>
                            <p class="text-slate-600">หัวหน้าฝ่าย: นางสาวรตา หมัดโต๊ะหมัน[cite: 1]</p>
                        </div>
                    </div>
                </div>

                <!-- Workforce Chart -->
                <div class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm flex flex-col justify-between">
                    <h2 class="text-lg font-bold text-slate-800 border-b pb-3">สัดส่วนบุคลากรรายกลุ่มงาน</h2>
                    <div class="relative my-auto py-4">
                        <canvas id="workforceChart" class="max-h-64 mx-auto"></canvas>
                    </div>
                    <p class="text-xs text-center text-slate-400 mt-2">*คำนวณแบบนับจำนวนคนไม่ซ้ำตัวบุคคล (Deduplicated)</p>
                </div>
            </div>

            <!-- Staff Directory Table -->
            <div class="bg-white rounded-2xl border border-slate-200 shadow-sm overflow-hidden">
                <div class="p-6 border-b border-slate-100 flex flex-col sm:flex-row justify-between sm:items-center gap-4">
                    <div>
                        <h2 class="text-lg font-bold text-slate-800">ทำเนียบบุคลากรสำนักบริหารเทคโนโลยีสารสนเทศ[cite: 1]</h2>
                        <p class="text-xs text-slate-500">แสดงรายชื่อพร้อมตำแหน่งทางราชการและตำแหน่งในการบริหาร[cite: 1]</p>
                    </div>
                    <input type="text" id="searchInput" onkeyup="filterDirectory()" placeholder="ค้นหาชื่อ, ตำแหน่ง, หรือสังกัด..." class="px-4 py-2 border border-slate-300 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-blue-500 w-full sm:w-64">
                </div>
                
                <div class="overflow-x-auto">
                    <table class="w-full text-left text-sm text-slate-600" id="directoryTable">
                        <thead class="bg-slate-50 text-slate-700 font-semibold text-xs uppercase border-b border-slate-200">
                            <tr>
                                <th class="py-3.5 px-4">ชื่อ - สกุล[cite: 1]</th>
                                <th class="py-3.5 px-4">ตำแหน่งทางราชการ[cite: 1]</th>
                                <th class="py-3.5 px-4">ตำแหน่งงานบริหาร / ฝ่ายสังกัด[cite: 1]</th>
                                <th class="py-3.5 px-4">กลุ่มงาน / สังกัด[cite: 1]</th>
                            </tr>
                        </thead>
                        <tbody class="divide-y divide-slate-100">
                            <!-- High Level Execs -->
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นางสาวมุทิตา ชูประดิษฐ์[cite: 1]</td>
                                <td class="py-3 px-4">ผู้อำนวยการสำนักบริหารเทคโนโลยีสารสนเทศ[cite: 1]</td>
                                <td class="py-3 px-4"><span class="px-2 py-1 bg-blue-100 text-blue-800 rounded-md text-xs font-medium">ผู้บริหารสูงสุด[cite: 1]</span></td>
                                <td class="py-3 px-4">สำนักบริหารเทคโนโลยีสารสนเทศ[cite: 1]</td>
                            </tr>
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นายเทวัญ แก้วศักดาศิริ[cite: 1]</td>
                                <td class="py-3 px-4">นักวิชาการคอมพิวเตอร์เชี่ยวชาญ[cite: 1]</td>
                                <td class="py-3 px-4"><span class="px-2 py-1 bg-amber-100 text-amber-800 rounded-md text-xs font-medium">ผู้เชี่ยวชาญกำกับดูแล[cite: 1]</span></td>
                                <td class="py-3 px-4">ผู้เชี่ยวชาญกำกับดูแล[cite: 1]</td>
                            </tr>
                            <!-- Sample Group Heads & Staff -->
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นายนัฐพงษ์ บุญวงศ์[cite: 1]</td>
                                <td class="py-3 px-4">นักวิชาการคอมพิวเตอร์ชำนาญการพิเศษ[cite: 1]</td>
                                <td class="py-3 px-4">ผอ.กลุ่มงาน[cite: 1]</td>
                                <td class="py-3 px-4">กลุ่มงานพัฒนาระบบสารสนเทศ[cite: 1]</td>
                            </tr>
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นายชวรัส เกรอต[cite: 1]</td>
                                <td class="py-3 px-4">นักวิชาการคอมพิวเตอร์ชำนาญการ[cite: 1]</td>
                                <td class="py-3 px-4">หัวหน้าฝ่ายพัฒนาระบบงานกองทุนประกันสังคม[cite: 1]</td>
                                <td class="py-3 px-4">กลุ่มงานพัฒนาระบบสารสนเทศ[cite: 1]</td>
                            </tr>
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นายไกรรัฐ อาภาบุษยพันธุ์[cite: 1]</td>
                                <td class="py-3 px-4">นักวิชาการคอมพิวเตอร์ชำนาญการ[cite: 1]</td>
                                <td class="py-3 px-4">รักษาการ ผอ.กลุ่มงาน[cite: 1]</td>
                                <td class="py-3 px-4">กลุ่มงานบริหารจัดการระบบคอมพิวเตอร์และประมวลผล[cite: 1]</td>
                            </tr>
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นายธนวัต สาธานนท์[cite: 1]</td>
                                <td class="py-3 px-4">นักวิชาการคอมพิวเตอร์ชำนาญการพิเศษ[cite: 1]</td>
                                <td class="py-3 px-4">ผอ.กลุ่มงาน[cite: 1]</td>
                                <td class="py-3 px-4">กลุ่มงานบริหารเครือข่ายสื่อสารและความมั่นคงคอมพิวเตอร์[cite: 1]</td>
                            </tr>
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นายธนากร ชัยวิชู[cite: 1]</td>
                                <td class="py-3 px-4">นักวิชาการคอมพิวเตอร์ชำนาญการ[cite: 1]</td>
                                <td class="py-3 px-4">รักษาการ ผอ.กลุ่มงาน / หัวหน้าฝ่าย[cite: 1]</td>
                                <td class="py-3 px-4">กลุ่มงานบริการเทคโนโลยีสารสนเทศ[cite: 1]</td>
                            </tr>
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นายธนพัฒน์ บริรักษ์[cite: 1]</td>
                                <td class="py-3 px-4">นักวิชาการคอมพิวเตอร์ชำนาญการพิเศษ[cite: 1]</td>
                                <td class="py-3 px-4">ผอ.กลุ่มงาน / หัวหน้าฝ่าย[cite: 1]</td>
                                <td class="py-3 px-4">กลุ่มงานบริการอิเล็กทรอนิกส์[cite: 1]</td>
                            </tr>
                            <tr class="hover:bg-slate-50">
                                <td class="py-3 px-4 font-semibold text-slate-900">นางสาวรตา หมัดโต๊ะหมัน[cite: 1]</td>
                                <td class="py-3 px-4">นักจัดการงานทั่วไปชำนาญการ[cite: 1]</td>
                                <td class="py-3 px-4">หัวหน้าฝ่ายบริหารทั่วไป[cite: 1]</td>
                                <td class="py-3 px-4">ฝ่ายบริหารทั่วไป[cite: 1]</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>

        </div>

        <!-- ================= PAGE 2: GROUP RESPONSIBILITIES ================= -->
        <div id="page-responsibilities" class="space-y-8 hidden">
            
            <div class="bg-blue-900 text-white p-6 rounded-2xl shadow-sm">
                <h2 class="text-xl font-bold">ขอบเขตหน้าที่และความรับผิดชอบของแต่ละกลุ่มงาน[cite: 1]</h2>
                <p class="text-sm text-blue-200 mt-1">อ้างอิงตามคำสั่งสำนักบริหารเทคโนโลยีสารสนเทศ เรื่อง มอบหมายหน้าที่ความรับผิดชอบให้ข้าราชการ ลูกจ้างประจำ พนักงานราชการ และพนักงานประกันสังคม[cite: 1]</p>
            </div>

            <!-- Group 0: Senior Expert -->
            <div class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm space-y-3">
                <div class="flex items-center gap-3 border-b pb-3">
                    <span class="p-2 bg-amber-100 text-amber-800 rounded-lg text-lg">🎓</span>
                    <div>
                        <h3 class="text-base font-bold text-slate-900">ตำแหน่งนักวิชาการคอมพิวเตอร์เชี่ยวชาญ (ผู้เชี่ยวชาญกำกับดูแล)[cite: 1]</h3>
                        <p class="text-xs text-slate-500">นายเทวัญ แก้วศักดาศิริ[cite: 1]</p>
                    </div>
                </div>
                <ul class="list-disc list-inside text-sm text-slate-600 space-y-1.5 pl-2">
                    <li>กำกับ ควบคุม ดูแลกลุ่มงานบริหารจัดการระบบคอมพิวเตอร์และประมวลผล และกลุ่มงานบริหารเครือข่ายสื่อสารและความมั่นคงคอมพิวเตอร์[cite: 1]</li>
                    <li>ศึกษา ทดลอง วิเคราะห์ สังเคราะห์การพัฒนาระบบคอมพิวเตอร์ เครือข่าย และระบบบริการอิเล็กทรอนิกส์[cite: 1]</li>
                    <li>ให้คำปรึกษา แนะนำ กำหนดมาตรฐานและหลักเกณฑ์การออกแบบ ติดตั้งระบบฐานข้อมูล และระบบความมั่นคงปลอดภัย[cite: 1]</li>
                    <li>เสนอความเห็นการจัดทำแผนแม่บทและแผนยุทธศาสตร์ด้านเทคโนโลยีสารสนเทศและการสื่อสารของหน่วยงาน[cite: 1]</li>
                </ul>
            </div>

            <!-- Group 1 -->
            <div class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm space-y-4">
                <div class="flex items-center gap-3 border-b pb-3">
                    <span class="p-2 bg-blue-100 text-blue-800 rounded-lg text-lg">💻</span>
                    <div>
                        <h3 class="text-base font-bold text-slate-900">1. กลุ่มงานพัฒนาระบบสารสนเทศ[cite: 1]</h3>
                        <p class="text-xs text-slate-500">ผู้อำนวยการกลุ่มงาน: นายนัฐพงษ์ บุญวงศ์[cite: 1]</p>
                    </div>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-4 text-xs">
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายพัฒนาระบบงานกองทุนประกันสังคม[cite: 1]</p>
                        <p class="text-slate-600">ศึกษา วิเคราะห์ ออกแบบ พัฒนา และบำรุงรักษาระบบประกันสังคม (ม.33, 39, 40) ระบบทะเบียนนายจ้าง ผู้ประกันตน เงินสมทบ สิทธิประโยชน์ บัญชี และการเงิน[cite: 1]</p>
                    </div>
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายพัฒนาระบบงานกองทุนเงินทดแทน[cite: 1]</p>
                        <p class="text-slate-600">ศึกษา ออกแบบ และพัฒนาระบบกองทุนเงินทดแทน ระบบเงินสมทบ ค่าตอบแทนแพทย์ ศูนย์ฟื้นฟู ระบบว่างงาน และงานคณะกรรมการที่เกี่ยวข้อง[cite: 1]</p>
                    </div>
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายพัฒนาระบบงานสนับสนุน[cite: 1]</p>
                        <p class="text-slate-600">พัฒนาระบบสนับสนุน เช่น UMS, RPA, Queue, HRD, WPD, Intranet, EDOC, Webmail, e-Receipt, ERP, DPIS6 และระบบดิจิทัล IDP[cite: 1]</p>
                    </div>
                </div>
            </div>

            <!-- Group 2 -->
            <div class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm space-y-4">
                <div class="flex items-center gap-3 border-b pb-3">
                    <span class="p-2 bg-indigo-100 text-indigo-800 rounded-lg text-lg">🖥️</span>
                    <div>
                        <h3 class="text-base font-bold text-slate-900">2. กลุ่มงานบริหารจัดการระบบคอมพิวเตอร์และประมวลผล[cite: 1]</h3>
                        <p class="text-xs text-slate-500">รักษาการผู้อำนวยการกลุ่มงาน: นายไกรรัฐ อาภาบุษยพันธุ์[cite: 1]</p>
                    </div>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-4 text-xs">
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายระบบเครื่องคอมพิวเตอร์แม่ข่าย[cite: 1]</p>
                        <p class="text-slate-600">บริหารทรัพยากรเครื่องแม่ข่าย ดูแลศูนย์คอมพิวเตอร์หลัก (Main Site) และศูนย์สำรอง (DR Site) สำรองและกู้คืนระบบ (System Backup & Recovery)[cite: 1]</p>
                    </div>
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายซอฟต์แวร์ระบบ[cite: 1]</p>
                        <p class="text-slate-600">บริหารและควบคุมระบบฐานข้อมูล ซอฟต์แวร์ระบบ ควบคุม Performance และดูแลด้าน Security Management[cite: 1]</p>
                    </div>
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายปฏิบัติการประมวลผล[cite: 1]</p>
                        <p class="text-slate-600">ควบคุมการทำงานประมวลผลระบบงานประกันสังคม ดูแลระบบ Online และบริหารจัดการห้อง Data Center ตามมาตรฐานสากล[cite: 1]</p>
                    </div>
                </div>
            </div>

            <!-- Group 3 -->
            <div class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm space-y-4">
                <div class="flex items-center gap-3 border-b pb-3">
                    <span class="p-2 bg-emerald-100 text-emerald-800 rounded-lg text-lg">🛡️</span>
                    <div>
                        <h3 class="text-base font-bold text-slate-900">3. กลุ่มงานบริหารเครือข่ายสื่อสารและความมั่นคงคอมพิวเตอร์[cite: 1]</h3>
                        <p class="text-xs text-slate-500">ผู้อำนวยการกลุ่มงาน: นายธนวัต สาธานนท์[cite: 1]</p>
                    </div>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-4 text-xs">
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายบริหารจัดการเครือข่าย[cite: 1]</p>
                        <p class="text-slate-600">ดูแลระบบโครงข่าย LAN/WAN ทั่วประเทศ, ระบบประชุมทางไกล (Video Conference), ศูนย์รับแจ้งปัญหา IT Helpdesk และอุปกรณ์ลูกข่าย[cite: 1]</p>
                    </div>
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายบริหารจัดการความมั่นคงปลอดภัยคอมพิวเตอร์[cite: 1]</p>
                        <p class="text-slate-600">รับมือและแก้ปัญหาเหตุการณ์ความมั่นคงทางไซเบอร์ ควบคุมการเข้าถึงเครือข่าย ตรวจสอบช่องโหว่ระบบคอมพิวเตอร์[cite: 1]</p>
                    </div>
                    <div class="p-4 bg-slate-50 rounded-xl border border-slate-200">
                        <p class="font-bold text-slate-800 mb-1">ฝ่ายกำกับมาตรฐานความมั่นคงปลอดภัยคอมพิวเตอร์[cite: 1]</p>
                        <p class="text-slate-600">บริหารความเสี่ยงด้านสารสนเทศ กำกับมาตรฐานให้เป็นไปตามกฎหมาย นโยบายความปลอดภัยไซเบอร์และมาตรฐานสากล[cite: 1]</p>
                    </div>
                </div>
            </div>

            <!-- Group 4 & 5 & Admin -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm space-y-3">
                    <h3 class="text-base font-bold text-slate-900 border-b pb-2">4. กลุ่มงานบริการเทคโนโลยีสารสนเทศ[cite: 1]</h3>
                    <p class="text-xs text-slate-500">รักษาการ ผอ.: นายธนากร ชัยวิชู[cite: 1]</p>
                    <ul class="text-xs text-slate-600 space-y-2">
                        <li><strong>ฝ่ายวางแผนเทคโนโลยีสารสนเทศ:</strong> จัดทำแผนปฏิบัติการดิจิทัล, งานเลขานุการคณะอนุกรรมการฯ, ฝึกอบรม ICT และรายงานทุนหมุนเวียน/ความเสี่ยง[cite: 1]</li>
                        <li><strong>ฝ่ายวิชาการและสถาปัตยกรรมองค์กร:</strong> จัดทำ Enterprise Architecture (EA), ประเมิน PMQA 4.0, GECC และเสนอโครงการต่อกระทรวงแรงงาน[cite: 1]</li>
                    </ul>
                </div>

                <div class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm space-y-3">
                    <h3 class="text-base font-bold text-slate-900 border-b pb-2">5. กลุ่มงานบริการอิเล็กทรอนิกส์[cite: 1]</h3>
                    <p class="text-xs text-slate-500">ผอ.: นายธนพัฒน์ บริรักษ์[cite: 1]</p>
                    <ul class="text-xs text-slate-600 space-y-2">
                        <li><strong>ฝ่ายบริการอิเล็กทรอนิกส์:</strong> พัฒนาระบบ e-Services, e-Self Service, Line Official และระบบดิจิทัลภาครัฐ[cite: 1]</li>
                        <li><strong>ฝ่ายบูรณาการข้อมูลอิเล็กทรอนิกส์:</strong> พัฒนาระบบ Big Data, Data Catalog, Linkage Center และธรรมาภิบาลข้อมูล (Data Governance)[cite: 1]</li>
                    </ul>
                </div>

                <div class="bg-white p-6 rounded-2xl border border-slate-200 shadow-sm space-y-3">
                    <h3 class="text-base font-bold text-slate-900 border-b pb-2">6. ฝ่ายบริหารทั่วไป[cite: 1]</h3>
                    <p class="text-xs text-slate-500">หัวหน้าฝ่าย: นางสาวรตา หมัดโต๊ะหมัน[cite: 1]</p>
                    <ul class="text-xs text-slate-600 space-y-2">
                        <li><strong>งานสารบรรณ & ธุรการ:</strong> รับ-ส่งหนังสือ จัดเก็บเอกสาร[cite: 1]</li>
                        <li><strong>งานบริหารบุคคล:</strong> ทะเบียนประวัติและการประเมินผล[cite: 1]</li>
                        <li><strong>งานการเงิน งบประมาณ พัสดุ & ยานพาหนะ:</strong> เบิกจ่าย ดูแลครุภัณฑ์ และสถานที่[cite: 1]</li>
                    </ul>
                </div>
            </div>

        </div>

    </main>

    <!-- Footer -->
    <footer class="bg-slate-900 text-slate-400 py-4 text-center text-xs border-t border-slate-800">
        สำนักบริหารเทคโนโลยีสารสนเทศ สำนักงานประกันสังคม[cite: 1]
    </footer>

    <!-- JavaScript for Interactivity -->
    <script>
        // Tab Switcher
        function switchTab(tab) {
            const pageChart = document.getElementById('page-chart');
            const pageResp = document.getElementById('page-responsibilities');
            const btnChart = document.getElementById('tab-chart');
            const btnResp = document.getElementById('tab-resp');

            if (tab === 'chart') {
                pageChart.classList.remove('hidden');
                pageResp.classList.add('hidden');
                btnChart.classList.add('active');
                btnResp.classList.remove('active');
            } else {
                pageChart.classList.add('hidden');
                pageResp.classList.remove('hidden');
                btnResp.classList.add('active');
                btnChart.classList.remove('active');
            }
        }

        // Table Filter Search
        function filterDirectory() {
            let input = document.getElementById("searchInput");
            let filter = input.value.toUpperCase();
            let table = document.getElementById("directoryTable");
            let tr = table.getElementsByTagName("tr");

            for (let i = 1; i < tr.length; i++) {
                let tdArray = tr[i].getElementsByTagName("td");
                let match = false;
                for (let j = 0; j < tdArray.length; j++) {
                    if (tdArray[j]) {
                        if (tdArray[j].innerText.toUpperCase().indexOf(filter) > -1) {
                            match = true;
                            break;
                        }
                    }
                }
                tr[i].style.display = match ? "" : "none";
            }
        }

        // Initialize Chart.js
        window.onload = function() {
            const ctx = document.getElementById('workforceChart').getContext('2d');
            new Chart(ctx, {
                type: 'doughnut',
                data: {
                    labels: [
                        'กลุ่มพัฒนาระบบสารสนเทศ',
                        'กลุ่มบริหารระบบคอมพิวเตอร์ฯ',
                        'กลุ่มบริหารเครือข่ายฯ',
                        'กลุ่มบริการเทคโนโลยีสารสนเทศ',
                        'กลุ่มบริการอิเล็กทรอนิกส์',
                        'ฝ่ายบริหารทั่วไป'
                    ],
                    datasets: [{
                        data: [17, 8, 10, 4, 8, 10],
                        backgroundColor: [
                            '#2563eb',
                            '#4f46e5',
                            '#059669',
                            '#d97706',
                            '#0891b2',
                            '#64748b'
                        ]
                    }]
                },
                options: {
                    responsive: true,
                    plugins: {
                        legend: {
                            position: 'bottom',
                            labels: { font: { family: 'Prompt', size: 11 } }
                        }
                    }
                }
            });
        };
    </script>
</body>
</html>
