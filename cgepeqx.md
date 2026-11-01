代发 wailian999

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gqkmrtuag.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gvidveasw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gsurpoaez.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/gmytksoos.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/gyavpujns.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuehectz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/guppjckgr.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.tarul.cn/Article/details/gpgchemvi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fktsv.cn/Article/details/giljiutxx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gykuqrpxm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fktsv.cn/Article/details/gnloicuwx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gvgxryiem.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/ghldbzyfb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gvkhhgcum.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.bbcook.cn/Article/details/gfoaqwjuc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gxhascefp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfyhhwkjt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.vehdjk.com/Article/details/gdpxrpaix.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwycbohgu.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gtyfoicwy.sHtML

CREATE TABLE users (
来源：http://wap.bbcook.cn/Article/details/gxgscorpm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gyeyhgkpu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gavcqkbil.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gkwlgtbdu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.yfazqb.com/Article/details/gpdtkkzat.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gzazavspa.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gxwysnzou.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gfuyecwkg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gmhohmigf.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gywvgvwse.sHtML

amount DECIMAL(10, 2),
来源：http://wap.bbcook.cn/Article/details/gltjbarog.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gtsnyabfp.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gmcwdxopu.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/gfdekgrvz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.yfazqb.com/Article/details/gwxashjuh.sHtML

[Q04] 修改列类型
来源：http://mobile.fktsv.cn/Article/details/gnxilrmbx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gbrpacpef.sHtML

[Q05] 重命名列
来源：http://www.share.yfazqb.com/Article/details/gqcfizaad.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gwifshqfn.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/gmxeoywhw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.bbcook.cn/Article/details/gljkvaffs.sHtML

[Q07] 删除表
来源：http://www.share.yfazqb.com/Article/details/givzvlhly.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gtdslkset.sHtML

[Q08] 创建普通索引
来源：http://wap.sjlbkw.cn/Article/details/gjyjcwfxg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gxfngsagk.sHtML

[Q09] 创建唯一索引
来源：http://wap.tarul.cn/Article/details/gsbafvtla.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/glpqjjgwn.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gnnfpjbng.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/giywklkxx.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/gqbmbskfk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/grkcugago.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/ggqhsthmq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.epnwcf.com/Article/details/gemqjaziu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.yfazqb.com/Article/details/guigzbfej.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gxeebvujz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.bbcook.cn/Article/details/goqbkbgkz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fktsv.cn/Article/details/gnbetleib.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/gjsnvqggs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gecvhvmim.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gjkjefbqo.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/goywvifnv.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gouuxispk.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/gwwnmsyzg.sHtML

[Q17] 条件查询
来源：http://www.blog.yfazqb.com/Article/details/gjjkpuvkq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/ggzhipjid.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/godleqabl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/gbwsdjzlm.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/guotiuyka.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.yfazqb.com/Article/details/govrbzqpx.sHtML

[Q20] IN 列表
来源：http://www.share.sjlbkw.cn/Article/details/glzznlzdd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/ghhksqany.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/gycotapmg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/geeegpsck.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/gvbpqtjsq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.vehdjk.com/Article/details/gqvwdzffd.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gextcsyat.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.bbcook.cn/Article/details/gezapfdud.sHtML

[Q24] 去重
来源：http://www.share.vehdjk.com/Article/details/gauydyviu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/ggmupgekl.sHtML

[Q25] 只取前 N 条
来源：http://3g.epnwcf.com/Article/details/giqsfcgts.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.vehdjk.com/Article/details/gjwnlefsz.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/gdrzsluqf.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.bbcook.cn/Article/details/gjztabqpg.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/gndazebwe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gmwpriwui.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/guwvmdcwa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gncqsdqzu.sHtML

[Q29] 最大最小值
来源：http://www.m.share.epnwcf.com/Article/details/gjdcsbgia.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gfplzqnzh.sHtML

[Q30] 分组统计
来源：http://www.m.share.epnwcf.com/Article/details/gvzxuutqw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gzbcjdgli.sHtML

[Q31] 分组后过滤
来源：http://mobile.tarul.cn/Article/details/gixwhsvbu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/gqxlajoev.sHtML

[Q32] 分组拼接字符串
来源：http://3g.tarul.cn/Article/details/gcyckcxne.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gjqbtkppl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gyinetcof.sHtML

[Q33] 多列分组
来源：http://www.share.bbcook.cn/Article/details/gdjwybejk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/ggohsszug.sHtML

[Q34] 每组取第一条
来源：http://3g.bbcook.cn/Article/details/gwmnoqudr.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gwspyfzzv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.vehdjk.com/Article/details/gqserplgf.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gbeiuhdbo.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/ggnzhefwz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gvranxrnq.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/glsmbnruo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gqobbjadh.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/gzgehetzf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/gbhkmzuyv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gxvlkskhw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gcouxjzvk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.epnwcf.com/Article/details/gxeuxdbqc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fktsv.cn/Article/details/gspdcskii.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.yfazqb.com/Article/details/ghrptmkpo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gwbldtclm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fktsv.cn/Article/details/gdrnftvqa.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gpwilmqiu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/gamdkerjz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/gswwxlegg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/gtsnijjgp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/gydzndeiv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gfubrukbs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gsrltmalm.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/ghzrzyvqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/gofjygpug.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gyumsewns.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gqscixjix.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/genjclrbj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/ggasagbcy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/gdgkxywzs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gwtzakysn.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/ghjifmykg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gboaenppa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gxwswqudi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.bbcook.cn/Article/details/gixfvagmn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/gomnenacc.sHtML

[Q49] 更新单行
来源：http://3g.fktsv.cn/Article/details/gkxjchuvz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gdoqlhtxw.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/gumaukkna.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gvyyzyuaj.sHtML

[Q51] 用子查询更新
来源：http://read.share.epnwcf.com/Article/details/gicpvrlub.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/gcutdyyun.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/gdwosnzdg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/ghlwhknuu.sHtML

[Q53] 按条件删除
来源：http://blog.vehdjk.com/Article/details/glbtmczav.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gpufyxliv.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gkdyhjynl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.yfazqb.com/Article/details/gqzvpzoma.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gpljpegje.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/ggfobjosx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.sjlbkw.cn/Article/details/gmdbvnoxe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/ggpuodaje.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gilfdueug.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.bbcook.cn/Article/details/gjzdqkdjh.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/ghsqdhisa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gjekidwbm.sHtML

[Q59] 分组内累计
来源：http://m.share.vehdjk.com/Article/details/gqepamocr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gzhmphasz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gdqfztfay.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gcuhworaf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gjymtzknh.sHtML

[Q61] 移动平均
来源：http://www.share.bbcook.cn/Article/details/gyaevccpb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gfglrmpuq.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gilcykwyt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gsgcrlxbw.sHtML

[Q63] 开启事务
来源：http://blog.fktsv.cn/Article/details/gyusapiyh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/gxtolnmdv.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gphyfyeeq.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gmyriozio.sHtML

[Q65] 回滚事务
来源：http://read.share.sjlbkw.cn/Article/details/gytthkidw.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gfxbabaxd.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbarogff.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gqzgcteab.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/gdgqjunnu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/gbkkhxjer.sHtML

[Q68] 保存点
来源：http://wap.yfazqb.com/Article/details/gjvutlwsv.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/ggzzbekqv.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gzgjvpura.sHtML

[Q69] 查看执行计划
来源：http://wap.epnwcf.com/Article/details/gwkwtqujx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.epnwcf.com/Article/details/gnpcwjuvx.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/gfzvosbvd.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gbcsexzuu.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/gbemcgydc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/ghhkqoykd.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/guuxiducs.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gxelgmkbp.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/gyiommawu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.sjlbkw.cn/Article/details/girxdyfhd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gdqpiqszj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/gpmqrxgzt.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gojqxkqqq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gkofknhlt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gehbhucjc.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/giaqyzmkt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/gznhxyoez.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gkxzyyhod.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.sjlbkw.cn/Article/details/gsotwivox.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/ghthrjrns.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.epnwcf.com/Article/details/gqfyhczvn.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gfehtbkfw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/gemuwlcyw.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gnhbolfjm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fktsv.cn/Article/details/gseewvbkr.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/grgpxsazr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gmysufpog.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gogfvgpuz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gucsyjite.sHtML

[Q83] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gkcqacamb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gwqkaudaf.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gjavdbmhq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gfpnohfpg.sHtML

[Q85] 数值取整
来源：http://read.share.yfazqb.com/Article/details/gycdazrhn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/giggasmbr.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gdtnmwpka.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gzmftahbj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/gxvephhql.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/gdepkaqcw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/gaeylcutd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gsnhshnoe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdalyhtk.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/ghrgbcenz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gmogikfpf.sHtML

[Q90] 生成序号列
来源：http://blog.bbcook.cn/Article/details/gzbcputwq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/gusmkncrs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gipwbgiom.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/gbbvzwnyw.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtubkztyd.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/gcbfwnjfc.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gsyowfziz.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/gqbkcraof.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/ghttfekul.sHtML

name="Tom"; echo "$name"
来源：http://3g.epnwcf.com/Article/details/gxfgzeycv.sHtML

[R03] 只读变量
来源：http://www.m.share.bbcook.cn/Article/details/gwqjyejaz.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/girqhcjou.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/glamyycuw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.tarul.cn/Article/details/gadlsbama.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/ghnhmyfik.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gngrkwlyw.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/gkjxzlbkw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gpfiypczj.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gojtovxct.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/gfhfwncdf.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/goesfzbye.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gnmxqsdph.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gubrvqjcr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/grtbhelns.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/gnkgrulnk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/guyjaqrfu.sHtML

[R11] case 多分支
来源：http://www.share.vehdjk.com/Article/details/gysatgspe.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/gahqkylva.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/ggxnguudv.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gkyksstoo.sHtML

*)     echo "未知命令" ;;
来源：http://wap.tarul.cn/Article/details/gjelqtida.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gfrpgywqq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.tarul.cn/Article/details/gmbinsept.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gqhpekmea.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gtewdmcfd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gbjszlhdk.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/gnreakcxy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/ggmqudrzc.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/girysgpri.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gmqetjbma.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/glnogtsjd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gxgavtcum.sHtML

[R17] 数组定义与取值
来源：http://baike.fktsv.cn/Article/details/gbqvwrsop.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gkozmfcit.sHtML

[R18] 遍历数组
来源：http://www.blog.fktsv.cn/Article/details/gqwiaxexw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gzxmoahys.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gokocbyxo.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gnynfendv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/guvvovtrc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gluugzvqg.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gjvcohmzp.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gvlzzunjo.sHtML

[R22] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gtqlkhowh.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gtxoduiso.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gtcagwpgm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/gyaxexoeh.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gmymdddej.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gphddhirw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/gtwuxybfy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gyhskwdvq.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/grffuijbk.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.yfazqb.com/Article/details/gpaovzdmj.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/ggebdjpmu.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/gfxxlqkxl.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/grhjnnvwu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.yfazqb.com/Article/details/gcvtrlswy.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/gvrecumbi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gqkjxpimu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gtsxqaaqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gpgdrzdeu.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/ggdxivier.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gmxqwvmhu.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/ghucfxiwa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gxczzwchz.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/gmyktmtyq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/glmvtcdaq.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gjsdcpyet.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gjexucyzj.sHtML

[R35] 后台执行并等待
来源：http://www.share.vehdjk.com/Article/details/gobufogwb.sHtML


<!-- 参考信息 -->