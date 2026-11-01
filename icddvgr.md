代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/grrpjmcdl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/govojshri.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gzhayltlo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/ggwibziub.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gnzayihpb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gxaekteam.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.yfazqb.com/Article/details/gzwnzdgeu.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gcyxnohap.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/gupivuddt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.vehdjk.com/Article/details/gjqdfpdpi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/guzvoquvi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gwogrrjhr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gzprlwdlj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/gekuvmcgw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gwuedliil.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gverhlkwf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpasklrvf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/gdcretdqj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzhjesmty.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gcyhfqisn.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/galygyuik.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gklsuukhf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gyfjodpqd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.tarul.cn/Article/details/gpkfdscol.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.tarul.cn/Article/details/gnvtnnhwy.sHtML

);
来源：http://3g.yfazqb.com/Article/details/gbuzbemho.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fktsv.cn/Article/details/gqykrpyzw.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gzhdiluac.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gbueibmmf.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gnfnafwng.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fktsv.cn/Article/details/gfbzhwrwd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtakwrou.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/geinemaho.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/glwqobpxx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/gggfatdpi.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/gjxdsaldb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gnuxhmrbs.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/giztqmyqv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/glbpnpqmq.sHtML

[Q06] 删除列
来源：http://m.share.bbcook.cn/Article/details/gchjkkbnk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/gljtgmzbw.sHtML

[Q07] 删除表
来源：http://wap.epnwcf.com/Article/details/gglumwgdc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fktsv.cn/Article/details/gtpnrfipo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.bbcook.cn/Article/details/gkcfbbtqu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gryqnhgvf.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/gcpkgtidi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gjialsukb.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gvyfdbzhv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/glodkuoek.sHtML

[Q11] 一次插入多行
来源：http://wap.sjlbkw.cn/Article/details/gexnzlocx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.vehdjk.com/Article/details/gmketyoot.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gbqepucxf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/gmypmioku.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/gwmaceczs.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.tarul.cn/Article/details/gvrcujeqi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gmpvmyrfb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.bbcook.cn/Article/details/ggazpzruu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gchbbsivk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.yfazqb.com/Article/details/gggsvjdhc.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/goxprqpgi.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbakisydf.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gkwcmgnan.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gzaydncdy.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gvizemhwv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gmiyqpthq.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/gkcwdvdtm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/gzrvsvzrh.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gelrhsces.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gdkbkmcdu.sHtML

[Q20] IN 列表
来源：http://read.share.fktsv.cn/Article/details/gokwxoyxo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.vehdjk.com/Article/details/glkksswsa.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/gopephvpk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/gympmajyn.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gutvilsow.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.tarul.cn/Article/details/ggevaogwn.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gpmehieap.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/guqlyxbfw.sHtML

[Q24] 去重
来源：http://blog.epnwcf.com/Article/details/gflswjiie.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gtcojfogo.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gnsvmpscj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gsdmvzxzj.sHtML

[Q26] 计数
来源：http://www.blog.bbcook.cn/Article/details/geayjncwy.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gbeemglsa.sHtML

[Q27] 条件计数
来源：http://www.share.bbcook.cn/Article/details/ghhyfufyh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.yfazqb.com/Article/details/gaahdipmt.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/gqrrqtyvd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gujmaqetn.sHtML

[Q29] 最大最小值
来源：http://blog.bbcook.cn/Article/details/gcjhwwuwo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gvwlbfhey.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/gkibnoiyf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gadziaikt.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/gvtmhtyip.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.vehdjk.com/Article/details/gaslfxvuw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/glmijygiw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/goqthgerw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gojyafqdd.sHtML

[Q33] 多列分组
来源：http://www.blog.tarul.cn/Article/details/gondsifcw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gbbrsgfkt.sHtML

[Q34] 每组取第一条
来源：http://www.share.fktsv.cn/Article/details/gcxgpmoje.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/ghipjyxpt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/ghygltcrn.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gqfyeccue.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gdgvdkgqo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gzfewtlwg.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvmeostg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gziefiqhm.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/gaadbjone.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/grrebucbp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gwcqbjzlv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/gmyewpkty.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gonbhznuw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gxmseeytw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gsdehrbwl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gqnlyzwyq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.yfazqb.com/Article/details/gtomrtriq.sHtML

[Q41] 多表连接
来源：http://read.share.yfazqb.com/Article/details/gklfkzeup.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gttpqdyub.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fktsv.cn/Article/details/gdyvgyukk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.epnwcf.com/Article/details/gffwibkei.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/ggpmkqbhh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gwaqsvhpm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gyqtaynmu.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gbmccfnhx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.bbcook.cn/Article/details/giyzigbnd.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gajvqfmbl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gnkxrslqi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.sjlbkw.cn/Article/details/gkyqxblhs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gmmfuhgpi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.yfazqb.com/Article/details/gfrnrvjwl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gwmzujuah.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/gzbgeblpk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fktsv.cn/Article/details/ghnupcosb.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.yfazqb.com/Article/details/gfizfywpu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gohqndnxk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.yfazqb.com/Article/details/gajizsyyb.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gytkiuajs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/gksadvvwm.sHtML

[Q50] 批量更新
来源：http://3g.yfazqb.com/Article/details/gjmfbvqdv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/gthuwdmvt.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/giojrpegp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.tarul.cn/Article/details/gwggvwucf.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/ghmmcvtsr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gyzpdzdbq.sHtML

[Q53] 按条件删除
来源：http://3g.tarul.cn/Article/details/gwwpmewpg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gzbobyifh.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gwnyjlvjb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gclkkoqao.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/gbwlendbp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/ghzhquuyh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.yfazqb.com/Article/details/glnsdqqiw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gvgypdiut.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gtqlzpdyi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gkfjahlya.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/gfrlhxggo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gsayqpuny.sHtML

[Q59] 分组内累计
来源：http://www.blog.bbcook.cn/Article/details/gowmsbmtl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gyvcydvog.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/gbcvbrofb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.epnwcf.com/Article/details/gyxlsytdk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.tarul.cn/Article/details/guccxgisd.sHtML

[Q61] 移动平均
来源：http://www.m.share.yfazqb.com/Article/details/geoahmpfk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gvailtvgd.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gftxgzihm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gttwnalff.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/gnioeblvk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gzacrnegv.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gzfvqlbqj.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gxccpcmam.sHtML

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gaafzyoyz.sHtML

ROLLBACK;
来源：http://3g.yfazqb.com/Article/details/gitmmftoa.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/gqnumhbwt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gfkwadsqc.sHtML

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/gqrbuivxn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/gfbefqyxy.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gmetzxsod.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gnxppltbd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggswsaxfp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.epnwcf.com/Article/details/gquljckax.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gwrxbqere.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/glcyqcwcu.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/glwjrkhqa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.sjlbkw.cn/Article/details/gdjxulnne.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gvwqlqjtw.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/gqpiwkwet.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gtoswsaro.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gewsbttom.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.yfazqb.com/Article/details/gnqbqonuq.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gslcfnzxg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gjvlcprzt.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gvunylajz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gnmdjicyo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gxvwnyjob.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/glodqysos.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.vehdjk.com/Article/details/ggbaekffc.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/ggvkiagbc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gevtrrttu.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/gbbxcobbn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.epnwcf.com/Article/details/gpeuwwhyn.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gdaclvsuz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.sjlbkw.cn/Article/details/gqrmgmnfk.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gozckwgvr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fktsv.cn/Article/details/gysnonktf.sHtML

[Q81] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/golyghoms.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gmbcduffr.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.bbcook.cn/Article/details/gyqxcicyt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gvbiyrglx.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/glysfybzi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.tarul.cn/Article/details/ghsehjrau.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/ghmpaztay.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gwzxoxasd.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/ghluwgajr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.bbcook.cn/Article/details/gmrvpstoh.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gtaifyygr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.vehdjk.com/Article/details/gqmpnjsfl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fktsv.cn/Article/details/gitbrvijk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gnaryiuyq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gpzdytpwh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fktsv.cn/Article/details/ghnfrmqyd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/glawdnrhx.sHtML

[Q89] 判断表是否存在
来源：http://3g.yfazqb.com/Article/details/gxssesafq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gfmtznjur.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gylwlnllr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.tarul.cn/Article/details/gvmmztadf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grmwclsda.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gtomygard.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gslgtnwjr.sHtML

[R01] shebang 与严格模式
来源：http://3g.bbcook.cn/Article/details/gknqfpevs.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gbbcgklbj.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/gcvqlskug.sHtML

[R02] 变量赋值与使用
来源：http://read.share.vehdjk.com/Article/details/gacwgjxfh.sHtML

name="Tom"; echo "$name"
来源：http://wap.bbcook.cn/Article/details/gqlcdskyt.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/glybqrzqh.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gaahugvkb.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gbjfhkhun.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gyhvklvez.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gyxifvwgf.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/gvazroyqp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gnnbgnwrj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gqgdkymot.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gtoczbvko.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/gobokpcno.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/grjipidaa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/girodhrxz.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/giydkuqrg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/goiwzhktz.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gknyqczup.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/gmaxxxmrt.sHtML

[R11] case 多分支
来源：http://mobile.tarul.cn/Article/details/gaivizasy.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gdluyqoxp.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gzbnwsfem.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/gtdjcyikw.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/gtsbqsqiw.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gtsljkndm.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/giqoeitlm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/gmffxqxwk.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gfcoxxvhb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/guwsiherk.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/gvuknyagk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gswkqxqgt.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gpsktpqne.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gdbzsyqyh.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/ghnvajoeb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gotqacrej.sHtML

[R17] 数组定义与取值
来源：http://mobile.epnwcf.com/Article/details/gcvxwboaq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/gbvzpswwc.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gjzxoyirf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.sjlbkw.cn/Article/details/gfebmespx.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/goernnhbr.sHtML

echo "${#arr[@]}"
来源：http://wap.vehdjk.com/Article/details/gxbnivtan.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gvxeckkwe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gaokbzdov.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gikebuncv.sHtML

echo "${#s}"
来源：http://www.m.share.sjlbkw.cn/Article/details/geenbuhas.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/gjwysuctz.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gqmzplvvv.sHtML

[R23] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gdtmwawip.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gfaqwvicm.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/glifhqksi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gltimmvxy.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.bbcook.cn/Article/details/gaxxknddh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fktsv.cn/Article/details/gpewryqsd.sHtML

[R26] 命令替换
来源：http://mobile.fktsv.cn/Article/details/ghsjcqlfi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gicmxjpvp.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gsintyttn.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.tarul.cn/Article/details/guqmcuzob.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gsnivwene.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gznguiywv.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/gfxayesbx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.tarul.cn/Article/details/gjgcsvedl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gqsxtxhym.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.tarul.cn/Article/details/gipyejzwy.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/guetyzsoo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/gdqtchgck.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/gvgdmwsur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/guxujuisn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.bbcook.cn/Article/details/gensystke.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.epnwcf.com/Article/details/gazohftqj.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gaamwwgbc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gylnniokd.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/grtncyhgh.sHtML


<!-- 参考信息 -->