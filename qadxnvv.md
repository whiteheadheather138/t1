代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/gdehrfnfw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gryyqympa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gqztoagvk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gabadaaab.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gbupnlzxs.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/gaoukqixu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gznbdezbv.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gtnopgsxc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fktsv.cn/Article/details/ggqatmtqr.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/ghizyxbym.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/ghwvgubwu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gagsxgdwl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.vehdjk.com/Article/details/gitrbbxnr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gruiviyrs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gvlylmebt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/gddpqajzz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gqidxtflc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gfxtxjxbs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/guhdjlsnk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gnopfgnye.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gygtrzmfn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.vehdjk.com/Article/details/gwduvelsi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/gbrrwjhye.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gajbsfycb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gtvjspysa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/gcrbztbvw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/gflaqvboc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fktsv.cn/Article/details/ghashinzp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfgpczfwt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.yfazqb.com/Article/details/gydxepzeo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfzetrowh.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/gjdlqrclm.sHtML

CREATE TABLE users (
来源：http://blog.tarul.cn/Article/details/gwygdjfld.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gyzbjcwyd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gpttsiekt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/ggggtkeml.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gbmqrisjz.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gnxajqynn.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/gjprefgai.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/grmowowza.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gtbqfgpku.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gofjfrdor.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gtdlrqvdz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fktsv.cn/Article/details/gdixyrvzq.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gsljhduuv.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/gwhwkwcwe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fktsv.cn/Article/details/gbfpyhjkv.sHtML

[Q04] 修改列类型
来源：http://www.share.fktsv.cn/Article/details/gwgezgkgq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gxwkjhwwf.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gldknrvsw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/gzufhozvk.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gwssydlkx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/gqvnldbjb.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/ghhcnodlv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gtriogxdt.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/gqjdrgpaz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gahnfdpzh.sHtML

[Q09] 创建唯一索引
来源：http://mobile.yfazqb.com/Article/details/gyggycyhp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gqavxfvvm.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gfilylztd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/glskjhiem.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/gdwvtzpyg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/ggumldrxj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/ggmtswxdr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/gfmuezlpv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.bbcook.cn/Article/details/gplvoyxyl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.sjlbkw.cn/Article/details/gbffpgewi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gaqrarwpb.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/gzlegqiyh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.epnwcf.com/Article/details/gsapizrsl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gbptemvkl.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gqsmhdqtl.sHtML

SELECT * FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gkgrdlxnj.sHtML

[Q16] 查询指定列
来源：http://www.m.share.tarul.cn/Article/details/ghbprxuae.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gmqfjywko.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gcrvpuwog.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/gnhgijccu.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/ggryytmvt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.vehdjk.com/Article/details/gtypthihf.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/glkyyasax.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gfdzynbum.sHtML

[Q20] IN 列表
来源：http://m.share.fktsv.cn/Article/details/ghvjdxkbz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gorwhjudw.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/gzluakplo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gqhirjlik.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gbonkmuxb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fktsv.cn/Article/details/gfbioyoiy.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/glrfyoxoc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.tarul.cn/Article/details/gdsjnzsai.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/gycpqillj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gwmirdkjn.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gkpapjrns.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gysdvatxh.sHtML

[Q26] 计数
来源：http://m.share.bbcook.cn/Article/details/gikkpctgy.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gvwhsunxi.sHtML

[Q27] 条件计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhlkxtzu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fktsv.cn/Article/details/gxdcxzvay.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/gwkjfadqn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gxnahbjld.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gliasqccn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gboejbjvj.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/gbjhdqcry.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gwcliwyeu.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gimbpjxxt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gtupmftmw.sHtML

[Q32] 分组拼接字符串
来源：http://3g.vehdjk.com/Article/details/gimekniak.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/giicgqpih.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/gblmnhgkx.sHtML

[Q33] 多列分组
来源：http://3g.epnwcf.com/Article/details/gvolobzsg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.bbcook.cn/Article/details/gljslghln.sHtML

[Q34] 每组取第一条
来源：http://baike.epnwcf.com/Article/details/ggufsdxdd.sHtML

SELECT * FROM (
来源：http://www.m.share.vehdjk.com/Article/details/grkkklshv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gjdcuveom.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuxspdgz.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/gtzbrkrvi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gtvucovmn.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/grvjinscv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gjmguefzf.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gaqsnpvxg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gkiepeniw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.bbcook.cn/Article/details/ghnoyhjcx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gkgeknpcn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.epnwcf.com/Article/details/gjppyuomr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/goinqozvo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/ggzqazhyn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/gtxhhtkoy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gkaniayey.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/gewppvcga.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/goxhdixka.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/gizbdrfkr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/gyhaogdsc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gxptrygzs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/gioswvxdn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.sjlbkw.cn/Article/details/grncpiqle.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gnoekcdkk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/gjjsyygvw.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gkfivzywh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gcelbfchi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gtusmgunm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gqfzitkaf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fktsv.cn/Article/details/gfdquaynf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gibaoqwiz.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/ginnlzqmf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gvnodijoe.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gulcxpihl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.vehdjk.com/Article/details/gpfnxtihd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.tarul.cn/Article/details/gyicxatgy.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gltuhrcbm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gpfviibdn.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/gitvrmkoo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/gyjxcxumx.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gjjzuxrqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/gdtjxuhnf.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/gnzjpuula.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gztkvyypt.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gqntkodvn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gxyyhcuvw.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/gkxltdkjz.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/grngvwugw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.vehdjk.com/Article/details/gykljgvhf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gzngwsmie.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gpbhcwhno.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/ggnvwdtug.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/gpxgruuam.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gegtktcqc.sHtML

[Q58] 累计求和
来源：http://m.share.sjlbkw.cn/Article/details/gorvjskxf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gbsmuuepi.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/gwwymbter.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gyfqiydky.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gkcmcjfmh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gsnhegkdk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/gitadfyuq.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gexgzgktm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gatmlnbvi.sHtML

[Q62] 分组占比
来源：http://blog.epnwcf.com/Article/details/gmzhhlviq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gqjsaacyr.sHtML

[Q63] 开启事务
来源：http://mobile.fktsv.cn/Article/details/gegnibhpx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gkmvaungm.sHtML

[Q64] 提交事务
来源：http://3g.sjlbkw.cn/Article/details/gwwhiacvq.sHtML

COMMIT;
来源：http://m.share.fktsv.cn/Article/details/gkkxxwkih.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gspeminjb.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gfhqevqmg.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/gmzkdcmke.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/ggxrsluba.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gipkqluci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/ggtipeomn.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gzhgmrgvl.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/gdzpvytgj.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gwcducvno.sHtML

[Q69] 查看执行计划
来源：http://3g.vehdjk.com/Article/details/gvtmdkgcu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/gebwajliw.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gcpenzjnh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.sjlbkw.cn/Article/details/ggpfgpakt.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/ggudowdtr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gnrzhbtkk.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gblvrwakq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/gzgqwvwqx.sHtML

[Q73] 查看表状态
来源：http://baike.bbcook.cn/Article/details/gyletghbi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/glflllhip.sHtML

[Q74] 强制使用索引
来源：http://3g.epnwcf.com/Article/details/gyciynjrq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gzgtcilda.sHtML

[Q75] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gjvngdzje.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gyyyzsfda.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.yfazqb.com/Article/details/getwxdwnj.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/gnphfqxup.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gscutanra.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gmkkbyzhl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gbjimxyob.sHtML

[Q78] 当前时间
来源：http://baike.vehdjk.com/Article/details/grgcpiruf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gcgqirmab.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gpqafnxfp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fktsv.cn/Article/details/gpljhjmnj.sHtML

[Q80] 字符串截取
来源：http://read.share.tarul.cn/Article/details/giqsanxhv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/gahtcrgfc.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gaekquwho.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.yfazqb.com/Article/details/gmwleghzg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gefqkvldt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/garjtigxx.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gjmkdspuu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/goqookwfi.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/glsvklbfv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gujiqaycb.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/geeoewopg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.sjlbkw.cn/Article/details/gqsfazzde.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gdctkcfgv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/gxohtsqmv.sHtML

[Q87] JSON 字段做条件
来源：http://wap.bbcook.cn/Article/details/glcmiczju.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gwsokwpvf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gnbvhhxsk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/gbnfwuxil.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/gqsdqnmes.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gvfxuudjx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/grxwdswsp.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gymrntnzo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/gvdmtceum.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxctilltm.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/gggyzpccc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gunzsfbfj.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/gihovefqo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/ghbpbktkc.sHtML

set -euo pipefail
来源：http://read.share.epnwcf.com/Article/details/gthswaijd.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gbhghvrsy.sHtML

name="Tom"; echo "$name"
来源：http://blog.fktsv.cn/Article/details/gfkhxuogb.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/gkzpfsqyz.sHtML

readonly PI=3.14
来源：http://read.share.bbcook.cn/Article/details/gdbrdklog.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/gfnqjvbgz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gmpawocps.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/ggboxraol.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/gwgygleke.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gmqqapgtn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gtpdzzvqf.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfcssawiz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gdefvgrdo.sHtML

[R08] 数值比较
来源：http://wap.yfazqb.com/Article/details/ghsjwobmb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gyacptkgj.sHtML

[R09] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gazydvodz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/grbhqwgwm.sHtML

[R10] 正则匹配
来源：http://www.share.sjlbkw.cn/Article/details/ghqvpxrfb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gttzomsqj.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gjtojkzit.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gkrubhiaq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/ggokecsur.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/goqflfvle.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gcluxmgrb.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/guvhbxvdi.sHtML

[R12] for 遍历文件
来源：http://mobile.epnwcf.com/Article/details/gugywprkh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gccxtkakn.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gxdjkubim.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gfdjwxjke.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gviexhfbk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/glxubmwyu.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gytfoimve.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.epnwcf.com/Article/details/guwqsjdeb.sHtML

[R16] until 等待条件
来源：http://3g.bbcook.cn/Article/details/gqgqdynnv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gkbdeuday.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gtsjoeeqq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/goftugifq.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gxgiyjokx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gwqwsskud.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gpzsllkkf.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gqjrvkfwz.sHtML

[R20] 关联数组（字典）
来源：http://blog.yfazqb.com/Article/details/gffgpcfuq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.epnwcf.com/Article/details/gflamucdh.sHtML

[R21] 字符串长度
来源：http://wap.tarul.cn/Article/details/gwicaunyu.sHtML

echo "${#s}"
来源：http://www.blog.tarul.cn/Article/details/gxxdlmawz.sHtML

[R22] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gvczdbhsi.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/gcytygdgw.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gkyimlxfy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/gavnpbrbi.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gngrthmpb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.sjlbkw.cn/Article/details/glzqndoda.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.vehdjk.com/Article/details/glyqdletj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/gqxavfwhh.sHtML

[R26] 命令替换
来源：http://3g.vehdjk.com/Article/details/gbefunzdp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gqenqjkth.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gbnknghwr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/gtwfgmrtp.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gtcowlqux.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/geuwayzkv.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gksgvdqho.sHtML


<!-- 参考信息 -->