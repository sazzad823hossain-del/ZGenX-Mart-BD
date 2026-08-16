<p style="text-align: left;"><a title="ZGenX Mart BD  &quot;নতুন প্রজন্মের লাইফস্টাইল পার্টনার&quot; (Lifestyle Partner for the New Gen)" href="#header-title">ZGenX Mart BD</a></p>
<header>
<div class="header-container"><img id="header-logo" class="logo-preview" style="display: none;" alt="ZGenX Mart BD Logo" />
<h1 id="header-title">ZGenX Mart BD</h1>
<p id="header-tagline">আয়-ব্যয় ট্র্যাকার ও প্রফেশনাল ক্যাশ মেমো জেনারেটর</p>
</div>
</header>
<div class="container"><!-- Quick Settings Box for Company Name & Logo -->
<div class="branding-card no-print">
<h3>⚙️ কোম্পানির নাম ও লোগো সেটআপ করুন</h3>
<div class="form-row">
<div class="form-group"><label>কোম্পানির নাম</label> <input id="setting-company-name" class="form-control" type="text" value="ZGenX Mart BD" /></div>
<div class="form-group"><label>লোগো ছবি সিলেক্ট করুন (Mobile/Computer থেকে)</label> <input id="setting-logo-file" class="form-control" accept="image/*" type="file" /></div>
</div>
<button class="btn btn-secondary">সেটিংস সেভ করুন</button></div>
<!-- Tab Navigation -->
<div class="tabs no-print"><button class="tab-btn active">ড্যাশবোর্ড &amp; আয়-ব্যয়</button> <button class="tab-btn">মেমো / ইনভয়েস তৈরি</button> <button class="tab-btn">পণ্য তালিকা</button> <button class="tab-btn">গ্রাহক তালিকা</button></div>
<!-- 1. DASHBOARD TAB -->
<div id="dashboard" class="tab-content active">
<div class="stats-grid">
<div class="stat-card">
<h3>মোট আয়</h3>
<div class="amount" style="color: var(--primary);">৳ <span id="stat-income">0</span></div>
</div>
<div class="stat-card expense">
<h3>মোট ব্যয়</h3>
<div class="amount" style="color: var(--secondary);">৳ <span id="stat-expense">0</span></div>
</div>
<div class="stat-card balance">
<h3>বর্তমান ব্যালেন্স</h3>
<div class="amount" style="color: var(--accent);">৳ <span id="stat-balance">0</span></div>
</div>
</div>
<div class="card">
<h2 class="card-title">নতুন আয় / ব্যয় এন্ট্রি করুন</h2>
<form id="cashbook-form">
<div class="form-row">
<div class="form-group"><label>তারিখ</label> <input id="cb-date" class="form-control" required="" type="date" /></div>
<div class="form-group"><label>টাইপ</label><select id="cb-type" class="form-control" required="">
<option value="income">আয় (Income)</option>
<option value="expense">ব্যয় (Expense)</option>
</select></div>
<div class="form-group"><label>টাকার পরিমাণ (৳)</label> <input id="cb-amount" class="form-control" required="" type="number" placeholder="0" /></div>
</div>
<div class="form-group"><label>বিবরণ / নোট</label> <input id="cb-note" class="form-control" required="" type="text" placeholder="যেমন: পণ্য বিক্রয় বা ডেলিভারি চার্জ" /></div>
<button class="btn" type="submit">এন্ট্রি সেভ করুন</button></form></div>
<div class="card">
<h2 class="card-title">সাম্প্রতিক আয়-ব্যয়ের হিসাব</h2>
<table>
<thead>
<tr>
<th>তারিখ</th>
<th>টাইপ</th>
<th>বিবরণ</th>
<th>পরিমাণ</th>
<th>অ্যাকশন</th>
</tr>
</thead>
<tbody id="cashbook-table-body"></tbody>
</table>
</div>
</div>
<!-- 2. INVOICE TAB -->
<div id="invoice" class="tab-content">
<div class="card no-print">
<h2 class="card-title">মেমো জেনারেটর ফরম</h2>
<form id="invoice-form">
<div class="form-row">
<div class="form-group"><label>গ্রাহকের নাম</label> <input id="inv-customer" class="form-control" required="" type="text" placeholder="গ্রাহকের নাম" /></div>
<div class="form-group"><label>ফোন নম্বর</label> <input id="inv-phone" class="form-control" type="text" placeholder="017xxxxxxxx" /></div>
<div class="form-group"><label>তারিখ</label> <input id="inv-date" class="form-control" required="" type="date" /></div>
</div>
<div class="form-group"><label>গ্রাহকের ঠিকানা</label> <input id="inv-address" class="form-control" type="text" placeholder="জেলা, উপজেলা বা বিস্তারিত ঠিকানা" /></div>
<div style="border: 1px solid var(--border); padding: 15px; border-radius: 6px; margin-bottom: 15px; background: #fafafa;">
<h4 style="margin-bottom: 10px; color: var(--primary);">আইটেম যুক্ত করুন</h4>
<div class="form-row">
<div class="form-group" style="flex: 2;"><label>পণ্যের নাম</label> <input id="inv-item-name" class="form-control" type="text" placeholder="পণ্যের নাম" /></div>
<div class="form-group"><label>পরিমাণ</label> <input id="inv-item-qty" class="form-control" min="1" type="number" value="1" /></div>
<div class="form-group"><label>একক মূল্য (৳)</label> <input id="inv-item-price" class="form-control" type="number" placeholder="0" /></div>
</div>
<button class="btn" style="background-color: #333;" type="button">+ আইটেম যোগ করুন</button></div>
<div class="form-row">
<div class="form-group"><label>ডেলিভারি চার্জ (৳)</label> <input id="inv-delivery" class="form-control" type="number" value="0" /></div>
<div class="form-group"><label>ডিসকাউন্ট (৳)</label> <input id="inv-discount" class="form-control" type="number" value="0" /></div>
</div>
<button class="btn btn-block" type="button">মেমো তৈরি করুন</button></form></div>
<!-- Printable Invoice -->
<div id="printable-area" class="invoice-box" style="display: none;">
<div class="invoice-header">
<div style="display: flex; align-items: center; gap: 15px;"><img id="memo-logo" style="height: 60px; max-width: 150px; object-fit: contain; display: none;" alt="Logo" />
<div>
<div id="memo-company-name" class="invoice-title">ZGenX Mart BD</div>
<p style="color: #666; font-size: 13px;">অর্ডার ও ক্যাশ মেমো</p>
</div>
</div>
<div style="text-align: right;">
<p><strong>তারিখ:</strong> <span id="memo-date"></span></p>
<p><strong>মেমো নং:</strong> #<span id="memo-id"></span></p>
</div>
</div>
<div style="margin-bottom: 20px; line-height: 1.6;">
<p><strong>গ্রাহকের নাম:</strong> <span id="memo-customer"></span></p>
<p><strong>ফোন:</strong> <span id="memo-phone"></span></p>
<p><strong>ঠিকানা:</strong> <span id="memo-address"></span></p>
</div>
<table>
<thead>
<tr>
<th>পণ্যের নাম</th>
<th>পরিমাণ</th>
<th>মূল্য</th>
<th>মোট (৳)</th>
</tr>
</thead>
<tbody id="memo-items-body"></tbody>
</table>
<div style="margin-top: 20px; text-align: right; line-height: 1.8;">
<p>সাবটোটাল: ৳ <span id="memo-subtotal">0</span></p>
<p>ডেলিভারি চার্জ: ৳ <span id="memo-delivery">0</span></p>
<p>ডিসকাউন্ট: -৳ <span id="memo-discount">0</span></p>
<h3 style="color: var(--primary); margin-top: 5px;">সর্বমোট প্রদেয়: ৳ <span id="memo-grand-total">0</span></h3>
</div>
<div style="margin-top: 40px; text-align: center; border-top: 1px dashed #ccc; padding-top: 15px; font-size: 13px; color: #777;">ZGenX Mart BD "নতুন প্রজন্মের লাইফস্টাইল পার্টনার" (Lifestyle Partner for the New Gen) ধন্যবাদ, আমাদের সাথে কেনাকাটা করার জন্য!</div>
</div>
<div id="print-btn-container" class="no-print" style="text-align: center; margin-top: 20px; display: none;"><button class="btn">মেমো প্রিন্ট / PDF সেভ করুন</button></div>
</div>
<!-- 3. PRODUCTS TAB -->
<div id="products" class="tab-content">
<div class="card">
<h2 class="card-title">নতুন পণ্য যুক্ত করুন</h2>
<form id="product-form">
<div class="form-row">
<div class="form-group" style="flex: 2;"><label>পণ্যের নাম</label> <input id="p-name" class="form-control" required="" type="text" placeholder="যেমন: স্কিন কেয়ার সিরাম" /></div>
<div class="form-group"><label>বিক্রয় মূল্য (৳)</label> <input id="p-price" class="form-control" required="" type="number" placeholder="0" /></div>
</div>
<button class="btn" type="submit">পণ্য যোগ করুন</button></form></div>
<div class="card">
<h2 class="card-title">পণ্য তালিকা</h2>
<table>
<thead>
<tr>
<th>পণ্যের নাম</th>
<th>মূল্য (৳)</th>
<th>অ্যাকশন</th>
</tr>
</thead>
<tbody id="product-table-body"></tbody>
</table>
</div>
</div>
<!-- 4. CUSTOMERS TAB -->
<div id="customers" class="tab-content">
<div class="card">
<h2 class="card-title">নতুন গ্রাহক যুক্ত করুন</h2>
<form id="customer-form">
<div class="form-row">
<div class="form-group"><label>গ্রাহকের নাম</label> <input id="c-name" class="form-control" required="" type="text" placeholder="নাম" /></div>
<div class="form-group"><label>ফোন নম্বর</label> <input id="c-phone" class="form-control" required="" type="text" placeholder="মোবাইল নম্বর" /></div>
</div>
<div class="form-group"><label>ঠিকানা</label> <input id="c-address" class="form-control" type="text" placeholder="জেলা, উপজেলা বা বিস্তারিত ঠিকানা" /></div>
<button class="btn" type="submit">গ্রাহক সেভ করুন</button></form></div>
<div class="card">
<h2 class="card-title">গ্রাহকদের তালিকা</h2>
<table>
<thead>
<tr>
<th>নাম</th>
<th>ফোন নম্বর</th>
<th>ঠিকানা</th>
<th>অ্যাকশন</th>
</tr>
</thead>
<tbody id="customer-table-body"></tbody>
</table>
</div>
</div>
</div>
