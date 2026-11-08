代发 wailian999

TS:   crypto.randomUUID()
来源：https://xi.zhonguo5118.cn

Java: UUID.randomUUID().toString()
来源：https://mj.zhonguo4118.cn

Go:   // 用 github.com/google/uuid
来源：https://xy.zhonguo3118.cn

Ruby: SecureRandom.uuid
来源：https://xu.zhonguo3118.cn

C#:   Guid.NewGuid().ToString()
来源：https://qt.zhonguo7118.cn

[P02] MD5 / SHA256 摘要
来源：https://pq.zhonguo7118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://nt.zhonguo8118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://go.zhonguo8118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://ei.zhonguo6118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://sk.zhonguo4118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://gl.zhonguo7118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://lm.zhonguo2118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://ps.zhonguo8118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://sa.zhonguo3118.cn

[P03] 生成短随机字符串
来源：https://do.zhonguo3118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://no.zhonguo2118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://md.zhonguo4118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://ts.zhonguo4118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://ha.zhonguo1118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://oc.zhonguo2118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://pe.zhonguo8118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://hl.zhonguo2118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://rw.zhonguo6118.cn

[P04] 求长度
来源：https://fd.zhonguo8118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://zv.zhonguo5118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://en.zhonguo7118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://bj.zhonguo3118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://ya.zhonguo4118.cn

Java: list.size();  map.size();  s.length()
来源：https://bm.zhonguo3118.cn

Go:   len(arr);  len(m)
来源：https://jj.zhonguo5118.cn

Ruby: x.length;  x.size
来源：https://nz.zhonguo8118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://mf.zhonguo5118.cn

[P05] 判断两个对象内容是否相等
来源：https://gj.zhonguo7118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://aa.zhonguo4118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://vt.zhonguo6118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://xq.zhonguo7118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://bm.zhonguo1118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://ey.zhonguo4118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://yx.zhonguo6118.cn

Ruby: a == b
来源：https://yg.zhonguo7118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://do.zhonguo8118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://al.zhonguo3118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://wv.zhonguo7118.cn

PHP:  if (empty($x)) {}
来源：https://ue.zhonguo4118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://ex.zhonguo2118.cn

TS:   if (x == null) {}
来源：https://mn.zhonguo5118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://am.zhonguo7118.cn

Go:   if x == nil {}
来源：https://ou.zhonguo5118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://fc.zhonguo8118.cn

C#:   if (x is null) {}
来源：https://ut.zhonguo7118.cn

[P07] 防抖与节流
来源：https://pj.zhonguo2118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://mw.zhonguo3118.cn

PHP:  // 手写时间戳比较
来源：https://yh.zhonguo2118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://sw.zhonguo5118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://dd.zhonguo3118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://py.zhonguo6118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://vv.zhonguo7118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://ca.zhonguo2118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://tp.zhonguo5118.cn

[P08] 处理浮点精度问题
来源：https://bm.zhonguo5118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://xw.zhonguo6118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://up.zhonguo1118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://cf.zhonguo2118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://dm.zhonguo4118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://xs.zhonguo3118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://gg.zhonguo3118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://pi.zhonguo4118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://jn.zhonguo7118.cn

================================================================================
来源：https://ii.zhonguo4118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://po.zhonguo6118.cn

================================================================================
来源：https://wz.zhonguo7118.cn

[Q01] 创建表
来源：https://xp.zhonguo3118.cn

CREATE TABLE users (
来源：https://xj.zhonguo2118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://dy.zhonguo3118.cn

name VARCHAR(50) NOT NULL,
来源：https://mc.zhonguo5118.cn

email VARCHAR(100) UNIQUE,
来源：https://ym.zhonguo2118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://la.zhonguo8118.cn

);
来源：https://or.zhonguo1118.cn

[Q02] 创建带外键的表
来源：https://vu.zhonguo4118.cn

CREATE TABLE orders (
来源：https://fa.zhonguo6118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://cn.zhonguo1118.cn

user_id INT NOT NULL,
来源：https://je.zhonguo6118.cn

amount DECIMAL(10, 2),
来源：https://ox.zhonguo6118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://qz.zhonguo4118.cn

);
来源：https://aw.zhonguo8118.cn

[Q03] 增加列
来源：https://yf.zhonguo6118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://ci.zhonguo6118.cn

[Q04] 修改列类型
来源：https://tx.zhonguo6118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://mi.zhonguo6118.cn

[Q05] 重命名列
来源：https://yx.zhonguo1118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://pk.zhonguo4118.cn

[Q06] 删除列
来源：https://fe.zhonguo5118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://ix.zhonguo4118.cn

[Q07] 删除表
来源：https://ss.zhonguo2118.cn

DROP TABLE IF EXISTS orders;
来源：https://tt.zhonguo1118.cn

[Q08] 创建普通索引
来源：https://uf.zhonguo5118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://nh.zhonguo7118.cn

[Q09] 创建唯一索引
来源：https://xe.zhonguo5118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://wh.zhonguo8118.cn

[Q10] 插入单行
来源：https://wd.zhonguo5118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://sg.zhonguo4118.cn

[Q11] 一次插入多行
来源：https://ip.zhonguo2118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://hz.zhonguo8118.cn

[Q12] 插入后取自增 ID
来源：https://kc.zhonguo5118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://nk.zhonguo3118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://ct.zhonguo8118.cn

[Q13] 忽略重复插入
来源：https://hv.zhonguo1118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://zs.zhonguo7118.cn

[Q14] 存在则更新（upsert）
来源：https://kk.zhonguo6118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://kl.zhonguo4118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://fr.zhonguo5118.cn

[Q15] 查询全部
来源：https://cb.zhonguo4118.cn

SELECT * FROM users;
来源：https://ic.zhonguo6118.cn

[Q16] 查询指定列
来源：https://ti.zhonguo3118.cn

SELECT id, name FROM users;
来源：https://ep.zhonguo1118.cn

[Q17] 条件查询
来源：https://do.zhonguo8118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://df.zhonguo8118.cn

[Q18] 模糊匹配
来源：https://hv.zhonguo3118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://xy.zhonguo4118.cn

[Q19] 范围查询
来源：https://et.zhonguo4118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://se.zhonguo7118.cn

[Q20] IN 列表
来源：https://cl.zhonguo1118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://ih.zhonguo7118.cn

[Q21] 空值判断
来源：https://se.zhonguo7118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://te.zhonguo3118.cn

[Q22] 排序
来源：https://oc.zhonguo3118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://ev.zhonguo8118.cn

[Q23] 分页
来源：https://cg.zhonguo4118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://tt.zhonguo7118.cn

[Q24] 去重
来源：https://rd.zhonguo8118.cn

SELECT DISTINCT city FROM users;
来源：https://iv.zhonguo3118.cn

[Q25] 只取前 N 条
来源：https://xf.zhonguo8118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://fi.zhonguo6118.cn

[Q26] 计数
来源：https://zj.zhonguo8118.cn

SELECT COUNT(*) FROM users;
来源：https://zw.zhonguo6118.cn

[Q27] 条件计数
来源：https://zn.zhonguo1118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://sd.zhonguo5118.cn

[Q28] 求和与平均
来源：https://si.zhonguo6118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://xu.zhonguo5118.cn

[Q29] 最大最小值
来源：https://zc.zhonguo5118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://bi.zhonguo3118.cn

[Q30] 分组统计
来源：https://fl.zhonguo6118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://ji.zhonguo4118.cn

[Q31] 分组后过滤
来源：https://nz.zhonguo8118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://yr.zhonguo6118.cn

[Q32] 分组拼接字符串
来源：https://xl.zhonguo4118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://la.zhonguo1118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://yx.zhonguo6118.cn

[Q33] 多列分组
来源：https://xy.zhonguo5118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://ay.zhonguo7118.cn

[Q34] 每组取第一条
来源：https://gv.zhonguo8118.cn

SELECT * FROM (
来源：https://ia.zhonguo8118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://lm.zhonguo4118.cn

) t WHERE rn = 1;
来源：https://ea.zhonguo7118.cn

[Q35] 内连接
来源：https://jb.zhonguo6118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://ud.zhonguo5118.cn

[Q36] 左连接
来源：https://od.zhonguo4118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://gq.zhonguo4118.cn

[Q37] 右连接
来源：https://ez.zhonguo1118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://vj.zhonguo1118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://mo.zhonguo1118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://nw.zhonguo6118.cn

[Q39] 自连接（查上下级）
来源：https://sb.zhonguo1118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://vc.zhonguo5118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://hp.zhonguo4118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://vw.zhonguo8118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://nv.zhonguo8118.cn

[Q41] 多表连接
来源：https://xn.zhonguo2118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://sz.zhonguo7118.cn

JOIN users u ON u.id = o.user_id
来源：https://gq.zhonguo5118.cn

JOIN products p ON p.id = o.product_id;
来源：https://gy.zhonguo1118.cn

[Q42] 连接条件附加过滤
来源：https://ys.zhonguo6118.cn

SELECT u.name, o.amount FROM users u
来源：https://bv.zhonguo8118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://on.zhonguo5118.cn

[Q43] 标量子查询
来源：https://id.zhonguo5118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://lv.zhonguo4118.cn

[Q44] IN 子查询
来源：https://px.zhonguo5118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://lz.zhonguo5118.cn

[Q45] EXISTS 判断存在
来源：https://ar.zhonguo6118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://kw.zhonguo2118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://bx.zhonguo4118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://du.zhonguo5118.cn

[Q47] 与平均值比较
来源：https://dz.zhonguo1118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://ok.zhonguo5118.cn

[Q48] CTE 公用表表达式
来源：https://jp.zhonguo3118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://bb.zhonguo3118.cn

SELECT * FROM t WHERE c > 5;
来源：https://fw.zhonguo7118.cn

[Q49] 更新单行
来源：https://oi.zhonguo2118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://jl.zhonguo5118.cn

[Q50] 批量更新
来源：https://zq.zhonguo6118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://zm.zhonguo1118.cn

[Q51] 用子查询更新
来源：https://wk.zhonguo2118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://qr.zhonguo8118.cn

[Q52] 删除指定行
来源：https://rd.zhonguo1118.cn

DELETE FROM users WHERE id = 10;
来源：https://di.zhonguo8118.cn

[Q53] 按条件删除
来源：https://ew.zhonguo1118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://lc.zhonguo4118.cn

[Q54] 清空表
来源：https://vv.zhonguo4118.cn

TRUNCATE TABLE logs;
来源：https://dr.zhonguo2118.cn

[Q55] 排名（并列占位）
来源：https://cr.zhonguo7118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://xy.zhonguo2118.cn

[Q56] 密集排名（并列不占位）
来源：https://cw.zhonguo7118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://sk.zhonguo7118.cn

[Q57] 行号
来源：https://ks.zhonguo4118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://jx.zhonguo7118.cn

[Q58] 累计求和
来源：https://la.zhonguo2118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://kb.zhonguo7118.cn

[Q59] 分组内累计
来源：https://qa.zhonguo2118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://pv.zhonguo4118.cn

[Q60] 取上一行 / 下一行
来源：https://bn.zhonguo8118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://dq.zhonguo8118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://rt.zhonguo3118.cn

[Q61] 移动平均
来源：https://ij.zhonguo5118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://am.zhonguo5118.cn

[Q62] 分组占比
来源：https://pj.zhonguo7118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://vx.zhonguo7118.cn

[Q63] 开启事务
来源：https://om.zhonguo5118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://yz.zhonguo2118.cn

[Q64] 提交事务
来源：https://no.zhonguo7118.cn

COMMIT;
来源：https://zi.zhonguo2118.cn

[Q65] 回滚事务
来源：https://ce.zhonguo8118.cn

ROLLBACK;
来源：https://qr.zhonguo2118.cn

[Q66] 行锁查询
来源：https://lb.zhonguo6118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://xs.zhonguo6118.cn

[Q67] 设置隔离级别
来源：https://gv.zhonguo8118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://hq.zhonguo8118.cn

[Q68] 保存点
来源：https://kx.zhonguo7118.cn

SAVEPOINT sp1;
来源：https://gm.zhonguo7118.cn

ROLLBACK TO sp1;
来源：https://ay.zhonguo5118.cn

[Q69] 查看执行计划
来源：https://bl.zhonguo4118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://hi.zhonguo1118.cn

[Q70] 更新统计信息
来源：https://yf.zhonguo8118.cn

ANALYZE TABLE users;
来源：https://mx.zhonguo6118.cn

[Q71] 查看建表语句
来源：https://nq.zhonguo7118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://wc.zhonguo2118.cn

[Q72] 查看索引
来源：https://ma.zhonguo4118.cn

SHOW INDEX FROM users;
来源：https://vs.zhonguo5118.cn

[Q73] 查看表状态
来源：https://pq.zhonguo5118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://xy.zhonguo2118.cn

[Q74] 强制使用索引
来源：https://nf.zhonguo8118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://sw.zhonguo2118.cn

[Q75] 日期格式化
来源：https://as.zhonguo6118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://xw.zhonguo6118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://gy.zhonguo8118.cn

[Q76] 按天统计
来源：https://of.zhonguo8118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://zs.zhonguo8118.cn

[Q77] 时间加减
来源：https://te.zhonguo6118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://wj.zhonguo6118.cn

[Q78] 当前时间
来源：https://ic.zhonguo3118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://eb.zhonguo3118.cn

[Q79] 字符串拼接
来源：https://tu.zhonguo5118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://yd.zhonguo5118.cn

[Q80] 字符串截取
来源：https://vv.zhonguo1118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://it.zhonguo8118.cn

[Q81] 字符串替换
来源：https://nw.zhonguo2118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://bu.zhonguo8118.cn

[Q82] 字符长度与字节长度
来源：https://uk.zhonguo5118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://me.zhonguo7118.cn

[Q83] 大小写转换
来源：https://zh.zhonguo5118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://ub.zhonguo6118.cn

[Q84] 去除首尾空格
来源：https://cg.zhonguo8118.cn

SELECT TRIM(name) FROM users;
来源：https://ug.zhonguo1118.cn

[Q85] 数值取整
来源：https://ld.zhonguo1118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://zj.zhonguo2118.cn

[Q86] 读取 JSON 字段
来源：https://wm.zhonguo3118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://bj.zhonguo4118.cn

[Q87] JSON 字段做条件
来源：https://ze.zhonguo7118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://ba.zhonguo5118.cn

[Q88] 行转列（条件聚合）
来源：https://uf.zhonguo7118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://ij.zhonguo6118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://yf.zhonguo2118.cn

[Q89] 判断表是否存在
来源：https://tt.zhonguo2118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://mv.zhonguo5118.cn

[Q90] 生成序号列
来源：https://fc.zhonguo4118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://jo.zhonguo2118.cn

================================================================================
来源：https://jv.zhonguo4118.cn

R. Bash 专题
来源：https://xo.zhonguo5118.cn

================================================================================
来源：https://sl.zhonguo4118.cn

[R01] shebang 与严格模式
来源：https://zu.zhonguo6118.cn

#!/usr/bin/env bash
来源：https://jw.zhonguo3118.cn

set -euo pipefail
来源：https://pe.zhonguo7118.cn

[R02] 变量赋值与使用
来源：https://ha.zhonguo6118.cn

name="Tom"; echo "$name"
来源：https://nw.zhonguo1118.cn

[R03] 只读变量
来源：https://vr.zhonguo8118.cn

readonly PI=3.14
来源：https://ml.zhonguo2118.cn

[R04] 位置参数
来源：https://hy.zhonguo7118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://uv.zhonguo6118.cn

[R05] 参数默认值
来源：https://ov.zhonguo4118.cn

name="${1:-default}"
来源：https://me.zhonguo8118.cn

[R06] 判断命令是否存在
来源：https://th.zhonguo1118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://zj.zhonguo6118.cn

[R07] if 判断文件
来源：https://gb.zhonguo4118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://oi.zhonguo5118.cn

[R08] 数值比较
来源：https://sa.zhonguo8118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://hh.zhonguo8118.cn

[R09] 字符串比较
来源：https://tu.zhonguo8118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://do.zhonguo7118.cn

[R10] 正则匹配
来源：https://rq.zhonguo2118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://ps.zhonguo8118.cn

[R11] case 多分支
来源：https://jo.zhonguo2118.cn


<!-- 参考信息 -->