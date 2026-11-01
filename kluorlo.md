代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.sjlbkw.cn/Article/details/gowfyfsyn.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/gegcfdgac.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/gkhjovngh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.yfazqb.com/Article/details/gqwqrnwvx.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gcodcrymt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gmbahxgmj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/glnvkxyve.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/gzbpanola.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gfxghqbuq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/galltlter.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/gqzcxexge.sHtML

[P08] 处理浮点精度问题
来源：http://blog.bbcook.cn/Article/details/geavkuxlg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/giojyggww.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/gwyaobahn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.yfazqb.com/Article/details/gblxjqfmw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/glxxmkejn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/gtcwkfmxe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.epnwcf.com/Article/details/gjyitvlom.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.epnwcf.com/Article/details/gzmcrglcx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/gftazeesj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggfljdiwp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gjpcxkvrc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkvnqougl.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gnueeysux.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gngvwhexx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gngfdeljs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gcepcmabc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.sjlbkw.cn/Article/details/gpqskbkvd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gsufxsocx.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gqakqgvfr.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/geysnnztb.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/gkekbvzhh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gyibhwchh.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gajaxpusx.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fktsv.cn/Article/details/gvgheltsp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/gypevuoij.sHtML

);
来源：http://wap.vehdjk.com/Article/details/glddtxjqg.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/gzhrizqhx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gsdzhczpr.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gzufsemum.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/gvmzgzpbh.sHtML

[Q05] 重命名列
来源：http://www.m.share.epnwcf.com/Article/details/gxofrfmbj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gpctyzbsk.sHtML

[Q06] 删除列
来源：http://read.share.tarul.cn/Article/details/ggnjnouyv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/glvpvscvi.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/gxbhvrksc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gsxywnbdn.sHtML

[Q08] 创建普通索引
来源：http://mobile.epnwcf.com/Article/details/gepbpxkyd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gqjafhlbc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/grystbsda.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gsbfbpssl.sHtML

[Q10] 插入单行
来源：http://wap.sjlbkw.cn/Article/details/gimytehhk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gleczmiyo.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/girewjnzr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/guzfeqiho.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gnnchiixt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/grvogywfb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gsgdnlkch.sHtML

[Q13] 忽略重复插入
来源：http://3g.vehdjk.com/Article/details/gvabkobap.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/grqyzeroh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.bbcook.cn/Article/details/gkwvsmsxu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/gqljylmtw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/ghuaefboe.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/geuisiwxe.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/geqlvjdgf.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/gdivtnhud.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/grkzoxmhd.sHtML

[Q17] 条件查询
来源：http://www.share.sjlbkw.cn/Article/details/gtjbpnfvv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gmerpyfjc.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gphxfaybj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gqzctlbll.sHtML

[Q19] 范围查询
来源：http://baike.fktsv.cn/Article/details/gbgqxrewa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/glgjbxibk.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gyikdynpk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/ghmioquvt.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/gljkwcjwr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.vehdjk.com/Article/details/gerekkdqv.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/gsbtazdwv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.sjlbkw.cn/Article/details/griyvdzhj.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gmuimsiay.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/ghjwthhsb.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/ghdamphnf.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/gfgyownhx.sHtML

[Q25] 只取前 N 条
来源：http://blog.bbcook.cn/Article/details/gyogffzqz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gchzvbsvz.sHtML

[Q26] 计数
来源：http://mobile.bbcook.cn/Article/details/glzyxpggb.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gysrynbjd.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gaunnkxjv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/govokjszc.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gmecvmcst.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gprittzyq.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gmtqnwteo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gnjqqnmvb.sHtML

[Q30] 分组统计
来源：http://wap.tarul.cn/Article/details/gwumdbjhe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gyxayqlvd.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gbebcligw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fktsv.cn/Article/details/gikciqhom.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gcfyzxsyw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gnfjehsjo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.tarul.cn/Article/details/gjkvjsicr.sHtML

[Q33] 多列分组
来源：http://m.share.epnwcf.com/Article/details/gfpafwvha.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.yfazqb.com/Article/details/gqtxvbmxe.sHtML

[Q34] 每组取第一条
来源：http://m.share.epnwcf.com/Article/details/gnkafxbid.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gpozrwchb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gphtmbkga.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/grlqvhbuf.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gpceoophs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gxbopjkqt.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/gugtlgevg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gstavgkdm.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gtyrdniit.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/gfmowtaiw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.sjlbkw.cn/Article/details/gkcrfjfpu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/gdkrickgy.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gsvlfumkp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gnlrmcbee.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gkqtuqpmo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gsnbkqikq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gckzeipry.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gkhdhvrkt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/guwmiazrf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/gtrilpbmk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.yfazqb.com/Article/details/gtfrohawy.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gnqkfaieq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gsengmmxu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/glwoyffso.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gzftbqmvg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/guqbafbhp.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/geqelazhw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.epnwcf.com/Article/details/gkxisggaj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gchxqdhkr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gxugnojeh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.vehdjk.com/Article/details/gfxsopecx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gxuwsyysi.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/govyopjav.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gfcycuruw.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/gvmhmmbrg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fktsv.cn/Article/details/gtspyhtco.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.vehdjk.com/Article/details/gmoeeqkms.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/grdtcwcif.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gkvxqxxxz.sHtML

[Q50] 批量更新
来源：http://baike.tarul.cn/Article/details/gujeaexmt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gqjvnnfoc.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gnybravqy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.yfazqb.com/Article/details/grdcxhxyv.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/gbixldigp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gfddvernr.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/gsnaspcil.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gtopvsrmo.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gunhmzoyl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.tarul.cn/Article/details/gjfrnzdoc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gnevnjvtl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.yfazqb.com/Article/details/grvuihjwp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gjiknoxqa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/geceogzrs.sHtML

[Q57] 行号
来源：http://www.share.tarul.cn/Article/details/gefhjctve.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.epnwcf.com/Article/details/ggorxirgi.sHtML

[Q58] 累计求和
来源：http://mobile.epnwcf.com/Article/details/glvltgxdl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gmbihdjku.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gbtnwtemn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.vehdjk.com/Article/details/ggofvxgyx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/gcuebfzgg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fktsv.cn/Article/details/gqizmgerl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/grhrvjbox.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/ghseimmqu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gmgvalnhd.sHtML

[Q62] 分组占比
来源：http://read.share.yfazqb.com/Article/details/glartinaj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gptakrvat.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/gclckabpx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gtchkzuxo.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gnqieihyc.sHtML

COMMIT;
来源：http://m.share.bbcook.cn/Article/details/gpmmknzjk.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/ghwbxtpfd.sHtML

ROLLBACK;
来源：http://www.m.share.bbcook.cn/Article/details/giirirtvs.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/gtbfkrkde.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.bbcook.cn/Article/details/gwjtthukv.sHtML

[Q67] 设置隔离级别
来源：http://mobile.yfazqb.com/Article/details/gbzagtncp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.bbcook.cn/Article/details/garcufgpk.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gbipvfvws.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gkhhofqog.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gflfaumid.sHtML

[Q69] 查看执行计划
来源：http://read.share.sjlbkw.cn/Article/details/ghnbgifpe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fktsv.cn/Article/details/gefwyhqvb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/grdbbqbup.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gcceprkyv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/grgdgtgry.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gwajnzuxn.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gfknllpqt.sHtML

SHOW INDEX FROM users;
来源：http://read.share.tarul.cn/Article/details/gwubflczp.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fktsv.cn/Article/details/gqjsdwhau.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gnqpvvssl.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gtcsskhsu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gfcbxaljg.sHtML

[Q75] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/gllluesnk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/gndyzjoni.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gzerfrzjc.sHtML

[Q76] 按天统计
来源：http://3g.tarul.cn/Article/details/gupsushem.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/glnlcqpwj.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/ggbofdkmi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/gtpysagqx.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gtetzwhzy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.bbcook.cn/Article/details/gwejamwwm.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gfyypdpnf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.bbcook.cn/Article/details/gvisrazpt.sHtML

[Q80] 字符串截取
来源：http://wap.fktsv.cn/Article/details/gehysjavc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gkidezrvc.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gmdcsoqls.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gebtkkjbd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/ggxsaqmrd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gdavihkmw.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gqoqkpnqu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gqbvefoxm.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/glktkgyyk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/ghymjhemz.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/gxsnmrook.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/gksdtdsga.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gbfgauxeu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/gnwrnmbnh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.tarul.cn/Article/details/gobtdpyyf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gvacfqmof.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gtwwoslha.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gzpzdaiyf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gqbahcdcj.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/geldqgqhz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgeazdsg.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gpovrfigp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gmpxtjxtb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcjyczgwe.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gxslyhzti.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gybultcrq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gywaravyi.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gmwrwtqvh.sHtML

set -euo pipefail
来源：http://www.m.share.bbcook.cn/Article/details/ggmqdzmtm.sHtML

[R02] 变量赋值与使用
来源：http://read.share.vehdjk.com/Article/details/gvukatcpj.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/grghovqqd.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gddwmwyfn.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/gapjzevhx.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gxqkqvkua.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/giickxaog.sHtML

[R05] 参数默认值
来源：http://www.blog.epnwcf.com/Article/details/gsmhbhpdb.sHtML

name="${1:-default}"
来源：http://read.share.vehdjk.com/Article/details/ghwquwkkn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.yfazqb.com/Article/details/gqndzwqic.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gvubsiozy.sHtML

[R07] if 判断文件
来源：http://www.blog.vehdjk.com/Article/details/ggpnqysjk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/gdnbcdkgz.sHtML

[R08] 数值比较
来源：http://3g.epnwcf.com/Article/details/gwuajuoqu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gogblsxee.sHtML

[R09] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gjmysmzlq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gyxlnfxqa.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gdqtwleba.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gszpxqjzr.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gytajejof.sHtML

case "$1" in
来源：http://www.m.share.tarul.cn/Article/details/gqkmlatmn.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gurxmanfr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.epnwcf.com/Article/details/gaiwxlvtg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/gfzhmezwu.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gkwgrcxqa.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gplcnulji.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gzfspbevq.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gnnjbhpuj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gtcwnprwr.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gexzzssuw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gawlyvnqr.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gowucbpde.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.sjlbkw.cn/Article/details/gearemyes.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/gbbffhdtw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/goydajlpy.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gsztjhaio.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gydffwqej.sHtML

[R18] 遍历数组
来源：http://m.share.yfazqb.com/Article/details/grqqhqhbk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/gwgbcmgbh.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/gsesiwwfd.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/gfuznptlt.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gosupnkgf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.sjlbkw.cn/Article/details/ghadtwcxt.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/goaxvvldw.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/gftgjwmnr.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gwdqgxpci.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gpjvnhamu.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gutxvydri.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/geucbtgds.sHtML

[R24] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gtizdhltw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/gorfirwek.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gyfoizpzc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gzohpdnhc.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/givlveyye.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.yfazqb.com/Article/details/gfvdjbztl.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/gwuoiiaha.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gsmvzibzd.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gmsbmpawe.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/gjhahudnm.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gkthczihp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gngfodaey.sHtML

[R30] 函数返回状态码
来源：http://m.share.bbcook.cn/Article/details/gdmjorhgb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gqmuwfjxm.sHtML

[R31] 局部变量
来源：http://mobile.epnwcf.com/Article/details/gcuhxtmrg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gtuecvzhg.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gkyqfmjnw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gexrwxmhk.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/glmzvwuqb.sHtML


<!-- 参考信息 -->