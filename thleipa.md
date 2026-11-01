代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gtlxxpsoh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gsjkgdijc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gkccfrjdq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gfpenqoaf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gdxwzhujw.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.sjlbkw.cn/Article/details/gjmceiwrh.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/gujqcvdsk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gqqgfzriu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gezlizoyj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/grgkphqjd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/gdsuzpphz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.tarul.cn/Article/details/gqlrcpnfq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gbrgfpwqx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fktsv.cn/Article/details/gbrshuhjj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gluumtoxj.sHtML

Ruby: a == b
来源：http://wap.yfazqb.com/Article/details/gmckchqsh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/gjpumpgnk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/gofzklitl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.yfazqb.com/Article/details/glogaajow.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/gicicpkiq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/guccjneko.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/grdbnlkci.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/ghehoxeoj.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gzqstykac.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gjwrbvrnz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gomuzlcjm.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gcwdqikbx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/ggxpromnt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gvffiyapf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gwwfwmmyz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/ggsublurk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/gmayliaqp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.epnwcf.com/Article/details/gjstwzjkd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gardluyij.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.tarul.cn/Article/details/gyckchmqx.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.sjlbkw.cn/Article/details/gnhyfsugu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gcmsticri.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gtybjeepl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gdnqghqoj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gcdjphhor.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gwufxbczx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/gkqdmygyq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/gluxqftcu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gymdsceho.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwqwrfrbl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gnctshrdd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/guuxqrifu.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gjymachvr.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gosqydajm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gtajtgswz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.tarul.cn/Article/details/gpyvnuitc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.yfazqb.com/Article/details/gnhuxjnos.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzowwxfi.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gygjaxxod.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/guoypebuu.sHtML

CREATE TABLE orders (
来源：http://www.m.share.bbcook.cn/Article/details/ghpwzvind.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gkoqghnlq.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/ggmpnacor.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/giygqxyin.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/gpfxnybzi.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gufewymls.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/ghjdposnj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.vehdjk.com/Article/details/ghhxdocev.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/gvwfalkow.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/gaszeylzd.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gyzcuwkfc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/ghbzkuozv.sHtML

[Q06] 删除列
来源：http://www.share.bbcook.cn/Article/details/gphndqqop.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gunsntnte.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/genutnghg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/grxulofuk.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gqxogdwse.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gllpszlhe.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/geoieljua.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gpbhrywfn.sHtML

[Q10] 插入单行
来源：http://www.share.sjlbkw.cn/Article/details/gaqfsdfmu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gvsxgmjnq.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gzsbipaqm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gqmbtvfvu.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fktsv.cn/Article/details/gwmfdolqc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/gjzshmdon.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/gicyjtbkf.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/ggktjraps.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gmmcpussf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/gpxlqcova.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/gmjjalbqz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/gpbcbjybe.sHtML

[Q15] 查询全部
来源：http://wap.bbcook.cn/Article/details/gsswhreti.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gwozuyuci.sHtML

[Q16] 查询指定列
来源：http://wap.fktsv.cn/Article/details/gprzxfwbz.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkalvfemz.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/ggrpndzve.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.bbcook.cn/Article/details/ghbceobll.sHtML

[Q18] 模糊匹配
来源：http://www.blog.tarul.cn/Article/details/ginamgrbg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/gpaykmgko.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/ggqibodhs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.tarul.cn/Article/details/gzedmnkme.sHtML

[Q20] IN 列表
来源：http://read.share.epnwcf.com/Article/details/gsdtuggpq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.tarul.cn/Article/details/gagwdefwp.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/gpsdgimvt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/gkmttemla.sHtML

[Q22] 排序
来源：http://3g.epnwcf.com/Article/details/gqjguntvd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gukxxvurt.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/gidojwaxl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gbxlifzcz.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/gczrqiumw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gzeevphzh.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/ghwbiymag.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/gsqnfgare.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gijjqsktj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gurowqnpz.sHtML

[Q27] 条件计数
来源：http://wap.yfazqb.com/Article/details/gzaxaeavt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.bbcook.cn/Article/details/ggndbkatm.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gfkyofbte.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gtqxripdu.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gtfxngbhf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/goduogcuv.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gudmvmdqp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gwvsvppbd.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.yfazqb.com/Article/details/gnszvdpkj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fktsv.cn/Article/details/gujztccve.sHtML

[Q32] 分组拼接字符串
来源：http://3g.tarul.cn/Article/details/ghtyjlcog.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gdjaywmav.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gzrzaudox.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gizwdoebt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.vehdjk.com/Article/details/glrnwfgyh.sHtML

[Q34] 每组取第一条
来源：http://mobile.tarul.cn/Article/details/garrusjlv.sHtML

SELECT * FROM (
来源：http://www.share.epnwcf.com/Article/details/gtvmzsqbr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.bbcook.cn/Article/details/gtabuglxv.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/godveuraw.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/gbpzawyol.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gfayjwyze.sHtML

[Q36] 左连接
来源：http://mobile.yfazqb.com/Article/details/givktpmgz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gxkblsmvb.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/glythaqwl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/gaikxnpdo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gehrbmcso.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/ghvyszcoh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/gigqkormn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/gszzmdood.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/guwoqnmqq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/gdubnjfiu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gsmyafkai.sHtML

[Q41] 多表连接
来源：http://read.share.sjlbkw.cn/Article/details/gbvypvsxc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gamyobxbw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.vehdjk.com/Article/details/gfvsywwrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/giimogarf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.bbcook.cn/Article/details/gocnavart.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gtwojqbpy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.yfazqb.com/Article/details/gfyuccnil.sHtML

[Q43] 标量子查询
来源：http://blog.tarul.cn/Article/details/gimghtozi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.tarul.cn/Article/details/gequosbmx.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/ghhvivnxz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/gktyjarwn.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/ghmkfjhbq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gagpindbd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/gcpxtalgl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gpiosqkgv.sHtML

[Q47] 与平均值比较
来源：http://mobile.vehdjk.com/Article/details/gezlxxeko.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcijdwego.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.epnwcf.com/Article/details/gptehvnpr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.yfazqb.com/Article/details/gwijccvbo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/gaqsxfota.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/gqtmjvcuf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/ghmeanlvy.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/girlnemcb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/ggbmvabwd.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gjqxkoelt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gvnykmbgp.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/gmugdvaul.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gowrzzevx.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gbryagtoc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/giowccvdr.sHtML

[Q54] 清空表
来源：http://mobile.sjlbkw.cn/Article/details/gvmqoljcr.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.epnwcf.com/Article/details/grrbffokg.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fktsv.cn/Article/details/gggechsio.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gbkewfkjw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gojrjnibs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gdrjjwapj.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gngphzghb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gltzonphw.sHtML

[Q58] 累计求和
来源：http://blog.tarul.cn/Article/details/gagpynnpr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gruwsfkcq.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gxmiwuuue.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gyqzhdojn.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/gjxrozwru.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gajrqlyjq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gjxvbcnis.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/ghmfszhdd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gzvnbcsix.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/gzqodljhh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/goltcowey.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/gljtpczhm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/gwtlibilg.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/gleztdzge.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gikfehrwn.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/getnfcxmf.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/goebpbaig.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gnwekwdxf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/giznlbnwq.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/gfyardskz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/gabbxrmfz.sHtML

[Q68] 保存点
来源：http://read.share.bbcook.cn/Article/details/gasgsyzvz.sHtML

SAVEPOINT sp1;
来源：http://www.share.tarul.cn/Article/details/gndocstso.sHtML

ROLLBACK TO sp1;
来源：http://3g.tarul.cn/Article/details/gcszghdbp.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gkzveedbd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/gzdednddc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gktgezmrv.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gsbjmmtki.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/getipswph.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.bbcook.cn/Article/details/gdcsfowee.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/gijfvjhyg.sHtML

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/gybzmdmur.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gtoqyjyea.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gjbbaxebw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gdieoptdy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/gqfkiqttq.sHtML

[Q75] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gcevblcvl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/giahxqmbw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.epnwcf.com/Article/details/gsmxlokng.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gmwmmcjll.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gxirefaqk.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/gtfbbzulx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gqewomebz.sHtML

[Q78] 当前时间
来源：http://3g.yfazqb.com/Article/details/gwsskahxj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/gxytjfehw.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gpioyafxu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/gqrgsayjj.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gmoxpqgqk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqcxfanzl.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gkbnhfqet.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gwmxzemjd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/grlhhwvrc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gtaicsabz.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gmsipafbu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gwnivkkkh.sHtML

[Q84] 去除首尾空格
来源：http://wap.yfazqb.com/Article/details/gqrcudojq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gvkoxhhwu.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gjowqyzle.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gdnwnbhne.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.vehdjk.com/Article/details/gedctwpey.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.sjlbkw.cn/Article/details/gjhlfkqel.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/grcvcuvng.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/gqclwbimf.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gkuuudaja.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/grldoyuih.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.yfazqb.com/Article/details/gsbmjcbbe.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/gknkrpoxd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/ggqefxhfi.sHtML

[Q90] 生成序号列
来源：http://m.share.epnwcf.com/Article/details/gbpjxjaor.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/giunezoqc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gynuzvnbb.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/gaqeztgqp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvmlcaiey.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/ggjonnbhp.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gpazxxejl.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gdtwiltdx.sHtML

[R02] 变量赋值与使用
来源：http://3g.tarul.cn/Article/details/gvwukopye.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.yfazqb.com/Article/details/gfojezqej.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gtvegjlyk.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/gcyfosket.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gjjdkjsli.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.tarul.cn/Article/details/gcuqnrsxu.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/grkqigqwz.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/gddmodzij.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/garhwlnyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/goblkwqoe.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gjuzjzmnr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/gwhmnhneg.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gzmayfoep.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gvnsudfaw.sHtML

[R09] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gqzmdapdi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gfufxtzwf.sHtML

[R10] 正则匹配
来源：http://www.share.sjlbkw.cn/Article/details/glzwjwfpl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.yfazqb.com/Article/details/gqrewtlgk.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/ggpqiaryc.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/grebhbdqr.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/gppqeafdd.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gbpsawqrl.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gfriwhanu.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gawgjpgtj.sHtML

[R12] for 遍历文件
来源：http://www.blog.vehdjk.com/Article/details/gwnpihjpo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/gnilgmdvb.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gktaltemq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gokgxquhv.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/gihbprefx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gvwbeivxg.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gmcgzlfbq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.sjlbkw.cn/Article/details/gicvopnvx.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gombsukvz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gojkictro.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/gqbeapdjp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/geduqsmyc.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gnvhywilx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gqpamvopl.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gieedxvgl.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gltorbows.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gihooradi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gfrtdeypg.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/geytijyho.sHtML


<!-- 参考信息 -->