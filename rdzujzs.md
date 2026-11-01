代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gkbhyulmf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gbguwvwuv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gcdzliysi.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gjxdkidxy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gnzmietrf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gwcuxojfp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/gwievbkzx.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.vehdjk.com/Article/details/gdgxmudor.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.yfazqb.com/Article/details/ggnhkiqsu.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gydklgygj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gskgbiyma.sHtML

Go:   if x == nil {}
来源：http://baike.sjlbkw.cn/Article/details/gdrejppgr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.tarul.cn/Article/details/ggdqnvwil.sHtML

C#:   if (x is null) {}
来源：http://mobile.tarul.cn/Article/details/gdkutbudx.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/guboqmfzr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/garbeocya.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/gtptlflkj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gjjpulmxd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/glbuhqhre.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gatobvazb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gyzzcujwr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.tarul.cn/Article/details/gqleoqylt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gsdurmehz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gvtyqfcqu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gcdemsmiy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gpmjeeewd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.vehdjk.com/Article/details/gticumhao.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gpqqgzpre.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.epnwcf.com/Article/details/gsasyhpid.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/ghksupqjn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/gxybpqlpb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gnqznrota.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsxhrucfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gyrehifgh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxgdknry.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/guaufmaqc.sHtML

CREATE TABLE users (
来源：http://read.share.fktsv.cn/Article/details/gffbzoqxc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gmbbvrvco.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gljzhgnyp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.sjlbkw.cn/Article/details/ggfacusnp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.epnwcf.com/Article/details/ggxxpzaoy.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gjitocqpw.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fktsv.cn/Article/details/goewvusgy.sHtML

CREATE TABLE orders (
来源：http://m.share.fktsv.cn/Article/details/grcajlqhp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gumlrampk.sHtML

user_id INT NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gdbdsffco.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.bbcook.cn/Article/details/gtyrrgpam.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gceinemyp.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gruxdlejz.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/guclrqsqn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.bbcook.cn/Article/details/ggalnldgn.sHtML

[Q04] 修改列类型
来源：http://wap.tarul.cn/Article/details/gkbmccsej.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.yfazqb.com/Article/details/gaqloxzgr.sHtML

[Q05] 重命名列
来源：http://wap.vehdjk.com/Article/details/grbsuqyex.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/gjprwnhed.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/gzmfuuczn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.vehdjk.com/Article/details/guobbmwkw.sHtML

[Q07] 删除表
来源：http://www.m.share.tarul.cn/Article/details/ghjmoiegv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/goqsleneg.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gtlxafvtn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gloauwdyj.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gipxzbuvn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gmqlrzhrf.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gcdashzyj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gmkvozapy.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/gnaubahtg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gllbfwoxx.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/ggmlsomcm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/gngwztcsa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/gjljbltbs.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/gobutcfyj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/grfjkzsxb.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gtubylybi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/gcqbadofi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gxemvqqvz.sHtML

[Q15] 查询全部
来源：http://www.blog.sjlbkw.cn/Article/details/gotrazrkn.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gykvlwfjf.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gfkfmgiqr.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gdlimegbi.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/gawesdzot.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.tarul.cn/Article/details/gcbpuktid.sHtML

[Q18] 模糊匹配
来源：http://read.share.yfazqb.com/Article/details/gywiwriyf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gqfirrkyp.sHtML

[Q19] 范围查询
来源：http://baike.sjlbkw.cn/Article/details/ggezjmfjb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gmbrflhcz.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/geagjxpyi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/gfimxxlnz.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/goxezzxzx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/giccpclnd.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/gxlzxpapw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gfbcmurov.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gzevoerfu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/guwoqdpnf.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/gttjscejb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gxaiqfuzm.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/genippuqw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gzqbkjaga.sHtML

[Q26] 计数
来源：http://read.share.epnwcf.com/Article/details/glnzvvfhv.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gisqplyzh.sHtML

[Q27] 条件计数
来源：http://wap.sjlbkw.cn/Article/details/gwgifxywg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/goziekkzr.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/gjjknopcg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gencovgjk.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gxktdffqq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gftfynkdv.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/gpcuvzscc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyrxwfvs.sHtML

[Q31] 分组后过滤
来源：http://m.share.fktsv.cn/Article/details/gxzclxkxg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/gczghjjcd.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/ggimpbcio.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gfthqqdpm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.bbcook.cn/Article/details/gqkjgykyx.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gmtayxydc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gzmjmzfcx.sHtML

[Q34] 每组取第一条
来源：http://3g.bbcook.cn/Article/details/glnnvixmm.sHtML

SELECT * FROM (
来源：http://read.share.yfazqb.com/Article/details/gzrvetyby.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.tarul.cn/Article/details/gjsfjiiia.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/grgljltmw.sHtML

[Q35] 内连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpbofzme.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/geckwakoz.sHtML

[Q36] 左连接
来源：http://baike.sjlbkw.cn/Article/details/gqfjkbtnq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/giwrrwbkm.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/gomicgwtk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/gbfxdrifc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.epnwcf.com/Article/details/gsputtypi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.sjlbkw.cn/Article/details/guqgtqejl.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/gsjfqpwgi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gnjjizqyr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fktsv.cn/Article/details/guablpluh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.bbcook.cn/Article/details/gwgybkknb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.bbcook.cn/Article/details/gfgrgbnor.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/gdarrfbom.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.tarul.cn/Article/details/gprgjlgsc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/gzfsbtgmp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gqwsdyvid.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/gtoluuyhb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.yfazqb.com/Article/details/gzqkgzjwu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gdqxzexde.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gdpdfvoav.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gsbupeubn.sHtML

[Q44] IN 子查询
来源：http://www.share.sjlbkw.cn/Article/details/gysctwngb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gfxzivmeo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gaebspioo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gscmcijpe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fktsv.cn/Article/details/gqpaknhex.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gcxqhyscx.sHtML

[Q47] 与平均值比较
来源：http://3g.tarul.cn/Article/details/gqoxqqoas.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gplyxpouy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fktsv.cn/Article/details/gftxktspi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.tarul.cn/Article/details/gxlshdyrp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnxvfnqk.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/gmbexloya.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gzilsnhqo.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/glupnjxyu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gqwqhlqsv.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/guwbfwyev.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/gczqtzvjy.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/gvqvnowxd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gbpzgcrrn.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gvwlpqnqq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gvenqiyal.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/glfkzoesb.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/gbbttrmte.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gzyppdkud.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gdzzmcpil.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/gexhcoajd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.vehdjk.com/Article/details/gmgimgrmb.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/goscdycvb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gkutlrylz.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/ggqqsisqr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gaablzwpb.sHtML

[Q59] 分组内累计
来源：http://www.blog.yfazqb.com/Article/details/gprijgefx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gpbhpaoii.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gubnhgopu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/ghdklryoo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gpfhozgqh.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gafgjtvah.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/glmkzvooj.sHtML

[Q62] 分组占比
来源：http://3g.sjlbkw.cn/Article/details/ggsbxjynp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gosblgvpq.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/gukxzdopw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/gyprcwexh.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/gexritpua.sHtML

COMMIT;
来源：http://3g.yfazqb.com/Article/details/gzontofdd.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gohjchsae.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/ghfkkcrfl.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/gytmzknrd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fktsv.cn/Article/details/gcntdlawr.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/gozlhzdyb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.sjlbkw.cn/Article/details/gnzohtvmi.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gcsdpkizn.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/gatbgnjkc.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gbzxlbzyk.sHtML

[Q69] 查看执行计划
来源：http://baike.fktsv.cn/Article/details/gxliuipel.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.tarul.cn/Article/details/gaormastr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.bbcook.cn/Article/details/gllwtwbcn.sHtML

ANALYZE TABLE users;
来源：http://m.share.sjlbkw.cn/Article/details/gaiqxmqwa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/grbrhivbq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.bbcook.cn/Article/details/gprcfgbpi.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/gavhheuen.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gakagaahv.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/gorueldre.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.bbcook.cn/Article/details/gqzpvnbzc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gedesbxty.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gxoaxlzhl.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/geoctjbxl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/gostsymja.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/gmfufekpv.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/gbcofasap.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.vehdjk.com/Article/details/gvhwleais.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/gxnkqsphd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.vehdjk.com/Article/details/gwiwjgcqs.sHtML

[Q78] 当前时间
来源：http://read.share.fktsv.cn/Article/details/gqsqplsnl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.yfazqb.com/Article/details/geogssdns.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/ggjpwsoqz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/ginmmskaz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.epnwcf.com/Article/details/gzkngklfx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/grkodgnwv.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/giubotwro.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/glshxorfn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.bbcook.cn/Article/details/gvsxdyhod.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gpyyatpln.sHtML

[Q83] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gszpusphg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/glwyilxkk.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.vehdjk.com/Article/details/gukqvzwil.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ggmevfcix.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gxgloevxv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.vehdjk.com/Article/details/ghyodyplw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fktsv.cn/Article/details/gddjctjme.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gbgwvnhep.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gxtvjyjup.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/grdbfwuof.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.bbcook.cn/Article/details/gqfmqcasz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/gjwmnlffu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.epnwcf.com/Article/details/gltvtezaf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.yfazqb.com/Article/details/gjmqsowid.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.tarul.cn/Article/details/gtphljmfz.sHtML

[Q90] 生成序号列
来源：http://www.blog.tarul.cn/Article/details/gvcnzcgxt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gpzqehjuc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glinxbglu.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gvsurbnhm.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gklvokgck.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gaiijetah.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gmjbxzyqi.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gculgjqol.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/gvbcgcicd.sHtML

name="Tom"; echo "$name"
来源：http://blog.sjlbkw.cn/Article/details/ggdqbpswf.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gplwkzchb.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/galttyfdk.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/ghcidwczl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gbslqewtc.sHtML

[R05] 参数默认值
来源：http://blog.epnwcf.com/Article/details/gcvxbbcol.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/ggjtekimz.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gvmuupvoc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gkidasdjq.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gopwbbzov.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/gvziusopw.sHtML

[R08] 数值比较
来源：http://wap.tarul.cn/Article/details/gshjuhfwu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.bbcook.cn/Article/details/gkngprzjj.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gfuhlriyp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/ghoecsqua.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gescjdart.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/glzcjlbve.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/ggsnmnfme.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/gjswenxfr.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/ghaivfhvu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gfjnnehij.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gzfaklasc.sHtML

esac
来源：http://baike.fktsv.cn/Article/details/gvlkpgite.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/glfmbtfyh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gdugjgcgu.sHtML

[R13] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gahefmhfg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gmnzgfcyb.sHtML

[R14] C 风格 for
来源：http://read.share.sjlbkw.cn/Article/details/gajhobsxq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gkyezyinh.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gevgkbnyw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gcdloshiv.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gxzjdoifs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/grpzxcneg.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gvurzpbck.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/gqblnimvi.sHtML

[R18] 遍历数组
来源：http://blog.epnwcf.com/Article/details/grakkfmto.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gglfalvtb.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/grsbmgfib.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gqzhcwmms.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/gjfjmlpyh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.yfazqb.com/Article/details/gyvmtxpta.sHtML

[R21] 字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmmtcxvf.sHtML

echo "${#s}"
来源：http://www.m.share.fktsv.cn/Article/details/gsavugjwu.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gkbbgfdmh.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gtdetdmar.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gvrklfkaw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.yfazqb.com/Article/details/gdwndqvwu.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gtulgfchq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/gzrjfrrgy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gwfhvibpm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/gnpiqckhy.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gadiwxovx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gnyniykvi.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gmrqnanin.sHtML


<!-- 参考信息 -->