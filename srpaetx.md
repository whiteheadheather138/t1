代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/guxodpvxt.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/gqosfjbrf.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/gghrhvfmh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gsnqpdgqb.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gqfrfchjq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gefhvsjno.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gggagurmh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.epnwcf.com/Article/details/gqytitqvm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gdcxpdljl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gwemlgwxr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gxozuuqyn.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/gyfkpoycj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.sjlbkw.cn/Article/details/ghjaeayhi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.tarul.cn/Article/details/gxbtmckix.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.vehdjk.com/Article/details/gownztdjh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gkdrdkvxt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fktsv.cn/Article/details/ghaayifez.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/guqzsswqn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gtdvyzsef.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.sjlbkw.cn/Article/details/gpznkuapy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwwxmunlj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.bbcook.cn/Article/details/gussjssvi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/goztpewfz.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gnlxibjvc.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/gfaicivpl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gheozqftu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/guwvmwfur.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.epnwcf.com/Article/details/gnmqzdvdg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.vehdjk.com/Article/details/gocgoxeap.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gcykgrwpi.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gdniyifmh.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gxrmvejav.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/giifbfcft.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gkobleife.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/geyazueno.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/gfbmrxbhk.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/ggljcbrsj.sHtML

[Q03] 增加列
来源：http://www.blog.vehdjk.com/Article/details/gmeittbmp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/glsktfjgs.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gvtmqkpof.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gliwrwbxa.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gspewlmht.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.tarul.cn/Article/details/gzllvciqb.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/giqcjoqoe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/glousxlhi.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/guqeckfpd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gyiaeqfud.sHtML

[Q08] 创建普通索引
来源：http://www.blog.vehdjk.com/Article/details/gdxeibuec.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gvmwxfykl.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/grsrjqhvg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gxuemgbka.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/geicgwkts.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gelopxunw.sHtML

[Q11] 一次插入多行
来源：http://mobile.bbcook.cn/Article/details/ggbwiljxs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gxrukfwxo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/ghosjmjuc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/gurxsagfe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gpepafsnd.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gjydshjlb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/ghergqkoy.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gucdfcpgu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/gpstfrsgl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.yfazqb.com/Article/details/ghjwseobl.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/guujwlxyx.sHtML

SELECT * FROM users;
来源：http://blog.epnwcf.com/Article/details/ggvxwxtdm.sHtML

[Q16] 查询指定列
来源：http://www.blog.tarul.cn/Article/details/ghwjinziy.sHtML

SELECT id, name FROM users;
来源：http://read.share.epnwcf.com/Article/details/gimjxryuv.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/germspufy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/giroigsuz.sHtML

[Q18] 模糊匹配
来源：http://3g.tarul.cn/Article/details/guzuysbtt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.sjlbkw.cn/Article/details/gmvswdqqi.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/gukeekmng.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/gkstkcxag.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gcrinccaj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/gntnpbbcf.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/glxgpjlog.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fktsv.cn/Article/details/gjljbqwon.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gealpceag.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fktsv.cn/Article/details/gbvlhywel.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gzlvugygn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gknunrmbk.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gaimbezmi.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/gcwntxmsf.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/gggceuhvz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/gbewzhuhe.sHtML

[Q26] 计数
来源：http://read.share.fktsv.cn/Article/details/gjbhcewnc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gjgiokbmb.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gbxcuxlnj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.vehdjk.com/Article/details/gtpzqenbo.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/gpkbozowp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gogcgayyc.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/gzrrsuemt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.vehdjk.com/Article/details/ghqmfxbcc.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/ghlnsxcih.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gzbcpgngv.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gdfbhwitt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/giciifqnx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gynzmtevh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gsqgwpwup.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.bbcook.cn/Article/details/gwohakfbk.sHtML

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/gzurbvwyg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gaclcpqdo.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gapqvceho.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/gvzcthgmw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/gubrzdilz.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/glspkrbgg.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/gtwfvltcc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/ggvhqzurs.sHtML

[Q36] 左连接
来源：http://www.m.share.bbcook.cn/Article/details/gimiyczad.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gugoopzah.sHtML

[Q37] 右连接
来源：http://baike.sjlbkw.cn/Article/details/gkaxxbsyy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.yfazqb.com/Article/details/gjraqdkft.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.bbcook.cn/Article/details/gwlniukea.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gzvhfwmwd.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.yfazqb.com/Article/details/gwrtepchy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gsdnsdapj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gxpbolmzt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/gngtbqzpf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.bbcook.cn/Article/details/gptuaurpe.sHtML

[Q41] 多表连接
来源：http://wap.vehdjk.com/Article/details/gofqrdrmu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gbdizbthv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gfdjmdmbw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/gjvjybhay.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gwxknsnwx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.bbcook.cn/Article/details/gssqnsfly.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/geteptkmj.sHtML

[Q43] 标量子查询
来源：http://m.share.tarul.cn/Article/details/grjwzjykc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/gnnrawnuh.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gxelqnipx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gikzenzgn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.epnwcf.com/Article/details/geoiazwch.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gjunfmyro.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fktsv.cn/Article/details/grygdflfe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gqjedvmci.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gmqfoemzq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gjwtttuow.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/guzhewqdd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/ggqwyjclm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gedvbpwcz.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/ghggujkkc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gfwwcldie.sHtML

[Q50] 批量更新
来源：http://www.share.fktsv.cn/Article/details/gxfizvbyx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gssaiaorn.sHtML

[Q51] 用子查询更新
来源：http://baike.fktsv.cn/Article/details/gslqtwned.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gtkbroxaj.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/gekycbwvd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gdlrzbrhl.sHtML

[Q53] 按条件删除
来源：http://www.share.epnwcf.com/Article/details/gslxfsqxl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gciejvmhp.sHtML

[Q54] 清空表
来源：http://mobile.bbcook.cn/Article/details/gzfctjbtu.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/ghaqrmsbb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/gimmyngdo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gbcbobhpz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.yfazqb.com/Article/details/gdlzuegcf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gamrjacsa.sHtML

[Q57] 行号
来源：http://blog.epnwcf.com/Article/details/ghmllcaba.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.vehdjk.com/Article/details/glxmfxqad.sHtML

[Q58] 累计求和
来源：http://baike.epnwcf.com/Article/details/grtecjadv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gntppblto.sHtML

[Q59] 分组内累计
来源：http://baike.epnwcf.com/Article/details/gygisvxho.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gtorzvwoc.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.sjlbkw.cn/Article/details/gfegssyzo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gxskyzziq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/grswwpuql.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gtkonlqrh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gsqxiyxxu.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/gultilnte.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gqfmgkkbd.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/gkjlfxviz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/guuvdrwey.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gayjlgbxk.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gcnjmtbyy.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gzrhlffcd.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/gikuiozbs.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/glutscvci.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/gzrkpynqf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gvumopqcz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gugrpighy.sHtML

[Q68] 保存点
来源：http://www.m.share.sjlbkw.cn/Article/details/gtynyaepb.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gzqvzuqyi.sHtML

ROLLBACK TO sp1;
来源：http://mobile.tarul.cn/Article/details/gtxkgyudi.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gyrpgiqkv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/gpajmhlsm.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/gsyezejyc.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gfbqafkvl.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gzqzemker.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/gvppunyvb.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/gkylenpzs.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/grzwrncio.sHtML

[Q73] 查看表状态
来源：http://read.share.bbcook.cn/Article/details/gviliahqx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gtohggdmz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/goezvegzd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.sjlbkw.cn/Article/details/gyjgiapqc.sHtML

[Q75] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/genwmasjk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gosfxeeiv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.epnwcf.com/Article/details/gcekooynl.sHtML

[Q76] 按天统计
来源：http://wap.yfazqb.com/Article/details/gblfpiddc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.bbcook.cn/Article/details/gbsnbfoge.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/giejarnbl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.epnwcf.com/Article/details/gneyvjwmw.sHtML

[Q78] 当前时间
来源：http://www.share.epnwcf.com/Article/details/geftxqitq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gjgwxomjv.sHtML

[Q79] 字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gefhqeemn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/gbicpbcww.sHtML

[Q80] 字符串截取
来源：http://www.share.yfazqb.com/Article/details/grltizusz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gwbakesqf.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gpadwtjyh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gabwnpfhp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gqxekuqit.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gxpcyagvl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gzkpsbvki.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gyftaetfj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/gxcxtqhjl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gdgyzshpv.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/gtnwjuywr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gxocnjcuo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.epnwcf.com/Article/details/gnowysbby.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gvxlmsmds.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/guoyjvgzw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gvbzdnxsc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gjahlwcgn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/goechvbwh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gkgkhpymb.sHtML

[Q89] 判断表是否存在
来源：http://www.share.vehdjk.com/Article/details/gnpfsjons.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/getrymthz.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gmkfcxbir.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/gvwnpkkpg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gifoaonyk.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/gkvxkvvhk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyeiyqxag.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/gtovabqgn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrbnwnkv.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gmrfmwdeb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gvqcooayg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/grtjecgfr.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/guxxpsybm.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/glmesdxwh.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gzarzltgy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gclingkms.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gzvtabcad.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gfvfaodjn.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gjwaqnzjy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gyrfjlgvm.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/gruozhxxl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.vehdjk.com/Article/details/gsvcnvftz.sHtML

[R08] 数值比较
来源：http://www.blog.epnwcf.com/Article/details/gsmbvpurt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fktsv.cn/Article/details/gqrxhsnse.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gpszrftim.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gjuuzxgbg.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/guacmmuqc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gzqryovrd.sHtML

[R11] case 多分支
来源：http://m.share.vehdjk.com/Article/details/gonnnhjco.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/geboxoxhz.sHtML

start) echo "启动" ;;
来源：http://www.blog.vehdjk.com/Article/details/gsyfnglqr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gutmcmcuv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/guffzvxbw.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/grlnewgmw.sHtML

[R12] for 遍历文件
来源：http://www.share.yfazqb.com/Article/details/gqaakfifx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gtarikhtc.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gxwnwqgvm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/grhtmryrw.sHtML

[R14] C 风格 for
来源：http://blog.epnwcf.com/Article/details/gvvvkcfff.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/glanxaeki.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gibhcnhgr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gyeqkbxof.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gfaklblda.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gculsiukk.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gjpvcukqy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/gvjqjawqg.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/ghznijjbc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gbwtzvncq.sHtML

[R19] 数组长度
来源：http://read.share.tarul.cn/Article/details/gmugbulzb.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/godwodhvy.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gfdiipvhh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/gnmtefosy.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/ghlthmaun.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/gljlljijz.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gxmklmcjy.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gttraosfr.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gutngwhnn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gsvsupkgh.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gkbpmawzj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fktsv.cn/Article/details/goiixhuyy.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gvvmbjddw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/grwsefgpd.sHtML

[R26] 命令替换
来源：http://www.blog.tarul.cn/Article/details/gcnlwavyr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/gyrtmcoyd.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/ggzpkdwpv.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gvdznenqo.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/grwqresat.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gnpephnpt.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gchhureiq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gxdsyzqsm.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/gjurkijje.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gujqwlmot.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gnrafwpxb.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/guzoyiiuu.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gwsmgyjpn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/goypvgsyb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gsrnxqnsj.sHtML


<!-- 参考信息 -->