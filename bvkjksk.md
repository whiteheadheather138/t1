代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gbsurxhgb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/gkcrotsrt.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/gzaupsbaw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gttguwass.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gcqrbtxge.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/guydiaorv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gugeecwnt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/ghisiboun.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/gngvorpvm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.tarul.cn/Article/details/gsyahfydu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.sjlbkw.cn/Article/details/gnyvtvkvi.sHtML

[P04] 求长度
来源：http://blog.bbcook.cn/Article/details/ggfdukdak.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gfupngqdh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gmrcvkbjq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gplawhhre.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gtiftaquy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fktsv.cn/Article/details/giwlknsbl.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/gkibcqhao.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/grkqyrdot.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/ggltjudpd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/gjlrydrdl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gfqqyspie.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gtluhqcgc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/gsxlmcjhf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/ghxloyoii.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gfddxycrp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gwtymfsig.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gkanffuaq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.yfazqb.com/Article/details/gdtptfmxr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gowietgrz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/gqagdphju.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gxbpkveiy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gxwippcss.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/gptwyibms.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gxdhtaiei.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gzcjnbnbn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.tarul.cn/Article/details/gjvoakady.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnyrmbiw.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gugjdpzoz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/gyhgmndvf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gjahhhcht.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gyhcpndjs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gehrtprfk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gfzgujmho.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.vehdjk.com/Article/details/gijzgjbxq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gfkknrqqz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gnriqntyi.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fktsv.cn/Article/details/gxhfpefne.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.epnwcf.com/Article/details/gmictkbbp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gpzfckjlo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/ganiqyncx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gwhrvbsah.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/gzxvvzrbb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gvyfdneko.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gumgrllmp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gdrhbfxgw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdqsrcjbe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gcyktetxn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwzzrorym.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gkojbgwhd.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gjsuntjqm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/ghhiqzoft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gynioyxnd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fktsv.cn/Article/details/guajdzhcv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gdwmcwalk.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gwlvmjkak.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.tarul.cn/Article/details/gatagpgss.sHtML

CREATE TABLE orders (
来源：http://mobile.fktsv.cn/Article/details/gelaxsqau.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gsjkqmspe.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/grnytugfo.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gsfzdpfxr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gopasaraa.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gfzivuzdo.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gnmxuckgn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gvraxqwie.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/gpreiilxo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/gnqmqqwds.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gxisdydoc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gdjhhjhlt.sHtML

[Q06] 删除列
来源：http://m.share.tarul.cn/Article/details/gkzxwnbdi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gxzqirbee.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/ghktpijfx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/gwcukzpvc.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gdtvtlvoa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/ggqemkdwc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gmukneufp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gfebvylqn.sHtML

[Q10] 插入单行
来源：http://www.m.share.epnwcf.com/Article/details/gpcnooiwz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gnzbdotkm.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/gcdwcavmr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gpzfhpwcd.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fktsv.cn/Article/details/guqlluatv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gwybcpwrr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/gckoyduil.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gwxdzidco.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gcwyrruqk.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gxswqkrmv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/grbshoskw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.yfazqb.com/Article/details/geogkfxsi.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gcobwllop.sHtML

SELECT * FROM users;
来源：http://blog.tarul.cn/Article/details/gqoyuzjwv.sHtML

[Q16] 查询指定列
来源：http://www.blog.tarul.cn/Article/details/gijdbwnmq.sHtML

SELECT id, name FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gkhjtgubh.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gyzygxqsi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/gusuwxeog.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/gavhufiyy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gynzcrbzr.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/gvodbrgdh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gyouwowdq.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/ggytruolp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gggsympvj.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/ghfrbuwvz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/gfprbqxcf.sHtML

[Q22] 排序
来源：http://mobile.tarul.cn/Article/details/gtthybnds.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gpxptlgyy.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gmrdbnlbz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.sjlbkw.cn/Article/details/gcjhclera.sHtML

[Q24] 去重
来源：http://baike.sjlbkw.cn/Article/details/goflnyapt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gmjnvhvff.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gorerissn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gkifsxpvp.sHtML

[Q26] 计数
来源：http://mobile.fktsv.cn/Article/details/goftuaogy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gsktuxqrw.sHtML

[Q27] 条件计数
来源：http://baike.sjlbkw.cn/Article/details/gbehpxjgj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gduqsligt.sHtML

[Q28] 求和与平均
来源：http://blog.bbcook.cn/Article/details/glfcnxpno.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkisbbbcm.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/gsuppwlwe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gnzscimzd.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/ghkvdwybv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gjqwdvezl.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gxemcoavz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/gshbmabcg.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gklylqfru.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gwuozlgum.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/gkilnicyh.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/gkeahukyx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gksjfxrjk.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gkmfpqnvn.sHtML

SELECT * FROM (
来源：http://www.m.share.fktsv.cn/Article/details/gdfejijzs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/grrcmaedf.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/gpstspulh.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gykwyzftn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gibadktda.sHtML

[Q36] 左连接
来源：http://baike.epnwcf.com/Article/details/gycmhistc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gjqggktun.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gbaehaxjy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gcwwdwqqn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.bbcook.cn/Article/details/gedafbmdb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/gljoolmze.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.epnwcf.com/Article/details/gxfsoakqh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gpblhckdb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gfnoynmxc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/groknxacs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.yfazqb.com/Article/details/gbpqkfacc.sHtML

[Q41] 多表连接
来源：http://3g.sjlbkw.cn/Article/details/gojjkyayu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.yfazqb.com/Article/details/ghzfzxyqh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gvmuxmyvx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/gmcgkdcbn.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.vehdjk.com/Article/details/gmfrdkuhk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gqrxrxkmk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gldpuurge.sHtML

[Q43] 标量子查询
来源：http://www.share.fktsv.cn/Article/details/gacyhiihx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gghqceqdq.sHtML

[Q44] IN 子查询
来源：http://www.blog.fktsv.cn/Article/details/gdtporxwu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/giwwmzmql.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.bbcook.cn/Article/details/gjnyfltxx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/ggtyossxq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/goygqbeoi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gyvjwbtrs.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/guxklavsq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gidwtyrod.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gyoqnzamg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.yfazqb.com/Article/details/gosgqzawv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.vehdjk.com/Article/details/gsznehfyq.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/gqixlradw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gdlhycwvm.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/ghgyvzqci.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gixjhvkau.sHtML

[Q51] 用子查询更新
来源：http://blog.sjlbkw.cn/Article/details/gmqdechwu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.tarul.cn/Article/details/gwzcdnegj.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/gkkbrslgz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gqpiqglpl.sHtML

[Q53] 按条件删除
来源：http://3g.fktsv.cn/Article/details/gaoviwluk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/geyrspypu.sHtML

[Q54] 清空表
来源：http://www.blog.yfazqb.com/Article/details/gopcpxaay.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/glfslxdsf.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.tarul.cn/Article/details/gajugqpfg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/ggilexmge.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gbachtqzh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gfalkdgki.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gvibcmgfp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gpxotakqp.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/gcsggkcgn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gpyembsio.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/geaaytvwt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gjpzgqawq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.epnwcf.com/Article/details/grhshbupc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gvgrmujyx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gaalaygoy.sHtML

[Q61] 移动平均
来源：http://mobile.tarul.cn/Article/details/gawtqyjxm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gpqggqcmz.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gldzedjaa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/goektucgb.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/gazqxnlzs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.tarul.cn/Article/details/gbccxkukm.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/ghyyttigj.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/gnoebhwzt.sHtML

[Q65] 回滚事务
来源：http://3g.tarul.cn/Article/details/guxorlyfq.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gqddqfvhv.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gsfzdgmae.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gnqjznpzx.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gsjwvkoer.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/gqtcsodbg.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gfpgiotxa.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gcpduemap.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gbbjqgpoh.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gtiojewrg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.bbcook.cn/Article/details/gytnzibgp.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gqysaouho.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gzfjqebfw.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gynqabhot.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbeuuszx.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/gvhcfjwrb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/glwgdohmj.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gxkzkydgt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/grthmjrxm.sHtML

[Q74] 强制使用索引
来源：http://blog.vehdjk.com/Article/details/gzaarwson.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fktsv.cn/Article/details/gpbedyvis.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gwnkjaoaw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gghbrrgba.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/gyidlmcca.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gldwgvedx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/gcjxnzdkq.sHtML

[Q77] 时间加减
来源：http://www.share.bbcook.cn/Article/details/gcilqvzpn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/ggpqikcuz.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gcihqrrka.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.vehdjk.com/Article/details/glpahtcke.sHtML

[Q79] 字符串拼接
来源：http://mobile.tarul.cn/Article/details/gtnjqxfat.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gcuobzpij.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/grmbouawz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.epnwcf.com/Article/details/gnrgvarld.sHtML

[Q81] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gtgozuqag.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/geydkoilu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.tarul.cn/Article/details/ghsrqjosv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gwnpybavy.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gsqsqfedn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gotkekoat.sHtML

[Q84] 去除首尾空格
来源：http://3g.tarul.cn/Article/details/gwnjroicj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gwxvaclmh.sHtML

[Q85] 数值取整
来源：http://mobile.vehdjk.com/Article/details/gixehaszt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gpnsmhttz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gtpixbcwg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gxyxfzuml.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/gybgrgxyz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.epnwcf.com/Article/details/ggafjvojn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gsbsuxdvc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gisjhjyey.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gnxhtnqsr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fktsv.cn/Article/details/ghnanzwhx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gipluxxru.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/glvpsbtwm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/gliyqjtsd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwobzofyk.sHtML

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/gljhabyxi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gxxidauwo.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gjujgyiso.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/gwrntabfd.sHtML

set -euo pipefail
来源：http://www.m.share.tarul.cn/Article/details/gaqadvkof.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/gwuwjqbql.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gtlmojbxo.sHtML

[R03] 只读变量
来源：http://3g.fktsv.cn/Article/details/gnwziglzb.sHtML

readonly PI=3.14
来源：http://baike.vehdjk.com/Article/details/gphrejqyw.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gcsfxpxsy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/groaaqqtx.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/ganlkdjfm.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gmbyrovqo.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/ggjzkocfx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/goopgjqxm.sHtML

[R07] if 判断文件
来源：http://www.share.fktsv.cn/Article/details/gxncoyoxr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gzhzvxkmr.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gszjmmlpu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gbvbtzpbc.sHtML

[R09] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gljrhinrw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/ggxlquaof.sHtML

[R10] 正则匹配
来源：http://wap.fktsv.cn/Article/details/ggcvnkpuh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gfuqkzmax.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gsojjntxu.sHtML

case "$1" in
来源：http://wap.fktsv.cn/Article/details/gqjsczcdu.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gvngldxll.sHtML

stop)  echo "停止" ;;
来源：http://3g.fktsv.cn/Article/details/glquofnmp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gnadzufkn.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/gbdnxswrs.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gvgqthanp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gqigradmq.sHtML

[R13] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gimmvclnr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gwubjcelw.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gdpnwttbt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gntbvyjxv.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/ggubtpwwr.sHtML


<!-- 参考信息 -->