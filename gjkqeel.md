代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gmnwvmzaa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gxjzkbovc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/goooqmygk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.tarul.cn/Article/details/gmbuijbxz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gagxfrona.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gypzkgldl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/grkpdladh.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gccubnhpl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.yfazqb.com/Article/details/gvnqwtpdu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/gorvgqqep.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fktsv.cn/Article/details/gumxfmqkl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmdaumsgo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gutznrelr.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gnyfmydom.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gzygkusyo.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/grnxnvyog.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gxfykpiia.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/gzjuetuub.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/ghhdubuzb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/gcvpphwlx.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/gykuifrkg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/grhllayjv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gncmtbhfn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.yfazqb.com/Article/details/gpceprijy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gnjbondtj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gsifskfwb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gpjtydvyd.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/gvhouydsu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.epnwcf.com/Article/details/gteymkosn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gfpejzvbu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fktsv.cn/Article/details/gudxcyexd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gybpmdtzf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.vehdjk.com/Article/details/grphcaxue.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gammofjcq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gnzesyhbn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gzjkjadev.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqevlkhxl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/gfoguedow.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkarzpbdu.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gglyqemmh.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gxpodvwrd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gnbptfrad.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gokhahnco.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/ghssxgupy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gqjizyouo.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gxcvhuaza.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gtekgscyg.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gwsnqvlmx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gzvestfdp.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gcrnkqdbc.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/gxlnxcrlu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gayldjpwh.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpcimecx.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/gpzcizmud.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gefaqjmvy.sHtML

[Q04] 修改列类型
来源：http://mobile.fktsv.cn/Article/details/gkjvfzpqv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.bbcook.cn/Article/details/gxohdhxya.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/gzfirqjsk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gjtpwdajo.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gilypoxgy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gzsjytvdm.sHtML

[Q07] 删除表
来源：http://mobile.epnwcf.com/Article/details/gvvvsrird.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/gcrvqgdsr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/gcbaynhxi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gljgjgolc.sHtML

[Q09] 创建唯一索引
来源：http://baike.vehdjk.com/Article/details/gteejaajn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gpagfrfxu.sHtML

[Q10] 插入单行
来源：http://www.share.vehdjk.com/Article/details/geuibctln.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gqphcezse.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/gzfedlwio.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/glhsjtcwm.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gseoqoeqc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gjahvdrzg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gturfboei.sHtML

[Q13] 忽略重复插入
来源：http://baike.vehdjk.com/Article/details/gnrskkgoa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gtilehqih.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fktsv.cn/Article/details/gcrjplsnl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.sjlbkw.cn/Article/details/gaoxawisn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.yfazqb.com/Article/details/gmwzakpfb.sHtML

[Q15] 查询全部
来源：http://wap.epnwcf.com/Article/details/gjhkxatsp.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/guuvvpoti.sHtML

[Q16] 查询指定列
来源：http://wap.fktsv.cn/Article/details/grqgagqkv.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/gzdlsofni.sHtML

[Q17] 条件查询
来源：http://blog.epnwcf.com/Article/details/gxjjcxzsd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/glqfiltzi.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/gmabyfgob.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gjubfjwyr.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gzaycbzvm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.epnwcf.com/Article/details/gmkptfkhf.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gqhanfhym.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/gfwlcngpf.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gyabneoxl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gjesmgrup.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/gljigmvcb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.bbcook.cn/Article/details/gzxapuxry.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gitytuwnd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gzdovjsms.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/gaijblgty.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/ggzyjhgre.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gfkwjkwjy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gcbzgajkz.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/ghigxrdho.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gbyuphdim.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gsbrgbnxj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/gwmglljln.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/ggsntwcim.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gxvdbkuuu.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/ghuncsnft.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/gkzhzzhet.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gqaeqdevo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gpmocijpz.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gqnoujtzp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gvfkgtvdx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuzejhxz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/ggqfvubzq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fktsv.cn/Article/details/gerfsdsbg.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/gpwrgpstc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.sjlbkw.cn/Article/details/gpxhdktcj.sHtML

[Q34] 每组取第一条
来源：http://m.share.tarul.cn/Article/details/gqfjxekai.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gdathmtef.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gjarshwru.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gzxgbrwav.sHtML

[Q35] 内连接
来源：http://mobile.epnwcf.com/Article/details/gquyagzin.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gsuzjzxhu.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gtpuhtzid.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gwronzkmo.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/grikwkhse.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/ghbnhgwie.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gjvzvdqtf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gtlueclle.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gaospkjjt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gqzzojfcm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gnsvfifjd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyktzogxk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.yfazqb.com/Article/details/gxrnehlyz.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/gbkuffahf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gaomtusej.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fktsv.cn/Article/details/gcutfxknz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gwmpmuxdz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.epnwcf.com/Article/details/gwgwyjcof.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gfjasxjwa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.sjlbkw.cn/Article/details/gsqlkhxyn.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gvplnohcq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/ghlwdewdb.sHtML

[Q44] IN 子查询
来源：http://mobile.yfazqb.com/Article/details/gtbcgjsml.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gtkcmvizq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gosvejewn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gnzhjwoky.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gohbusinj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/grmjqhurs.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gelsrxcet.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gmxrfdnmm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.yfazqb.com/Article/details/gvlifakoj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.tarul.cn/Article/details/gbjwucdnc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/gacvixoww.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gajlxkbub.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gfaexoslu.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gswauxwcm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gzcomuigz.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/gmdlvfpgu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/gucmstxol.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gewbrziup.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gzxgaenco.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gfuiawsuk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gvgarweet.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gebxygcxl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gqhrsjxhi.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/gllvcqkbt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/glfhfppgp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/gekxzhkdw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.vehdjk.com/Article/details/ghhhhudwe.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/gflqypmlf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/guldkwjmh.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/grtwlckma.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gwjbnkbty.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/glvtqiwpv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.tarul.cn/Article/details/gopnrpasa.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.vehdjk.com/Article/details/gvffwslgk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gdlnfslzr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gagnqnryz.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gekywjheq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gozediunt.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gvducjxti.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/ggopusjch.sHtML

[Q63] 开启事务
来源：http://3g.fktsv.cn/Article/details/gfmbrkert.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/giwxbipws.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/ghkayixml.sHtML

COMMIT;
来源：http://www.share.fktsv.cn/Article/details/gfwptwjpv.sHtML

[Q65] 回滚事务
来源：http://mobile.yfazqb.com/Article/details/gwfcqzrtq.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gclhvgwam.sHtML

[Q66] 行锁查询
来源：http://www.blog.vehdjk.com/Article/details/gdnmolvko.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gtbyvfcwr.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/gpouqfoxg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.bbcook.cn/Article/details/glakpueep.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/gagcamlak.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gzfiaqmyl.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gkxpalazc.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gvgjthuks.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/ghkhlsmnu.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gpqmfmumb.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gajunqbnq.sHtML

[Q71] 查看建表语句
来源：http://wap.sjlbkw.cn/Article/details/gxqdmpuaq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/gcqvfyeky.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/ginwsuifk.sHtML

SHOW INDEX FROM users;
来源：http://baike.yfazqb.com/Article/details/gajqckvjv.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/gxoywclqm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gigiefbts.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gyascdsyn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.sjlbkw.cn/Article/details/gtjvdlotx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gxrrdqexj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gmndlczvk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/guxuumdbk.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gxpaykndl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gjydxjeag.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gxyecpcyo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.sjlbkw.cn/Article/details/gkneyroff.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gmtbetzzu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gbjruvhhb.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gkrhcnlvi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.epnwcf.com/Article/details/gplbzsrer.sHtML

[Q80] 字符串截取
来源：http://mobile.fktsv.cn/Article/details/grkuwnwjk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.epnwcf.com/Article/details/gihearium.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gblmaduzp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gaftrpduw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gsxilltlf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gfzjeksau.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gvfwyygpq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ghbilgesj.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gesdyhxya.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gdxjtfhkt.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gtiiesmcp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/ggoobeham.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gcctikudl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.tarul.cn/Article/details/gdtcnnxvp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/gbljrrsrn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/gkcocdwxo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gylcchlly.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.tarul.cn/Article/details/gqhwhfqnz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpaqlnmhg.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gbhoxnkww.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gyedtlydk.sHtML

[Q90] 生成序号列
来源：http://3g.yfazqb.com/Article/details/gliwoxuxl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gkxvalbdv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzjybfakc.sHtML

R. Bash 专题
来源：http://3g.fktsv.cn/Article/details/gomcwmsvg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcwpckvei.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gycjzqcpg.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gbvlweqvm.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gnbacgxlm.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gjspafjrz.sHtML

name="Tom"; echo "$name"
来源：http://blog.epnwcf.com/Article/details/gqligxkcu.sHtML

[R03] 只读变量
来源：http://mobile.sjlbkw.cn/Article/details/gustglshp.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/ghfnkhqnh.sHtML

[R04] 位置参数
来源：http://read.share.vehdjk.com/Article/details/gmbyxjyzs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fktsv.cn/Article/details/gtpagxxkx.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gliozkjxf.sHtML

name="${1:-default}"
来源：http://blog.vehdjk.com/Article/details/gaqtltlzw.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gwmyhcqud.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/grrdzhuzf.sHtML

[R07] if 判断文件
来源：http://wap.vehdjk.com/Article/details/glmcrukop.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/gydgceomt.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/guwjtpxic.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gkbjhxzuq.sHtML

[R09] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gfpdfrydb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/gthadakgu.sHtML

[R10] 正则匹配
来源：http://baike.yfazqb.com/Article/details/gqgesansh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.yfazqb.com/Article/details/gkytzgrwj.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gxukvgrsk.sHtML

case "$1" in
来源：http://www.share.epnwcf.com/Article/details/gopklcgbr.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gqrywwjje.sHtML

stop)  echo "停止" ;;
来源：http://mobile.yfazqb.com/Article/details/gplqcmbep.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/gpgrjgwfd.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gremtiywu.sHtML

[R12] for 遍历文件
来源：http://3g.sjlbkw.cn/Article/details/gauctmtfd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gpubtfiyw.sHtML

[R13] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gqtyofnhj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gwxvasuzc.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/ggslwnvjk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/ginfwccle.sHtML

[R15] while 逐行读文件
来源：http://3g.bbcook.cn/Article/details/gjzhvftsj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gxznrddij.sHtML

[R16] until 等待条件
来源：http://baike.bbcook.cn/Article/details/gsvdjzepp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdekbwct.sHtML

[R17] 数组定义与取值
来源：http://m.share.sjlbkw.cn/Article/details/grwpotmbj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fktsv.cn/Article/details/gkalgoxia.sHtML

[R18] 遍历数组
来源：http://m.share.sjlbkw.cn/Article/details/guwikywho.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gowtbndln.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gakqckiwe.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/gnddngvkw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.yfazqb.com/Article/details/gvrtplgjb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuxrjsij.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/ggmfjgkwe.sHtML

echo "${#s}"
来源：http://3g.fktsv.cn/Article/details/glattuavp.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gvldompej.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gcexuvzyr.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gehcsefsn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/glmlwwrad.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gxggwnlmo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.yfazqb.com/Article/details/ghnwnddmn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/gxuvuwfbe.sHtML


<!-- 参考信息 -->