CREATE TABLE visit_reservations (
    id INT AUTO_INCREMENT PRIMARY KEY,
    visit_date DATE NOT NULL,
    visit_time VARCHAR(20) NOT NULL,
    organization VARCHAR(100) NOT NULL,
    contact_name VARCHAR(50) NOT NULL,
    phone VARCHAR(30) NOT NULL,
    email VARCHAR(100),
    people_count INT NOT NULL,
    elderly_count INT DEFAULT 0,
    disability_count INT DEFAULT 0,
    need_guide BOOLEAN DEFAULT FALSE,
    purpose TEXT,
    special_needs TEXT,
    note TEXT,
    status VARCHAR(20) DEFAULT 'pending',
    admin_note TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);<form action="submit.php" method="POST">

    <label>參訪日期</label>
    <input type="date" name="visit_date" required>

    <label>參訪時段</label>
    <select name="visit_time" required>
        <option value="">請選擇</option>
        <option value="09:00-10:00">09:00-10:00</option>
        <option value="10:00-11:00">10:00-11:00</option>
        <option value="14:00-15:00">14:00-15:00</option>
        <option value="15:00-16:00">15:00-16:00</option>
    </select>

    <label>參訪單位</label>
    <input type="text" name="organization" required>

    <label>聯絡人</label>
    <input type="text" name="contact_name" required>

    <label>電話</label>
    <input type="tel" name="phone" required>

    <label>Email</label>
    <input type="email" name="email">

    <label>參訪人數</label>
    <input type="number" name="people_count" min="1" required>

    <label>參訪目的</label>
    <textarea name="purpose"></textarea>

    <label>特殊需求</label>
    <textarea name="special_needs"></textarea>

    <button type="submit">送出預約</button>

</form>
