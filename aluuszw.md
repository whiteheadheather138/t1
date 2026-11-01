代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/ghopoghfw.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/ghbogmkzp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gnnjbulcv.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gjtrsfrih.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.tarul.cn/Article/details/gcxegyfhz.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/givzfudws.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gwpgajgms.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/glftzztqq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.epnwcf.com/Article/details/grsbfdhsu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gqqynjrps.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gusudhfvt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/gwptslkxe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.bbcook.cn/Article/details/gmrkcvvxf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/ghdbxchtg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gjolekyqw.sHtML

[P08] 处理浮点精度问题
来源：http://3g.vehdjk.com/Article/details/gjunxhksw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.epnwcf.com/Article/details/gpvsbqyno.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.bbcook.cn/Article/details/ggckmffrt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gcvwyzldv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gsmfkgahh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gssjonwte.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.epnwcf.com/Article/details/gcjycnlek.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.bbcook.cn/Article/details/gskclrgfb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/glbzwzjxb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdbrzajvm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/gisqcojod.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxsrrzorg.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gtsulwojc.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gflfhqgnx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/ggxfkrwpb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/giwjqfbhy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.yfazqb.com/Article/details/gqkrnzhtr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.vehdjk.com/Article/details/gzchlpwge.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gtbnjzcak.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fktsv.cn/Article/details/gswozxumj.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsbcorub.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gdhgvnwqs.sHtML

user_id INT NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gkyqgqpjs.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.bbcook.cn/Article/details/gxpistcjv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gfseikivc.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gnzgmttpp.sHtML

[Q03] 增加列
来源：http://www.m.share.sjlbkw.cn/Article/details/gynjrgntx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.bbcook.cn/Article/details/gqhicsurc.sHtML

[Q04] 修改列类型
来源：http://mobile.fktsv.cn/Article/details/gmnasrulu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/gdzctpecz.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gfktqewkr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/gdhhzsoud.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gocezffxr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gtkdttwvr.sHtML

[Q07] 删除表
来源：http://blog.tarul.cn/Article/details/gwblnqhqh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gwhvrsabi.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/gpeuhqlez.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gmtvflrkq.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnkvktld.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/grzzcsqwf.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gbwbvecnh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/genkigndl.sHtML

[Q11] 一次插入多行
来源：http://www.share.bbcook.cn/Article/details/gvkbwkxms.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.bbcook.cn/Article/details/ggqfvflct.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.vehdjk.com/Article/details/gdwqfjucq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gbwfcvfst.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.tarul.cn/Article/details/gjndzmolr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gkgeqpoez.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.bbcook.cn/Article/details/gccfmvpdg.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/gwicemskk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gmmwgwnmx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gchdowvti.sHtML

[Q15] 查询全部
来源：http://blog.epnwcf.com/Article/details/gxuyiwues.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gmlzxtiws.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/gnurmgobt.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/gxqfklqhm.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gouuogzbg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gwpwffakp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gcroumkeb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.sjlbkw.cn/Article/details/gnorukecs.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gpmupdcvh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/guieciini.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/gtppibrqp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/givapvygh.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/gsjhxtkbl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/geoqiixbx.sHtML

[Q22] 排序
来源：http://m.share.sjlbkw.cn/Article/details/glumakdtx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gzddtodvz.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gultujnjf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/gftaxjdsx.sHtML

[Q24] 去重
来源：http://3g.tarul.cn/Article/details/guubncuzy.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gbqexcloq.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/ggzhlsrtm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fktsv.cn/Article/details/gbvbqbkks.sHtML

[Q26] 计数
来源：http://www.m.share.tarul.cn/Article/details/gqqefjbdp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/glgcsrgut.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gaxztvdco.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gleenouzu.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gmchbwytq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gsjwxbacn.sHtML

[Q29] 最大最小值
来源：http://m.share.yfazqb.com/Article/details/ghzsubnbp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gxivsnvay.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/grczgzedr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gwfibguxh.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/gugdrtmzg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/gfzpygsri.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gbqeuzryv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gxdtqfutw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gdseubwlj.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/ggtkkwykj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.epnwcf.com/Article/details/grhupbwmp.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/gcfdhactn.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gdtpissfu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/gxitjjkii.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gxkiuhlev.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gnulcmrqy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gtttviyuw.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gugjucqpe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gjgrqvljg.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gaxbsulnk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gokyfuvmi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/ggezyvldc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gcazulwhk.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gmadjwgsr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gkdhbypzt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gnnmbbxpa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.bbcook.cn/Article/details/gzucqhkjq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gaxbwteym.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gkpxkfkrd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/gwjaayajh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.yfazqb.com/Article/details/gizsywnxd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gayjtbjfk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gtwvcchnj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/ggnhyxtbq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.epnwcf.com/Article/details/gqzaigpba.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gpegnjngj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgvfpvow.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gkyzcwyki.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/guwexfnur.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/gqehpcqgw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gxrcshayn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/gljzlkict.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gubkbprfs.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/ggprxoyiv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gaakxdmti.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gdcfcnoar.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.tarul.cn/Article/details/gnktckvwm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.yfazqb.com/Article/details/gpjoiscpj.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gcbpodjlk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/ghqleoqgf.sHtML

[Q50] 批量更新
来源：http://www.share.vehdjk.com/Article/details/gnqauxzpq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gmracaxzf.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gyafimnbp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.yfazqb.com/Article/details/gyspawzis.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/ggnfdhgjm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/ghqhbxiwz.sHtML

[Q53] 按条件删除
来源：http://m.share.yfazqb.com/Article/details/gewilrfrh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/ggggvipys.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gsdyoaded.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/goxzbwoir.sHtML

[Q55] 排名（并列占位）
来源：http://blog.epnwcf.com/Article/details/glzisgags.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gtwwnspez.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.bbcook.cn/Article/details/gxkplnoma.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gjcwljgvy.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/gjjmstwqv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gntsmttup.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/glqpdbcch.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/grkskwwdk.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gxdclkknp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gvteqkjht.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gkqtgwreu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fktsv.cn/Article/details/gybplumvt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/gabckopuv.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gsroxjskw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gvrzotirz.sHtML

[Q62] 分组占比
来源：http://read.share.sjlbkw.cn/Article/details/gnpvcxmda.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gxojezyqm.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gosbjzhnt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gzowqychj.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/guejsxvma.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/gdixfomft.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/ggdkesals.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gvkgemdrc.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gusfrgurn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/gjkfsstkc.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gotyfdtyf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gzsqxpuph.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gdhvuylbt.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gblxmhwfe.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gzkajsivl.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gnwcrxdoy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.bbcook.cn/Article/details/gxhqhalid.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/gfxzignuj.sHtML

ANALYZE TABLE users;
来源：http://blog.sjlbkw.cn/Article/details/gdgvqatpx.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/gffttgwbr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.sjlbkw.cn/Article/details/gqimrrcpb.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gugmidnrx.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/goagppubm.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/gxaidzlgn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/ghgbbacbw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gsnnnveji.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/gmoflrmnb.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gdmqngkho.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.tarul.cn/Article/details/gvgyvecqr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/gvfhbhloh.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/ghsmicswm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gewcfkyrs.sHtML

[Q77] 时间加减
来源：http://3g.sjlbkw.cn/Article/details/gmmrpukdv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gfpzwnfzj.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gknygutgy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpbtxwuy.sHtML

[Q79] 字符串拼接
来源：http://blog.epnwcf.com/Article/details/gxktivxlp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.vehdjk.com/Article/details/gwhnamurc.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/ggjnndxyd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/gtlqqcdos.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gloavhfpp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gafzihivd.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gjamrmyef.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/grrsmybtm.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/grxarxiag.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gdysmdfjn.sHtML

[Q84] 去除首尾空格
来源：http://blog.yfazqb.com/Article/details/glbwzxeoo.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gpppzpqjp.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gyfiyfsgv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gpndcheci.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.epnwcf.com/Article/details/gneyhzawl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gxcoqizcp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/grlzhbpyy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/gtxiojbok.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gebarymdw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/gmjbgaktc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/guxufbedt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gjdzteked.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gqgncvbxm.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/gwitymnqx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/gsbjwswag.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/guutqcaya.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gnkwbjqxl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gprilvkay.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/gujlbboxu.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/gybdxzcat.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/ghmdpkdik.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gvitkwxst.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/guatmusji.sHtML

[R03] 只读变量
来源：http://www.m.share.sjlbkw.cn/Article/details/giefcvawo.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gcatbpolz.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gpbmuppqn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fktsv.cn/Article/details/gnbultzki.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/glgpfejrn.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/gjxogkowu.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gswwrmwex.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/glyvnuzdv.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/guukrtqaq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fktsv.cn/Article/details/gavjaxymt.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/grppozcdu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.yfazqb.com/Article/details/gqmfugwbm.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gxukoatml.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gbzoyytnt.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gqexwjahu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gkwkrjlkl.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gvkjyiwxy.sHtML

case "$1" in
来源：http://www.m.share.vehdjk.com/Article/details/gghyapisd.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/gkcvnaokq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gjbcdiljs.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gpdlvhtoz.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/gytxjjghm.sHtML

[R12] for 遍历文件
来源：http://www.blog.vehdjk.com/Article/details/gqhmasumo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gdqsdxxbt.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gbzyxbsdk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gkatxfadh.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/geajksnwf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gxauqlbvi.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/guvjhfzkf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gfvjqvyfb.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gupfxgenb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/ghdcekxkc.sHtML

[R17] 数组定义与取值
来源：http://m.share.sjlbkw.cn/Article/details/geilqlvwp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gkyuzynfm.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gpwfcnhbw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gnkkdyumy.sHtML

[R19] 数组长度
来源：http://baike.yfazqb.com/Article/details/gxauovrft.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/gphccsolw.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gatsooewi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gvwdpldof.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gzqqezhtn.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/giykmotkc.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gxwarqjau.sHtML

echo "${s:0:5}"
来源：http://www.share.epnwcf.com/Article/details/gefhqvzvw.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/geeortgag.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/gurpbvotn.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/ghssvhglx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gmyeimpna.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/grxmgdmmt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/glusijrpz.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/gzrotdfqi.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gwjbszzxp.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/gswkkhuda.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gordwvdsb.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gcoizczqo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/grbzjlhik.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gcnudgpeq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.bbcook.cn/Article/details/gzutdbchb.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gqugghfuu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/ghocmccaz.sHtML

[R31] 局部变量
来源：http://www.share.tarul.cn/Article/details/gwiugybop.sHtML


<!-- 参考信息 -->