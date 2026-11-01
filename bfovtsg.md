代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/goqkkjeyr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gsiszeqhw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gotgbtxyj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gtiyawitv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.yfazqb.com/Article/details/gvjkxlkru.sHtML

TS:   if (x == null) {}
来源：http://blog.yfazqb.com/Article/details/ggpavgocl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/guqjjhfdp.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gdmosgydl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/griwuokbx.sHtML

C#:   if (x is null) {}
来源：http://baike.epnwcf.com/Article/details/gygmjtvse.sHtML

[P07] 防抖与节流
来源：http://mobile.sjlbkw.cn/Article/details/garcbrpos.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.tarul.cn/Article/details/gprtluhhu.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/goxztmnmo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gpuzlmloa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/getmqiirh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gioqagaic.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/ggqnoexqi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.bbcook.cn/Article/details/gebptoiyu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/gakopngob.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/ghsmwomrt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/ggglgjovs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gpgrtlfxf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gdrywjfeh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/grhsxorgp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.bbcook.cn/Article/details/gbaanlxnh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gdwsrboek.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.bbcook.cn/Article/details/gxrolxzpz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.yfazqb.com/Article/details/gabczcolb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfnjxbuhe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/gybamygvm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grlvgtmxj.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gkpzddkcw.sHtML

CREATE TABLE users (
来源：http://read.share.fktsv.cn/Article/details/godylwldd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gkbhgeter.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/grlozgagv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gsoslvzur.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gmibuujvg.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gfwmcfhhy.sHtML

[Q02] 创建带外键的表
来源：http://blog.epnwcf.com/Article/details/gffbxhnjk.sHtML

CREATE TABLE orders (
来源：http://mobile.vehdjk.com/Article/details/gpvdpnduf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/grymhyrfm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gncnvdvdm.sHtML

amount DECIMAL(10, 2),
来源：http://wap.sjlbkw.cn/Article/details/gfuzlwywu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gmtvdllpg.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gbgnqduvl.sHtML

[Q03] 增加列
来源：http://wap.vehdjk.com/Article/details/gletkwxpy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.sjlbkw.cn/Article/details/gicilsots.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gihmeypyf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/ghhyguiig.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/ggmmpfgqs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/glgkplird.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gjbdgvonu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.bbcook.cn/Article/details/gxiaaxgpk.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/gcyuungyy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gjaddvkkh.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gmnkrgvzo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gujjjcryp.sHtML

[Q09] 创建唯一索引
来源：http://3g.bbcook.cn/Article/details/gbjrzykgr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gvnxjltwj.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gjhpdhxrs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gufxacfib.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/gozndmeof.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gixcqmxvd.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.epnwcf.com/Article/details/gqljhuubv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/gddlhigyy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/giaigzrbl.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gspuqyhjz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/gsahigxxx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/gbnpzldvv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gpzpdcyyr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gukofessu.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/ggrawrplo.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gulvjzore.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/grjmhpkjt.sHtML

SELECT id, name FROM users;
来源：http://3g.vehdjk.com/Article/details/gqjsrrhax.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/gulawcdtb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gswnooxse.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/gnenbxbyr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gnumpybng.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gtvmqarut.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/gmratembw.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/glhcjggyp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.epnwcf.com/Article/details/ggnianzqf.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/glnrbdxtd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gdhwuqlwd.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gpdqmazoy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.tarul.cn/Article/details/gkikoqwet.sHtML

[Q23] 分页
来源：http://www.share.epnwcf.com/Article/details/gbxciwplk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/guqotrefb.sHtML

[Q24] 去重
来源：http://wap.epnwcf.com/Article/details/gcthsfkdf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/guhlqsvho.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gnfpiikyd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.vehdjk.com/Article/details/gmentmiyz.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gnymlmraf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/geufwtcde.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gkftzdszv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/gmuwfqkhm.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/gcwsbtumu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gimmtohgd.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/gulomauqo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gpdzjzqnt.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/ghoqheeyi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gurpjrhsq.sHtML

[Q31] 分组后过滤
来源：http://mobile.tarul.cn/Article/details/gnvqephag.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fktsv.cn/Article/details/gnerypkqh.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gypukwttu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gpocfniqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/gxdixttqr.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gcjnxvfjk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/glfqloqwa.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gzwcbyzts.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gsvuqcwhq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/glcexwmov.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gjpsyhfpw.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gbgrjhaoi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gohmmhcfm.sHtML

[Q36] 左连接
来源：http://mobile.epnwcf.com/Article/details/gczcaqopb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gfxwtridh.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/gvkwtsidy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/ghkyyhpae.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/gwshgypsl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/gwraqmhds.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gcafashsx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/gawiqowgo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/gcfeygfch.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gflgxdnir.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gfyibcvko.sHtML

[Q41] 多表连接
来源：http://baike.vehdjk.com/Article/details/gttdhjaip.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/genkyefua.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gmuhdithb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.epnwcf.com/Article/details/ggrbrnnpx.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.epnwcf.com/Article/details/giazdhndi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gxhygcmcw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gpxehldms.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/glevcraon.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.bbcook.cn/Article/details/giyzyuyvy.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gptorwurk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/gbnwmgsys.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gynphchmh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gnpoavnxw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.sjlbkw.cn/Article/details/gcvqfuzjh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/giatxuzaq.sHtML

[Q47] 与平均值比较
来源：http://mobile.sjlbkw.cn/Article/details/ggpzzqwxk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/gwfzfmklr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.epnwcf.com/Article/details/ggcagjexs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/ggndwivuw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/gifhyetgp.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/ggmlzmzhx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/glayfcnyj.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gctsbefch.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/gajddcjuk.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gyauqwrep.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fktsv.cn/Article/details/gdxettqak.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/gnzafdutb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gxwaxvjxq.sHtML

[Q53] 按条件删除
来源：http://m.share.vehdjk.com/Article/details/gomortkeo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.yfazqb.com/Article/details/gbelfedzl.sHtML

[Q54] 清空表
来源：http://www.share.sjlbkw.cn/Article/details/glmatllqu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.vehdjk.com/Article/details/gemguszox.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/ghlrpcypy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.tarul.cn/Article/details/gwdhmhswb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.bbcook.cn/Article/details/gyidzymmf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gnfgblgxd.sHtML

[Q57] 行号
来源：http://m.share.sjlbkw.cn/Article/details/gaungnpqd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/ghazfsuvu.sHtML

[Q58] 累计求和
来源：http://mobile.tarul.cn/Article/details/ghcqtqcgi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.yfazqb.com/Article/details/gqtudjtbp.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/gydhjwrtp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gcvmwqous.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/guegbswrx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.tarul.cn/Article/details/gyzwfgnpm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/giozdmswg.sHtML

[Q61] 移动平均
来源：http://www.m.share.yfazqb.com/Article/details/gnbrqkigu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gurgxfkwy.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gxresqrvh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gaxwrkumv.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gausdvuob.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/gzlokwifc.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gowmjzirw.sHtML

COMMIT;
来源：http://wap.fktsv.cn/Article/details/gzxkqtncg.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/guwieghxr.sHtML

ROLLBACK;
来源：http://mobile.sjlbkw.cn/Article/details/gdrnrlheg.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/gijyhqfag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/gngfrbnhp.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gcmqbnanl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gndzvgbwh.sHtML

[Q68] 保存点
来源：http://wap.bbcook.cn/Article/details/gykohgeda.sHtML

SAVEPOINT sp1;
来源：http://baike.vehdjk.com/Article/details/grpznqnkd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gpdorsvhk.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gaxhphsbs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gkcvblted.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwuvmlvg.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/gkdmgdccb.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfkksmvg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.bbcook.cn/Article/details/gbjoueesj.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gnprufwff.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gpjochqig.sHtML

[Q73] 查看表状态
来源：http://blog.tarul.cn/Article/details/gmfipgbwb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gcolryqte.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gjzggnffq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gumutuzdz.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gxjzorzav.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/gbosaymyk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/ghysimiqw.sHtML

[Q76] 按天统计
来源：http://m.share.epnwcf.com/Article/details/gpkyhyykk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.bbcook.cn/Article/details/gnhobavlc.sHtML

[Q77] 时间加减
来源：http://www.blog.bbcook.cn/Article/details/gruhyitel.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gfihjmmwr.sHtML

[Q78] 当前时间
来源：http://www.share.bbcook.cn/Article/details/gbunlbiux.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/glhpxrxwq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/ggtevrnsz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/goleelqsy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gmefweadc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gtwyvgklj.sHtML

[Q81] 字符串替换
来源：http://www.share.tarul.cn/Article/details/gprhpfzwn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/glieczgnz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/gltwmoxne.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gvkuldjsh.sHtML

[Q83] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gjqnvdutb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gezmeklsb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/geaidaiqp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gddsylapt.sHtML

[Q85] 数值取整
来源：http://www.m.share.tarul.cn/Article/details/golwzyikq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/ggtnypbtx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/gqzpqaffk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.sjlbkw.cn/Article/details/gkchthmbm.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/gfdjariuq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/gggpoxgix.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/geisfxmjj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gyszvdkwm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.bbcook.cn/Article/details/gktbmvudr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gvelzrlbp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gfomlfjyi.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/ghymvgytc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/gbrscovmz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grjhuykom.sHtML

R. Bash 专题
来源：http://www.m.share.vehdjk.com/Article/details/geylqggzu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqsdlklnd.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gaktvwbwm.sHtML

#!/usr/bin/env bash
来源：http://baike.tarul.cn/Article/details/grqcngmci.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/ggoaddwls.sHtML

[R02] 变量赋值与使用
来源：http://read.share.epnwcf.com/Article/details/germixqap.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/ghdhvdfbt.sHtML

[R03] 只读变量
来源：http://m.share.tarul.cn/Article/details/geydafkxf.sHtML

readonly PI=3.14
来源：http://m.share.tarul.cn/Article/details/gidnrxhcs.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gcbkrioor.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gexxnzqvd.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gqnnkpqcb.sHtML

name="${1:-default}"
来源：http://www.m.share.vehdjk.com/Article/details/gzybchiok.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/glfutvilb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gncrxzfmy.sHtML

[R07] if 判断文件
来源：http://3g.epnwcf.com/Article/details/gzvuiqqfv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gpabvzwjp.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/gsiepocix.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.yfazqb.com/Article/details/guywztqyw.sHtML

[R09] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/gbkixxyzb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gkefbuzun.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/gsyqjmcdv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gcesxejoh.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gghevzcdl.sHtML

case "$1" in
来源：http://wap.tarul.cn/Article/details/gcpihkuqi.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/gjzfkooxp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.bbcook.cn/Article/details/gjtddhari.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gmqmdsdtu.sHtML

esac
来源：http://baike.fktsv.cn/Article/details/gyymedxdz.sHtML

[R12] for 遍历文件
来源：http://www.share.vehdjk.com/Article/details/gzknrbmqg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/ghkttnpmm.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gxdasvxlp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gxgmqrszv.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gmqhimurj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gmdqroavj.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gjfjtkykd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/grmpipnam.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/gcmcxhmyu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gqsnelyif.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/grtnljbbo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.vehdjk.com/Article/details/guieghaok.sHtML

[R18] 遍历数组
来源：http://wap.tarul.cn/Article/details/gzdnmdfsy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.vehdjk.com/Article/details/gzjlcaxdr.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gkswdudzp.sHtML

echo "${#arr[@]}"
来源：http://3g.tarul.cn/Article/details/gduntafad.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/glnmkmtdi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/grevvvznn.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gbyttbqzy.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/grdhmcsrf.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/grywstdnl.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gsgetcadn.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gsmlrfius.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/gkgkexrnf.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/grmcekacn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.epnwcf.com/Article/details/ghlhnkyph.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gkmnjkher.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/ghpsfjyyq.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/grjjsxkdo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gbsgktuwe.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gflwmdjag.sHtML

echo $((1 + 2 * 3))
来源：http://blog.tarul.cn/Article/details/gzxuvybyw.sHtML

[R28] 浮点运算
来源：http://mobile.sjlbkw.cn/Article/details/gpbjuqyrf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/ghjwwuqbu.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gejbhnbzq.sHtML


<!-- 参考信息 -->