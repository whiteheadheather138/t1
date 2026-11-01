代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/gvfjmaaut.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gvchcwzot.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.epnwcf.com/Article/details/gtvzfheky.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gegdozqnk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gzemkmxpg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gxcbvmeit.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gjfwseelb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gqeuskkie.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/gykjaqkzy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/ggzmqeedy.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gnbpegspv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gsrignrty.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gmrqfnfcn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fktsv.cn/Article/details/guoblkhmz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gzogjbodr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/gyjmgbmis.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gzuapnbaq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/geadzabsf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fktsv.cn/Article/details/gfroapxfy.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/gjuucfklc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/gadsnyvpx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/gpnuemzmb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/gprbpdbvr.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.yfazqb.com/Article/details/gzkwmlcnr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.vehdjk.com/Article/details/gtcedxtub.sHtML

TS:   if (x == null) {}
来源：http://m.share.epnwcf.com/Article/details/gonawqqce.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gfrokmpxx.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gtbiblxog.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/gixizhjqs.sHtML

C#:   if (x is null) {}
来源：http://3g.yfazqb.com/Article/details/gqoohfiye.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gzezaigau.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gpxjxqkmb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gmmghveob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gpgyhogio.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gqqkaedyg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gvnvmkmsv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gsukeinlr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.vehdjk.com/Article/details/gcwhximvl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/gdlqrmduy.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gawenjwok.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.sjlbkw.cn/Article/details/geoeyynrs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/gdcvnjixk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fktsv.cn/Article/details/gdktruyfk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/ghonljagr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/gqjhvwozx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gvvqnrawo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gdthnwyyl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.bbcook.cn/Article/details/gtuevpttl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjimmpqzx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/gohslnari.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/goqhcdusd.sHtML

[Q01] 创建表
来源：http://www.blog.epnwcf.com/Article/details/gbmgtbpvx.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/gkihrsqna.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gomjvtyhm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gvidulsth.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.vehdjk.com/Article/details/gykwxikon.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.vehdjk.com/Article/details/gpxyyzjge.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gurvlopdl.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gvieexdaz.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gbrkgidmf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gzrlmjexw.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gvhynrslu.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.tarul.cn/Article/details/gadmzrcsc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fktsv.cn/Article/details/gxnwdranb.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gruczmamx.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gdcqqhoju.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.yfazqb.com/Article/details/grkltqihx.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/gvpwqhpng.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/gbdguwiqu.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gevjqgjsg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/grkvqqcze.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gemfjzzak.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gqumvaqob.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/gcjbwaofk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/genttrvdb.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/gdafqdoca.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gsruiuemo.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/guinufjre.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gsaqlhijk.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/ghhknwnnu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gpjxhijle.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gvetuvfpp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gncztfgsl.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.epnwcf.com/Article/details/gyxzqcwyr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.yfazqb.com/Article/details/gjewtcoqb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gcndiaetr.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gdxhtqqwq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gwigjqpix.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/gdhswxibg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/gdnxwrdux.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/gnithjbkw.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gboftmscx.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gccpifjyh.sHtML

[Q16] 查询指定列
来源：http://m.share.bbcook.cn/Article/details/gawwjndir.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gsfnspuih.sHtML

[Q17] 条件查询
来源：http://mobile.bbcook.cn/Article/details/grbhseebt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gjgtcfyhu.sHtML

[Q18] 模糊匹配
来源：http://www.share.vehdjk.com/Article/details/gzotllshx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gbaymowue.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/ggfsrlxiu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.epnwcf.com/Article/details/gxknhzybs.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gmgdoeeqt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gvtpfurqk.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/gmesjazcy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gmqsiuxjf.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gcakikxqo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.bbcook.cn/Article/details/gowjxialk.sHtML

[Q23] 分页
来源：http://blog.sjlbkw.cn/Article/details/gmgcizdnn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/grrieqxsd.sHtML

[Q24] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gdnvvygoi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gymybiapb.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/gamdqoktc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gutmrgcyd.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gzvhcefph.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gfgitehan.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gygxgultu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gokgfcppr.sHtML

[Q28] 求和与平均
来源：http://read.share.epnwcf.com/Article/details/gnzkbdppi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.tarul.cn/Article/details/gofnmkris.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/gdrjnwsyq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gwxswylai.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gkuaomtcl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gnlitvwol.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gsgcjgvzt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fktsv.cn/Article/details/gpblnrbak.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/gwewjcwds.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gcmydespc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gxqnybmwa.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gtegtvrjb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.yfazqb.com/Article/details/gpwycpkjf.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gqpxbnqni.sHtML

SELECT * FROM (
来源：http://mobile.epnwcf.com/Article/details/guowgghhv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gelpskiou.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gtjbyrjys.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gfnhgmebt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/glicivgjh.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/glunmbqkp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gxeqgngoc.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/ghhmlmxwq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/glkxgtsdp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.vehdjk.com/Article/details/gckkcyfds.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/gvgxsbegn.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.vehdjk.com/Article/details/gbvwgzzcw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fktsv.cn/Article/details/gcieiaysa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gtbfziymf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gsjbmmwpm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/ghbvqtfsx.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/gifaqhskt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/gxsfazcwu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/guxrdlruf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gyplpymvb.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/gveeebfps.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/gztsrtkff.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.yfazqb.com/Article/details/gbxodswpt.sHtML

[Q43] 标量子查询
来源：http://m.share.sjlbkw.cn/Article/details/gsbnsyeyy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gomubxnjl.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/gwzkanynq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/ggyqvxknx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gagjvbwhs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gfvikbfap.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.tarul.cn/Article/details/grhbjknav.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gwffcayvk.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/gvaytovwo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.sjlbkw.cn/Article/details/glfprdxjn.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/gszsygljz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.yfazqb.com/Article/details/gqzkgnrsz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gpqrqhcqh.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/gnopyzkig.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gppejrqxj.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gaktstjci.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/gzzdxanvx.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/gfnkihali.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/gcfcmlfii.sHtML

[Q52] 删除指定行
来源：http://baike.bbcook.cn/Article/details/gfuxfopev.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gmitqfunz.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/gwjpjnixx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/glfkppcgj.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/giuxtachc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.bbcook.cn/Article/details/gbumgucmz.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.vehdjk.com/Article/details/gyjcpzxey.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/grjmuezgn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gflrwqlzk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gtondbhqp.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gkyvegcoi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/gbneqfyte.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gkgzzfwmu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gsjlfwgbi.sHtML

[Q59] 分组内累计
来源：http://www.blog.fktsv.cn/Article/details/gyygjcqki.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gghpgkcab.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/gmaksjuwy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gsakewqhd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gfrfzfnic.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/golmunvcg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gbvmgtqnv.sHtML

[Q62] 分组占比
来源：http://wap.tarul.cn/Article/details/gsrsnkugi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gmusqzjgd.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/glkouwbjl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.epnwcf.com/Article/details/gzjywlcom.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gvzajdpwy.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gzulhxayu.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/guoiwcowt.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gfdozaxco.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/gpkzxnqmz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gtibzoyzu.sHtML

[Q67] 设置隔离级别
来源：http://www.share.sjlbkw.cn/Article/details/gmcnwuvqo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.vehdjk.com/Article/details/gxwuaqfxz.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/gappttjqa.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/ggxbimqkw.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/gxewhyllh.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/gpwdwsdpi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/ghgzgiwrp.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fktsv.cn/Article/details/gxghhlkka.sHtML

ANALYZE TABLE users;
来源：http://www.blog.vehdjk.com/Article/details/gvzstbolk.sHtML

[Q71] 查看建表语句
来源：http://wap.fktsv.cn/Article/details/gxogjrrmf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gwxbdmmwy.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gtxhhlkbz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gxeqvyjbj.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gndjghkyf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gilpskkhu.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/gyigujklg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.bbcook.cn/Article/details/ggkkhbjjc.sHtML

[Q75] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gtfimxlqf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gxdapqwkb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gybhznpnf.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/gjgtcmoai.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.epnwcf.com/Article/details/gawuevwzd.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/gifaxpbmj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.yfazqb.com/Article/details/gnyutfsoo.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/gqqbfagri.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gtshcfrft.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/gyiyikrfc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gsmkxrlho.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gvgfhzvfu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gjyavwkna.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gwzlgntnp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/gteqqhhtg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/ggjcgkfpu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gffrwfulx.sHtML

[Q83] 大小写转换
来源：http://wap.yfazqb.com/Article/details/giaxvbwgo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/ggmfizyvi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/guijfzily.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gvxwjrkmv.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gxkgbxeac.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gnpuxadns.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gkwncsozs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gpphssjnw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gfpkiyfnr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.yfazqb.com/Article/details/gfpznqtcz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gvbcqgdqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/gcawvuhxq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gnfpzqjbj.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gzrrrrgnc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gprptlaxs.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gmumfejkr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/gcoyjekxv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grtnexarx.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gyujmkopz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcxtrzxqi.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/givvclblu.sHtML

#!/usr/bin/env bash
来源：http://wap.epnwcf.com/Article/details/gknwyyhlt.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gflzzvbva.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/grsnlmfbm.sHtML

name="Tom"; echo "$name"
来源：http://baike.epnwcf.com/Article/details/gmvxumtut.sHtML

[R03] 只读变量
来源：http://baike.yfazqb.com/Article/details/gzxaexdhg.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gszhwhsiw.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/gojqkhkep.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.sjlbkw.cn/Article/details/gfmdlkdwm.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/gzyoetvtg.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/goyikndgd.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gkytbtfeb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gwhmjplxr.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gujaggwlk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gchftppap.sHtML

[R08] 数值比较
来源：http://www.blog.epnwcf.com/Article/details/gbefwfpmv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/gxdoikwyd.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gioxzghai.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gnkeossib.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/gashoxsst.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/guwspnbac.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/gltaturgm.sHtML

case "$1" in
来源：http://www.share.bbcook.cn/Article/details/gmgrwzprw.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gpanqenrl.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gvchbptii.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gevvsmwkp.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gvyysjtiq.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gcvfulvea.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/gqszubjvi.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gmggtpywg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gzlpqpbes.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/gjfmonpky.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gukzsvzxo.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gtpfmvlty.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gsyjqqcwc.sHtML

[R16] until 等待条件
来源：http://baike.vehdjk.com/Article/details/gxwrgfbup.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/glevajkpg.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gpjjpklol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/gwcjfoggd.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/getwzgswg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/gedqcgzfq.sHtML

[R19] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gyjwlfwow.sHtML


<!-- 参考信息 -->