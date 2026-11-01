代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gzocicscp.sHtML

C#:   if (x is null) {}
来源：http://blog.bbcook.cn/Article/details/gghnkwbkh.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gxwgmcfib.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/grqcnnuof.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gsgozyzhw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gxqvvogqi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gkjueftyq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.yfazqb.com/Article/details/geelaffrs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/glbhbzqor.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/ggnkoggqs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.yfazqb.com/Article/details/gcojmpwrw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gbkkrevcm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/gofbhvqie.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gbknyphve.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/gwlqgmimz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/ghefmcsna.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gdbpkaoxk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/gunyldnrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/giwpyngkx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gfoioicdf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gejadujng.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gtzghvykd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcsecmyyf.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gtmuiydyv.sHtML

CREATE TABLE users (
来源：http://3g.bbcook.cn/Article/details/gooouzoyn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/ggwzabpct.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gsbubkphf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gwmrhqhng.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.sjlbkw.cn/Article/details/gcnfysggh.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gbpsfrmnc.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gzedyblfc.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/gxgbhycdf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/geustokkn.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gyehdzhss.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.bbcook.cn/Article/details/gjiirkbdx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gyhnvdymx.sHtML

);
来源：http://baike.yfazqb.com/Article/details/ghcduistw.sHtML

[Q03] 增加列
来源：http://www.m.share.yfazqb.com/Article/details/gdwlenyqu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gcckwjryz.sHtML

[Q04] 修改列类型
来源：http://www.m.share.vehdjk.com/Article/details/goipjdewh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.bbcook.cn/Article/details/gmvxlbljn.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/gxlxsterz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/gxpvbzass.sHtML

[Q06] 删除列
来源：http://mobile.yfazqb.com/Article/details/guioyjjnz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.yfazqb.com/Article/details/gcxttykzv.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gydaxciqg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/gebdijadb.sHtML

[Q08] 创建普通索引
来源：http://read.share.sjlbkw.cn/Article/details/gpcdlbobb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/getnrakhg.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/ghpbjwndk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gehqujeng.sHtML

[Q10] 插入单行
来源：http://baike.fktsv.cn/Article/details/gtbwvqzae.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.yfazqb.com/Article/details/gyaexzwzd.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/gmwmkchhw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/gpaocrehb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gmixkpbuf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.yfazqb.com/Article/details/gfqsirxie.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gnlepvapy.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.bbcook.cn/Article/details/girxzqxhv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/gzzustozj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gfolcsaco.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fktsv.cn/Article/details/gckagfshs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gosaichcl.sHtML

[Q15] 查询全部
来源：http://www.m.share.tarul.cn/Article/details/gyloshnbz.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/gwzvnsqvo.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gazqepigc.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/ggjijcazf.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/gbtxeampu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gcvnapsrp.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gybowppaj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.sjlbkw.cn/Article/details/grcwxifby.sHtML

[Q19] 范围查询
来源：http://baike.bbcook.cn/Article/details/gnmpovksj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/gcyheogct.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/gxvwqclpg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fktsv.cn/Article/details/ggmekgkjq.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/gktzqkjhz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gqtswsjit.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/gvfaajreh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/grzjvruet.sHtML

[Q23] 分页
来源：http://wap.tarul.cn/Article/details/gwunqpxyz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gkntmanok.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/guuhtykfk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.vehdjk.com/Article/details/gvnraphix.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.epnwcf.com/Article/details/gfbtroutv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fktsv.cn/Article/details/gcqbmlvjb.sHtML

[Q26] 计数
来源：http://www.share.fktsv.cn/Article/details/gdybcxvur.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gmqduignl.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/gvdvtmivi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/gpcgkdyyi.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/gofelxtds.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gundqdklo.sHtML

[Q29] 最大最小值
来源：http://www.m.share.epnwcf.com/Article/details/gwuxwqxva.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gmgzoeays.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/gwosegpoi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gflsigwkt.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/ggopgrqom.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.bbcook.cn/Article/details/giuiciktj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gsigrajfn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gxvtmowaa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.tarul.cn/Article/details/gwubjoxxr.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/grurqicbw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gpuapapul.sHtML

[Q34] 每组取第一条
来源：http://mobile.tarul.cn/Article/details/gproejloo.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/gqaoycilq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/grigssgnt.sHtML

) t WHERE rn = 1;
来源：http://m.share.epnwcf.com/Article/details/gxfnearsi.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gflqebahm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/glgpfksjv.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gtsrsouyu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gjornkpiw.sHtML

[Q37] 右连接
来源：http://www.share.fktsv.cn/Article/details/gzkzrvudm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.vehdjk.com/Article/details/ghkybukje.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/gqpgwmccv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gbmifjjtc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gktvjhqfy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/guktujxls.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gsholdtuk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gnpwsqaze.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gbwczucrr.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/goqzyycwi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gagdjbzwb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gtxsxzcns.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gjsczqohd.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gdgqkxdlz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gcanfyfyi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/gsmfomxqj.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gfifldqwr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gsfxpbonb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gftueewcv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fktsv.cn/Article/details/ggvrrycvq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gozqeextm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gcjfaprfb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.bbcook.cn/Article/details/gntyjxfgk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnktlwscc.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gtwfvqxpj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/gctqssjws.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.tarul.cn/Article/details/gofppmcej.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/gijippbeg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gkcxxldmz.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/gwrkpytzs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gvsjkjcbn.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gvfdtfgoh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gziwmnlcd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.vehdjk.com/Article/details/gqewcryax.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/ggtlwrgzh.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gmjkvggoo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gahqfbpvk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gsztmdgjc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.yfazqb.com/Article/details/gkvazqnns.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gntxngxvn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.bbcook.cn/Article/details/gthbeaoah.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gzyvvqnyr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gkyraqcag.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gatmpwszf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gvtenehkt.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/grbmttldw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.vehdjk.com/Article/details/gvubaqbyp.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/ghutqqwbr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.yfazqb.com/Article/details/glksvviye.sHtML

[Q59] 分组内累计
来源：http://baike.fktsv.cn/Article/details/gicsxrogc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gwczvuylz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.vehdjk.com/Article/details/gilgookjl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/goqyziqjb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gnlzaldeh.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/ggaxoloci.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/grqushojf.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gdyuwbgkc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gjkdcxibv.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/gbqqvajbp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/gldbfsjtf.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gbpxyyazf.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gtjylqoby.sHtML

[Q65] 回滚事务
来源：http://www.blog.bbcook.cn/Article/details/gcgxeoxbb.sHtML

ROLLBACK;
来源：http://mobile.sjlbkw.cn/Article/details/gvhodnffj.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/gervlwkbm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gjhxnzgje.sHtML

[Q67] 设置隔离级别
来源：http://m.share.epnwcf.com/Article/details/gwlnilpxd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/ghkiktgvb.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gbrcedjep.sHtML

SAVEPOINT sp1;
来源：http://blog.yfazqb.com/Article/details/ghghebgci.sHtML

ROLLBACK TO sp1;
来源：http://www.share.vehdjk.com/Article/details/gwwzxglzj.sHtML

[Q69] 查看执行计划
来源：http://m.share.vehdjk.com/Article/details/gnsgiklkf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/glbcxjovq.sHtML

[Q70] 更新统计信息
来源：http://read.share.yfazqb.com/Article/details/gqnpmqqey.sHtML

ANALYZE TABLE users;
来源：http://3g.bbcook.cn/Article/details/gvbejkrvh.sHtML

[Q71] 查看建表语句
来源：http://3g.bbcook.cn/Article/details/gihqvpltw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/ggjwsjpjc.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/gxhoqhgob.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkkvwmxcs.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/gvlqbsepk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gznokhnmm.sHtML

[Q74] 强制使用索引
来源：http://mobile.tarul.cn/Article/details/ggzrrcsgh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/ggivdbzuv.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnjjygcx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gyecawjfy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/gtuencigg.sHtML

[Q76] 按天统计
来源：http://www.blog.tarul.cn/Article/details/gipypzbns.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/gfesngody.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gejgjhivh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.bbcook.cn/Article/details/gtletatle.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gcbkdpslq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/gjjnnwulf.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gptlgvgks.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.sjlbkw.cn/Article/details/gqzjzagew.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gpovtvpiw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gwjiqsnkq.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gtoqjaubr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/gjumlpxxn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gsjixmrbr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gyolbspny.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/ghqndafkb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gtaqffvgs.sHtML

[Q84] 去除首尾空格
来源：http://wap.bbcook.cn/Article/details/gqzezbmip.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gsdvuuzyu.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gincodafq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gdctgphbn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/gluunddus.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gqsvzmscw.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/gldqzlrcf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gjcjdogsq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.epnwcf.com/Article/details/gjgldtchi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.vehdjk.com/Article/details/gfmlfywxn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/giooedpkx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gooplrynt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/govfkxdci.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gyfxolfcj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.bbcook.cn/Article/details/gsufvldgj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvsvniaby.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gbdtxeqix.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjuvdnfdl.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gdtxujciu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fktsv.cn/Article/details/ghvqargft.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gqaqhgutw.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/gusxdtbjg.sHtML

name="Tom"; echo "$name"
来源：http://baike.sjlbkw.cn/Article/details/gjtkghnfl.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/glsveikoo.sHtML

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/gxsspkhnh.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/gcxkmrzwa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gikefizns.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/gcaxhmptw.sHtML

name="${1:-default}"
来源：http://m.share.vehdjk.com/Article/details/gaecggovj.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gqsrdrkmu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gszwjplaa.sHtML

[R07] if 判断文件
来源：http://www.m.share.epnwcf.com/Article/details/ghwzqspjn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fktsv.cn/Article/details/gdoggxuhp.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/geinwtyti.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gtotxyyee.sHtML

[R09] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/gayuhhcur.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gvivbdlch.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gzepqxhuj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/gagyfjgtk.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/gnlaplnlg.sHtML

case "$1" in
来源：http://m.share.tarul.cn/Article/details/gcuxpusux.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/glthopbub.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gjbcimglf.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gruuzcbox.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gywkgxarm.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gmqlliwxo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/gbabzqqoh.sHtML

[R13] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gdfedhega.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/glfplnlca.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gmxuvtyyn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gzwfjjvmf.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gffudlbiq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.sjlbkw.cn/Article/details/gtywzmkfp.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/glpohlxsc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/glluspjrh.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/ghcewlgum.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/graozzjix.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/grcgfktxg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gowkwpvvq.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gvmlcigyn.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/guywjmcuz.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/grlfepyyv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gjpnmxgfe.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gwsjbbygy.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/gelnlbemn.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gnplmdine.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/grpudnthz.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gpdgulzqy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/grefoearr.sHtML

[R24] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gyxssspou.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.sjlbkw.cn/Article/details/gajtxqfkt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.vehdjk.com/Article/details/gblkgfjed.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/ghhdwaipc.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/ganzfvjxm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/gdkfcgodn.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gmxavhllb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/grnqfsogu.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gyznkjoja.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gdfqulnec.sHtML

[R29] 定义函数
来源：http://mobile.tarul.cn/Article/details/gpvsnrrhe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gwhuspyul.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gbrluiufr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/gaucrvcal.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/goalejejo.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gjcgxpyfi.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gqidbllwp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/garizjkex.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gmgfabjrf.sHtML


<!-- 参考信息 -->