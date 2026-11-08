代发 wailian999

TS:   crypto.randomUUID()
来源：https://uy.zhonguo7118.cn

Java: UUID.randomUUID().toString()
来源：https://hy.zhonguo6118.cn

Go:   // 用 github.com/google/uuid
来源：https://wq.zhonguo4118.cn

Ruby: SecureRandom.uuid
来源：https://gc.zhonguo1118.cn

C#:   Guid.NewGuid().ToString()
来源：https://sw.zhonguo2118.cn

[P02] MD5 / SHA256 摘要
来源：https://xb.zhonguo5118.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：https://ts.zhonguo5118.cn

PHP:  hash("sha256", $s);  md5($s);
来源：https://yl.zhonguo6118.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：https://ma.zhonguo4118.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：https://ku.zhonguo3118.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：https://iw.zhonguo5118.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：https://jz.zhonguo2118.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：https://yi.zhonguo3118.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：https://si.zhonguo5118.cn

[P03] 生成短随机字符串
来源：https://yb.zhonguo3118.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：https://qo.zhonguo5118.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：https://ky.zhonguo7118.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://la.zhonguo7118.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：https://rr.zhonguo7118.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：https://fr.zhonguo1118.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：https://ki.zhonguo4118.cn

Ruby: SecureRandom.alphanumeric(16)
来源：https://uv.zhonguo6118.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：https://hr.zhonguo6118.cn

[P04] 求长度
来源：https://nq.zhonguo3118.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：https://bt.zhonguo7118.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：https://go.zhonguo8118.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://lk.zhonguo1118.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：https://xa.zhonguo6118.cn

Java: list.size();  map.size();  s.length()
来源：https://sh.zhonguo5118.cn

Go:   len(arr);  len(m)
来源：https://ck.zhonguo2118.cn

Ruby: x.length;  x.size
来源：https://vr.zhonguo8118.cn

C#:   list.Count;  dict.Count;  s.Length
来源：https://zk.zhonguo1118.cn

[P05] 判断两个对象内容是否相等
来源：https://ws.zhonguo6118.cn

Py:   a == b              # 列表与字典递归比较内容
来源：https://wc.zhonguo4118.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：https://jx.zhonguo6118.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：https://xn.zhonguo2118.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：https://jq.zhonguo6118.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：https://cq.zhonguo5118.cn

Go:   reflect.DeepEqual(a, b)
来源：https://br.zhonguo7118.cn

Ruby: a == b
来源：https://bf.zhonguo7118.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：https://rb.zhonguo6118.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：https://ha.zhonguo8118.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：https://eb.zhonguo5118.cn

PHP:  if (empty($x)) {}
来源：https://rr.zhonguo1118.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：https://dw.zhonguo2118.cn

TS:   if (x == null) {}
来源：https://me.zhonguo8118.cn

Java: if (x == null || x.isEmpty()) {}
来源：https://sq.zhonguo5118.cn

Go:   if x == nil {}
来源：https://ci.zhonguo1118.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：https://de.zhonguo8118.cn

C#:   if (x is null) {}
来源：https://xx.zhonguo4118.cn

[P07] 防抖与节流
来源：https://wg.zhonguo7118.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：https://pb.zhonguo4118.cn

PHP:  // 手写时间戳比较
来源：https://sn.zhonguo1118.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://zr.zhonguo7118.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://hm.zhonguo5118.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：https://yw.zhonguo6118.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：https://sa.zhonguo3118.cn

Ruby: // 手写闭包 + Time.now 判断
来源：https://lp.zhonguo3118.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：https://gw.zhonguo3118.cn

[P08] 处理浮点精度问题
来源：https://cr.zhonguo7118.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：https://gh.zhonguo4118.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：https://hg.zhonguo8118.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：https://ki.zhonguo3118.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：https://ro.zhonguo8118.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：https://vl.zhonguo5118.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：https://im.zhonguo2118.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：https://lm.zhonguo7118.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：https://mr.zhonguo6118.cn

================================================================================
来源：https://tb.zhonguo8118.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：https://kx.zhonguo4118.cn

================================================================================
来源：https://ha.zhonguo7118.cn

[Q01] 创建表
来源：https://fm.zhonguo3118.cn

CREATE TABLE users (
来源：https://qq.zhonguo2118.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：https://tr.zhonguo5118.cn

name VARCHAR(50) NOT NULL,
来源：https://rd.zhonguo6118.cn

email VARCHAR(100) UNIQUE,
来源：https://kl.zhonguo6118.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：https://bh.zhonguo5118.cn

);
来源：https://nv.zhonguo3118.cn

[Q02] 创建带外键的表
来源：https://ox.zhonguo8118.cn

CREATE TABLE orders (
来源：https://nr.zhonguo5118.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：https://et.zhonguo8118.cn

user_id INT NOT NULL,
来源：https://je.zhonguo4118.cn

amount DECIMAL(10, 2),
来源：https://kp.zhonguo2118.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：https://yp.zhonguo5118.cn

);
来源：https://vm.zhonguo4118.cn

[Q03] 增加列
来源：https://hm.zhonguo2118.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：https://od.zhonguo4118.cn

[Q04] 修改列类型
来源：https://ju.zhonguo2118.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：https://lq.zhonguo8118.cn

[Q05] 重命名列
来源：https://eo.zhonguo7118.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：https://rj.zhonguo1118.cn

[Q06] 删除列
来源：https://xk.zhonguo3118.cn

ALTER TABLE users DROP COLUMN age;
来源：https://iv.zhonguo7118.cn

[Q07] 删除表
来源：https://xj.zhonguo8118.cn

DROP TABLE IF EXISTS orders;
来源：https://ck.zhonguo2118.cn

[Q08] 创建普通索引
来源：https://hq.zhonguo7118.cn

CREATE INDEX idx_users_email ON users(email);
来源：https://zy.zhonguo2118.cn

[Q09] 创建唯一索引
来源：https://fh.zhonguo4118.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：https://kn.zhonguo4118.cn

[Q10] 插入单行
来源：https://bw.zhonguo3118.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：https://az.zhonguo5118.cn

[Q11] 一次插入多行
来源：https://fp.zhonguo8118.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：https://sr.zhonguo3118.cn

[Q12] 插入后取自增 ID
来源：https://qj.zhonguo4118.cn

INSERT INTO users (name) VALUES ('C');
来源：https://ip.zhonguo7118.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：https://sa.zhonguo1118.cn

[Q13] 忽略重复插入
来源：https://ph.zhonguo5118.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：https://eg.zhonguo8118.cn

[Q14] 存在则更新（upsert）
来源：https://pj.zhonguo5118.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：https://ws.zhonguo7118.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：https://gh.zhonguo6118.cn

[Q15] 查询全部
来源：https://cq.zhonguo5118.cn

SELECT * FROM users;
来源：https://fa.zhonguo5118.cn

[Q16] 查询指定列
来源：https://eo.zhonguo4118.cn

SELECT id, name FROM users;
来源：https://ma.zhonguo1118.cn

[Q17] 条件查询
来源：https://su.zhonguo1118.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：https://yh.zhonguo7118.cn

[Q18] 模糊匹配
来源：https://nf.zhonguo3118.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：https://ez.zhonguo5118.cn

[Q19] 范围查询
来源：https://pa.zhonguo7118.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：https://de.zhonguo2118.cn

[Q20] IN 列表
来源：https://sz.zhonguo6118.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：https://lp.zhonguo3118.cn

[Q21] 空值判断
来源：https://om.zhonguo2118.cn

SELECT * FROM users WHERE email IS NULL;
来源：https://ho.zhonguo1118.cn

[Q22] 排序
来源：https://mw.zhonguo1118.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：https://rb.zhonguo1118.cn

[Q23] 分页
来源：https://ai.zhonguo1118.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：https://ne.zhonguo7118.cn

[Q24] 去重
来源：https://wa.zhonguo2118.cn

SELECT DISTINCT city FROM users;
来源：https://rd.zhonguo1118.cn

[Q25] 只取前 N 条
来源：https://iw.zhonguo8118.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：https://wy.zhonguo7118.cn

[Q26] 计数
来源：https://wf.zhonguo3118.cn

SELECT COUNT(*) FROM users;
来源：https://xz.zhonguo4118.cn

[Q27] 条件计数
来源：https://tf.zhonguo8118.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：https://ce.zhonguo2118.cn

[Q28] 求和与平均
来源：https://cq.zhonguo5118.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：https://wl.zhonguo5118.cn

[Q29] 最大最小值
来源：https://li.zhonguo1118.cn

SELECT MAX(age), MIN(age) FROM users;
来源：https://ws.zhonguo8118.cn

[Q30] 分组统计
来源：https://wm.zhonguo1118.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：https://dm.zhonguo4118.cn

[Q31] 分组后过滤
来源：https://ax.zhonguo4118.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：https://co.zhonguo2118.cn

[Q32] 分组拼接字符串
来源：https://bi.zhonguo7118.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：https://pc.zhonguo5118.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：https://iv.zhonguo5118.cn

[Q33] 多列分组
来源：https://kd.zhonguo6118.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：https://rw.zhonguo1118.cn

[Q34] 每组取第一条
来源：https://ti.zhonguo8118.cn

SELECT * FROM (
来源：https://jt.zhonguo4118.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：https://rl.zhonguo3118.cn

) t WHERE rn = 1;
来源：https://jr.zhonguo2118.cn

[Q35] 内连接
来源：https://qg.zhonguo3118.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：https://kl.zhonguo8118.cn

[Q36] 左连接
来源：https://fb.zhonguo6118.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：https://qb.zhonguo2118.cn

[Q37] 右连接
来源：https://ag.zhonguo3118.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：https://ya.zhonguo4118.cn

[Q38] 全外连接（PostgreSQL）
来源：https://df.zhonguo2118.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：https://md.zhonguo6118.cn

[Q39] 自连接（查上下级）
来源：https://bn.zhonguo1118.cn

SELECT e.name, m.name AS manager FROM employees e
来源：https://pz.zhonguo2118.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：https://pt.zhonguo2118.cn

[Q40] 交叉连接（笛卡尔积）
来源：https://rm.zhonguo1118.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：https://yr.zhonguo1118.cn

[Q41] 多表连接
来源：https://td.zhonguo5118.cn

SELECT o.id, u.name, p.title FROM orders o
来源：https://pe.zhonguo8118.cn

JOIN users u ON u.id = o.user_id
来源：https://ze.zhonguo4118.cn

JOIN products p ON p.id = o.product_id;
来源：https://uk.zhonguo6118.cn

[Q42] 连接条件附加过滤
来源：https://gy.zhonguo6118.cn

SELECT u.name, o.amount FROM users u
来源：https://zs.zhonguo6118.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：https://ke.zhonguo2118.cn

[Q43] 标量子查询
来源：https://mb.zhonguo8118.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：https://mt.zhonguo4118.cn

[Q44] IN 子查询
来源：https://xx.zhonguo2118.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：https://zl.zhonguo6118.cn

[Q45] EXISTS 判断存在
来源：https://eo.zhonguo5118.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://pv.zhonguo8118.cn

[Q46] NOT EXISTS 判断不存在
来源：https://lg.zhonguo4118.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：https://un.zhonguo7118.cn

[Q47] 与平均值比较
来源：https://zd.zhonguo8118.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：https://gl.zhonguo8118.cn

[Q48] CTE 公用表表达式
来源：https://gd.zhonguo1118.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：https://yp.zhonguo2118.cn

SELECT * FROM t WHERE c > 5;
来源：https://za.zhonguo8118.cn

[Q49] 更新单行
来源：https://pq.zhonguo7118.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：https://pn.zhonguo6118.cn

[Q50] 批量更新
来源：https://kt.zhonguo2118.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：https://mg.zhonguo4118.cn

[Q51] 用子查询更新
来源：https://pu.zhonguo3118.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：https://xv.zhonguo2118.cn

[Q52] 删除指定行
来源：https://lr.zhonguo5118.cn

DELETE FROM users WHERE id = 10;
来源：https://ag.zhonguo5118.cn

[Q53] 按条件删除
来源：https://im.zhonguo3118.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：https://kj.zhonguo1118.cn

[Q54] 清空表
来源：https://hh.zhonguo3118.cn

TRUNCATE TABLE logs;
来源：https://tu.zhonguo8118.cn

[Q55] 排名（并列占位）
来源：https://ng.zhonguo6118.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：https://wl.zhonguo6118.cn

[Q56] 密集排名（并列不占位）
来源：https://kq.zhonguo2118.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：https://nn.zhonguo2118.cn

[Q57] 行号
来源：https://bw.zhonguo5118.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：https://ot.zhonguo8118.cn

[Q58] 累计求和
来源：https://gp.zhonguo5118.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：https://pf.zhonguo2118.cn

[Q59] 分组内累计
来源：https://it.zhonguo2118.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：https://qz.zhonguo3118.cn

[Q60] 取上一行 / 下一行
来源：https://dx.zhonguo7118.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：https://qf.zhonguo3118.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：https://kb.zhonguo2118.cn

[Q61] 移动平均
来源：https://nk.zhonguo6118.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：https://vm.zhonguo7118.cn

[Q62] 分组占比
来源：https://nm.zhonguo8118.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：https://if.zhonguo3118.cn

[Q63] 开启事务
来源：https://hw.zhonguo8118.cn

START TRANSACTION;                -- 或 BEGIN
来源：https://ld.zhonguo6118.cn

[Q64] 提交事务
来源：https://vx.zhonguo3118.cn

COMMIT;
来源：https://mw.zhonguo1118.cn

[Q65] 回滚事务
来源：https://bt.zhonguo1118.cn

ROLLBACK;
来源：https://qt.zhonguo7118.cn

[Q66] 行锁查询
来源：https://jb.zhonguo3118.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：https://ym.zhonguo5118.cn

[Q67] 设置隔离级别
来源：https://rg.zhonguo6118.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：https://dr.zhonguo7118.cn

[Q68] 保存点
来源：https://cy.zhonguo1118.cn

SAVEPOINT sp1;
来源：https://ls.zhonguo7118.cn

ROLLBACK TO sp1;
来源：https://yr.zhonguo2118.cn

[Q69] 查看执行计划
来源：https://ak.zhonguo4118.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：https://vv.zhonguo6118.cn

[Q70] 更新统计信息
来源：https://dd.zhonguo3118.cn

ANALYZE TABLE users;
来源：https://ha.zhonguo5118.cn

[Q71] 查看建表语句
来源：https://em.zhonguo8118.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：https://zc.zhonguo6118.cn

[Q72] 查看索引
来源：https://in.zhonguo2118.cn

SHOW INDEX FROM users;
来源：https://sr.zhonguo3118.cn

[Q73] 查看表状态
来源：https://hg.zhonguo6118.cn

SHOW TABLE STATUS LIKE 'users';
来源：https://zx.zhonguo5118.cn

[Q74] 强制使用索引
来源：https://ro.zhonguo6118.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：https://ic.zhonguo3118.cn

[Q75] 日期格式化
来源：https://pt.zhonguo5118.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：https://md.zhonguo7118.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：https://el.zhonguo4118.cn

[Q76] 按天统计
来源：https://zq.zhonguo7118.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：https://ec.zhonguo2118.cn

[Q77] 时间加减
来源：https://uz.zhonguo7118.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：https://bm.zhonguo4118.cn

[Q78] 当前时间
来源：https://tp.zhonguo2118.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：https://ny.zhonguo6118.cn

[Q79] 字符串拼接
来源：https://ux.zhonguo7118.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：https://vq.zhonguo1118.cn

[Q80] 字符串截取
来源：https://zs.zhonguo2118.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：https://dd.zhonguo5118.cn

[Q81] 字符串替换
来源：https://vd.zhonguo3118.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：https://jt.zhonguo4118.cn

[Q82] 字符长度与字节长度
来源：https://qu.zhonguo2118.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：https://lz.zhonguo2118.cn

[Q83] 大小写转换
来源：https://iy.zhonguo7118.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：https://ss.zhonguo5118.cn

[Q84] 去除首尾空格
来源：https://jo.zhonguo8118.cn

SELECT TRIM(name) FROM users;
来源：https://xp.zhonguo5118.cn

[Q85] 数值取整
来源：https://tu.zhonguo6118.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：https://yg.zhonguo1118.cn

[Q86] 读取 JSON 字段
来源：https://hx.zhonguo6118.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：https://nf.zhonguo2118.cn

[Q87] JSON 字段做条件
来源：https://zh.zhonguo8118.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：https://ss.zhonguo1118.cn

[Q88] 行转列（条件聚合）
来源：https://ws.zhonguo1118.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：https://nj.zhonguo8118.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：https://pr.zhonguo8118.cn

[Q89] 判断表是否存在
来源：https://pw.zhonguo3118.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：https://yb.zhonguo5118.cn

[Q90] 生成序号列
来源：https://pf.zhonguo4118.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：https://og.zhonguo4118.cn

================================================================================
来源：https://al.zhonguo2118.cn

R. Bash 专题
来源：https://mm.zhonguo6118.cn

================================================================================
来源：https://pb.zhonguo2118.cn

[R01] shebang 与严格模式
来源：https://tq.zhonguo1118.cn

#!/usr/bin/env bash
来源：https://hi.zhonguo1118.cn

set -euo pipefail
来源：https://qr.zhonguo5118.cn

[R02] 变量赋值与使用
来源：https://rk.zhonguo2118.cn

name="Tom"; echo "$name"
来源：https://gv.zhonguo5118.cn

[R03] 只读变量
来源：https://mk.zhonguo2118.cn

readonly PI=3.14
来源：https://lt.zhonguo1118.cn

[R04] 位置参数
来源：https://zt.zhonguo5118.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：https://hx.zhonguo2118.cn

[R05] 参数默认值
来源：https://tp.zhonguo6118.cn

name="${1:-default}"
来源：https://kr.zhonguo7118.cn

[R06] 判断命令是否存在
来源：https://hg.zhonguo7118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://iy.zhonguo8118.cn

[R07] if 判断文件
来源：https://id.zhonguo5118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://aj.zhonguo3118.cn

[R08] 数值比较
来源：https://sl.zhonguo7118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://uw.zhonguo1118.cn

[R09] 字符串比较
来源：https://tv.zhonguo6118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://lv.zhonguo1118.cn

[R10] 正则匹配
来源：https://cr.zhonguo1118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://tc.zhonguo7118.cn

[R11] case 多分支
来源：https://rg.zhonguo1118.cn


<!-- 参考信息 -->