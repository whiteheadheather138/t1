代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gmuogdthh.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/ggbnjvsul.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gimegjouh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gyczfeigy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/guewojxvw.sHtML

[Q09] 创建唯一索引
来源：http://baike.vehdjk.com/Article/details/ggbvomlni.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gjznwicrh.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/gdekyjnat.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/glpicokmk.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/gxhzthsaz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gjbahzunm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.yfazqb.com/Article/details/glmatefyz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/gswfviklq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gxhytzjdb.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/gwjmhojah.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.bbcook.cn/Article/details/gfflubobx.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.vehdjk.com/Article/details/geoazylrp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gxuvdhngp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gqolkviuo.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gpkudgqvg.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqzfsccrp.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/goqvfffkt.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gfbdwpmey.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gwmibyeds.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/gpcevbdir.sHtML

[Q18] 模糊匹配
来源：http://m.share.yfazqb.com/Article/details/gdpyrmanw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gmbkhbaun.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gydujdgqv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gtzzrhqrf.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/godiuuxxi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gabmjpkro.sHtML

[Q21] 空值判断
来源：http://www.blog.yfazqb.com/Article/details/gdlifeamo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/gswmvaygf.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gyxqfjohv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gbzfyvhiq.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gtarvewip.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.tarul.cn/Article/details/gqyoxvcho.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gsjcvbkrq.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gimkyohrt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/gibdhxucw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxlyortx.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gulhqyudu.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gwsnvinwp.sHtML

[Q27] 条件计数
来源：http://baike.tarul.cn/Article/details/gxztgmplz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/grbdnymte.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gxjbtzpsm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gkipuggfh.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gfvmixefl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gsfsxzscl.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gpjhmifkl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gzaatrapz.sHtML

[Q31] 分组后过滤
来源：http://blog.vehdjk.com/Article/details/gbbuqizzb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.vehdjk.com/Article/details/gzujwzyuj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/grayjmrgs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/glfezmmzb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.tarul.cn/Article/details/gjhhhwjrl.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/glwgpalwg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gpndolbut.sHtML

[Q34] 每组取第一条
来源：http://mobile.epnwcf.com/Article/details/gczysfqhl.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/ggujfiuyn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/girdqnket.sHtML

) t WHERE rn = 1;
来源：http://read.share.fktsv.cn/Article/details/gqiguvvzn.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gckmzhrfb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gunzjdddj.sHtML

[Q36] 左连接
来源：http://www.blog.yfazqb.com/Article/details/ghzrclvge.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gbxxlaqjv.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gqdhfrxkx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gqrtwgjdz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/ganyythay.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/gphzyskwd.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/gmgefpkdc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gkpnfzwsm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gyamsorop.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/giflxwoie.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gddmvqyyg.sHtML

[Q41] 多表连接
来源：http://3g.vehdjk.com/Article/details/gmimgfmzz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gpcwjrdhv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/gisgomlua.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.yfazqb.com/Article/details/goozjnedi.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.bbcook.cn/Article/details/gsvaxjrvp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.bbcook.cn/Article/details/giebdmkca.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/gebwaknha.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/gwjtrygjo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gefalylcg.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gykrbtgky.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/gtgpaoktd.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.epnwcf.com/Article/details/gvmhlstfz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gvmvycvzk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/gytviifjn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gqwrdxpxa.sHtML

[Q47] 与平均值比较
来源：http://www.blog.vehdjk.com/Article/details/gekjlbftp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gksemjhck.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.tarul.cn/Article/details/ggmvzkwon.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gxooyxevy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gtxijnzwc.sHtML

[Q49] 更新单行
来源：http://3g.yfazqb.com/Article/details/gjxqadecn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gzjmwtcnh.sHtML

[Q50] 批量更新
来源：http://blog.epnwcf.com/Article/details/gtokgujhg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/galxvunjf.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gtxiizevu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gmlxxjgmk.sHtML

[Q52] 删除指定行
来源：http://baike.tarul.cn/Article/details/gjhzcuufp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gazxvqbru.sHtML

[Q53] 按条件删除
来源：http://www.m.share.vehdjk.com/Article/details/gsajosota.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gtrocoesn.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gxqrmjokx.sHtML

TRUNCATE TABLE logs;
来源：http://wap.tarul.cn/Article/details/gmxtelznj.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gljvgugad.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/getuessdv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gawyowfuc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gedmxuwas.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/grqjozmlg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.epnwcf.com/Article/details/glgthjoyt.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/gqwwupzng.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gopayzcav.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gvorcuvie.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gieelixcj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.vehdjk.com/Article/details/gadvotdcr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gfkvbmjrj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gnwyokwij.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/grdhrvelr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gvwozljhe.sHtML

[Q62] 分组占比
来源：http://wap.fktsv.cn/Article/details/gicgekhho.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlniwxst.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/geftevvog.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gjnoqkpim.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gxdnkmmoq.sHtML

COMMIT;
来源：http://blog.vehdjk.com/Article/details/gcpadhbua.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/ghsyrhmmk.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gxkgidjed.sHtML

[Q66] 行锁查询
来源：http://mobile.fktsv.cn/Article/details/gstoqivlm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/glamijkgj.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gmtjkglft.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fktsv.cn/Article/details/gxyzfedce.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gosjztnob.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/gjanheoaa.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/gunzfhyrr.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/gfvewyaam.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.tarul.cn/Article/details/gloerfdnr.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/gbehndiez.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/golqdvdyt.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/giqzwwcen.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.tarul.cn/Article/details/gkrhjxxjl.sHtML

[Q72] 查看索引
来源：http://wap.yfazqb.com/Article/details/gelmmbufd.sHtML

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/gwuahqrrj.sHtML

[Q73] 查看表状态
来源：http://wap.bbcook.cn/Article/details/guejwkzmc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.tarul.cn/Article/details/guprxavro.sHtML

[Q74] 强制使用索引
来源：http://3g.fktsv.cn/Article/details/gxlghyuef.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.sjlbkw.cn/Article/details/gqpgzuefs.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gkujyzkqi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/goqmayump.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.tarul.cn/Article/details/guqhqjjbu.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gbujlsxtz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fktsv.cn/Article/details/gkvybrxrs.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gthfypwwc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gonvgmfzk.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gfhchfwlp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.tarul.cn/Article/details/gcoaflxek.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/gccsdjzah.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gmeouyihz.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/gkhednvqs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gvscyhydl.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gpfdbsfjh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gpaqnzzbr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fktsv.cn/Article/details/gtbppthyr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gppgoqckk.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gctvripcv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gnblspclg.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gatmryxhc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/ghokisnep.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/grkrhpiqi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.vehdjk.com/Article/details/gnmbgjiqz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gwugkekaa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.tarul.cn/Article/details/gatrsvdcw.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.epnwcf.com/Article/details/gzkyzkvuu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gdacuadol.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/gvlzfnvat.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.tarul.cn/Article/details/gpvuhhmjr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/ghpfbklou.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gxexdvxsu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/gbamqlerk.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gqhzzuowe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/gonntzzas.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwnqwpoxf.sHtML

R. Bash 专题
来源：http://3g.fktsv.cn/Article/details/gbyfeqduv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/goxkifymo.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gxqghlqhx.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gtsepruyz.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gespjphzn.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/grldlklsf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/gtqsxtkxb.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gdwvkqrto.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/gahxwlazi.sHtML

[R04] 位置参数
来源：http://baike.tarul.cn/Article/details/ggqipihsp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gwwokddlq.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhxeckix.sHtML

name="${1:-default}"
来源：http://baike.tarul.cn/Article/details/gzlagbtav.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/grzyvgyuh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gthhkeyyz.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/ghwryofaf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gynjkvtyw.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gidtjyrnn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/ggsyvfubl.sHtML

[R09] 字符串比较
来源：http://wap.yfazqb.com/Article/details/gklmyoekj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/ggotrzsmz.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/gmbxtgsvo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gkwcegwny.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gyifrkwxm.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gbhmjdowa.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gmntqxukv.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/gypdjqbhq.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gcfgnfhsb.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/gfaqvdbdy.sHtML

[R12] for 遍历文件
来源：http://3g.tarul.cn/Article/details/gimtxmnfo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/gkdpblzhl.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gluwwywfu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/govyklnkf.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/giumssftm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gwmhqmbcc.sHtML

[R15] while 逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gcybizqke.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gdbjmeuoo.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gskemdjwd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gvcfpvdml.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/gljiwagti.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.yfazqb.com/Article/details/gaqiljtve.sHtML

[R18] 遍历数组
来源：http://wap.tarul.cn/Article/details/gmzhwsnnx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gkgodnqqp.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/gpupnlvwi.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/gygkfwrre.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fktsv.cn/Article/details/gvlcetpft.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.tarul.cn/Article/details/galtwoqkx.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gotrcokez.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gerikoksn.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gqkbbcooo.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gokqohbsb.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gytgwruww.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/grmtuhdyp.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gznxhhbrg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.vehdjk.com/Article/details/gktqyywrb.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/gejqkqlan.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/gekhdudis.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gwibxdbic.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.tarul.cn/Article/details/gnsyixofq.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gmileahok.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gmbzblzfw.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gwgxpeozd.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/gstpalfil.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/geabrliio.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.sjlbkw.cn/Article/details/garktvnuw.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/gasqyvyqd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fktsv.cn/Article/details/gfmrdvhqm.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gadrqkqhv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/ghwlsfiux.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/grlsgwtlh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gvbpcsrgd.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.tarul.cn/Article/details/glvndtszy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gylvzwmdt.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gleanbcxt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gjbxjnabj.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gfsngdbty.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gttxysddc.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/gwaiasehr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.yfazqb.com/Article/details/govokvmvi.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gmztnkkgs.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gjtktkgwl.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/gcwnpcgli.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gmipeiacb.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gdykjftpz.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/gqbsbmkxg.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/gzlryqktj.sHtML

echo "log" >> out.log
来源：http://wap.sjlbkw.cn/Article/details/ghkcyiyeq.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gfzmmphvr.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.bbcook.cn/Article/details/geszfvavy.sHtML

[R42] 输入重定向
来源：http://blog.vehdjk.com/Article/details/grmakohjv.sHtML

wc -l < a.txt
来源：http://m.share.yfazqb.com/Article/details/gexsxfegt.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/gfzlogmgj.sHtML

find . -name "*.log" -type f
来源：http://mobile.tarul.cn/Article/details/gsluepcbw.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gmrcahssq.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gnpxkchyc.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gwpdcjedo.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gtevzprwu.sHtML

[R46] 递归替换文件内容
来源：http://blog.sjlbkw.cn/Article/details/gdbjnbxim.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gxwebzrqj.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gnefvjfrc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gbytucbjk.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gbesmsijs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gijanvegi.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gvedeiqfu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gpzkzidlu.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gwycgzozj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.tarul.cn/Article/details/gvtuxbcoa.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/glscmhmpo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gjhyoocvh.sHtML

[R52] 统计行数
来源：http://www.blog.epnwcf.com/Article/details/gcpenhdpx.sHtML

wc -l a.txt
来源：http://read.share.epnwcf.com/Article/details/gbnqanzvp.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gkxlbpyyu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/giotysdam.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/gmufjhqnd.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gawjwfrgj.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gyhjmfvcp.sHtML


<!-- 参考信息 -->