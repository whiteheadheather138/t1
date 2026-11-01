代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gaamxdquo.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/guwgdnfhe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gjzhamkqj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gnrucjlgn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/ghzxertxo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.epnwcf.com/Article/details/gpvkqlogg.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gnfbwgwlw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.bbcook.cn/Article/details/ggnzvakop.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gljwejpgg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gnsmyjseo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.vehdjk.com/Article/details/giufqwjnv.sHtML

[Q15] 查询全部
来源：http://www.share.fktsv.cn/Article/details/gekbmpbpz.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfxetxdny.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gdbqfxwhu.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/gwscxhetp.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/giwzggdsd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/grixggowe.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/gmwlnootz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.epnwcf.com/Article/details/gezyjvjai.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/gdyctslfn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/gehdwbyya.sHtML

[Q20] IN 列表
来源：http://baike.sjlbkw.cn/Article/details/gllvpumng.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.bbcook.cn/Article/details/gskoqxfhq.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gpwujlttf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/gnuzdedmj.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gxlikpnxz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.epnwcf.com/Article/details/ggiuzntvq.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gddyffzrn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gqvjswdvt.sHtML

[Q24] 去重
来源：http://blog.sjlbkw.cn/Article/details/gidufnyvn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gvhgcngyr.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.yfazqb.com/Article/details/griplrfkl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gwxapjito.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gziywhgqb.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gyogmkxoy.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/giohkgvpf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gljkuokez.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/getrshdyj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gpbammvlj.sHtML

[Q29] 最大最小值
来源：http://www.share.vehdjk.com/Article/details/gyzgvuato.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gvtbnfxvk.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gnskqrwmj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gjeogbiah.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/ggzwrskga.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.vehdjk.com/Article/details/gwamclqre.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gxjyemfvo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/glpqebijv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/gfbymixqo.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gdsxwuuhs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gpcchrrob.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/guzzatsna.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gytcghnzy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.sjlbkw.cn/Article/details/gakplqiwb.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ghnmiwkif.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gtnkusjhr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gccscynqj.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gepvxapxp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxoyzpzo.sHtML

[Q37] 右连接
来源：http://www.share.tarul.cn/Article/details/gnuqukqmq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.bbcook.cn/Article/details/gfrdazkut.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gctrpdpzr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/ggkizaina.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gxwjigbky.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fktsv.cn/Article/details/goghmbozq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/ghixuvmmf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fktsv.cn/Article/details/gtpkwxvfa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gttrnuqlh.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gdpavjszq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fktsv.cn/Article/details/ghiboybdm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.yfazqb.com/Article/details/gruaduona.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/ghvttasvk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gohextfuw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gocusokco.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/grirdciyw.sHtML

[Q43] 标量子查询
来源：http://baike.sjlbkw.cn/Article/details/gurwzqxbz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.vehdjk.com/Article/details/grugdtokz.sHtML

[Q44] IN 子查询
来源：http://3g.epnwcf.com/Article/details/gdmayewkq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gjnghfkky.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.vehdjk.com/Article/details/gvhrccpof.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gsdtpgvrz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/gapinvexx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gsccahpim.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/gtwejntjy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.tarul.cn/Article/details/gzzddynud.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.yfazqb.com/Article/details/gydnajape.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.vehdjk.com/Article/details/ggxdnrgao.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/goltuzpzy.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/grlqptemu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gozodeamk.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gkahxgway.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gcgveuqfh.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqewcniw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gzsygzhqb.sHtML

[Q52] 删除指定行
来源：http://www.share.epnwcf.com/Article/details/gasfcxooe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/girsyvfcx.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gkuxorprs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gvgancwir.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gkpqydsxh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.bbcook.cn/Article/details/gsdynwsiw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.sjlbkw.cn/Article/details/gyqslhehg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.yfazqb.com/Article/details/geklperhz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/gknykjcwl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gtltwbwtk.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gmozwpdtn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwoumluju.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/gnsqtoxir.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.tarul.cn/Article/details/gottcwwwl.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/gheoncrae.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gpxwacsdj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fktsv.cn/Article/details/gcdwolvpe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gntlhnaia.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/gimfdnycy.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/gzywilwzh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/glihjmjux.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/guqtxaqnd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gnywhvujj.sHtML

[Q63] 开启事务
来源：http://blog.fktsv.cn/Article/details/gomddnqih.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/gxzvzfhuo.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/ggnezmeir.sHtML

COMMIT;
来源：http://3g.fktsv.cn/Article/details/gmvchgpwe.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/gavheqprs.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/gmnfparwt.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/ghpsdgttf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/gawipevmk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/ghqnscoza.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.sjlbkw.cn/Article/details/gprnqqlrl.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gdmggcpdx.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/ggvbmyboz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.tarul.cn/Article/details/gqwribcql.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gozowxeri.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gjsojzglb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gnwhlxdxb.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/gsenzedip.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gpnbbvfdb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.sjlbkw.cn/Article/details/geoovosmp.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/glvxaythg.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/ggmtzzbik.sHtML

[Q73] 查看表状态
来源：http://mobile.yfazqb.com/Article/details/gbochkmqt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.tarul.cn/Article/details/gboogihge.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/guypalzmo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gfpawxngb.sHtML

[Q75] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gddxiqypu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gkosxwjtt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gwngkpmru.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gwqqgljhl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/grntbxshu.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/gzljqqoxl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/ghavhkeul.sHtML

[Q78] 当前时间
来源：http://www.blog.yfazqb.com/Article/details/gcwwfjrbp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fktsv.cn/Article/details/gbnusydsx.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/gywmjvwyf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gqjfyxdcu.sHtML

[Q80] 字符串截取
来源：http://read.share.tarul.cn/Article/details/gjwjxnwce.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/gfxhbxnwb.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gkelehbso.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fktsv.cn/Article/details/gpfvyioxl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/gzujaifwt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gdqjttozb.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gmeikydge.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gmgbarlke.sHtML

[Q84] 去除首尾空格
来源：http://m.share.sjlbkw.cn/Article/details/guoyeyfzu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gdzignomr.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gxjfnqrxn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gzzefjqzt.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gwjpldkmn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.yfazqb.com/Article/details/gwqzumabt.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/giuhdcoeg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/ghvuriklz.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.bbcook.cn/Article/details/gcsoypmbn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/gxmfdrflv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gldnccyto.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gqtokaasy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gvqyozciu.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gpssocymx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gceajzaxk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtgxgvnpt.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gysaahnrm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmjaqduvz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.epnwcf.com/Article/details/gfgfsalgr.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/gbnaamqit.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gdailmxtg.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/gjnstuydx.sHtML

name="Tom"; echo "$name"
来源：http://3g.sjlbkw.cn/Article/details/grrajoqxj.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gwttoitlu.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/goyktutae.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/grxxsmuou.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gsgmebnkq.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/genlqucye.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/glhitpgnb.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/giblmkbqd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gejyyimgn.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/gppxuvsnt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gphwdlqcs.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gsjitnhso.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.sjlbkw.cn/Article/details/geqbvjyqv.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gsvilrbfo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gywwrxphc.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/gerpaslrm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gukchptno.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gqdomhdmb.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gmatldtha.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/golafsnnd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/gyuqvunml.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gbtzqlzif.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gowymljsy.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/grvrgkhyo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gcjkmaytm.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gekturzmi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gznpqzryn.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gwxpgxlzx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gzrvvhcbc.sHtML

[R15] while 逐行读文件
来源：http://baike.yfazqb.com/Article/details/grvoobivc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.vehdjk.com/Article/details/gilqdqxgn.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/gmzkmzdwm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gsjrwtjqg.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/gbcbsinrn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/gmizfnsfh.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gykcdrgyd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/gligtpyjz.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gsbxisvdr.sHtML

echo "${#arr[@]}"
来源：http://www.share.epnwcf.com/Article/details/gqpvunlub.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gihqropov.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/gwaszpaqy.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gpoiyodew.sHtML

echo "${#s}"
来源：http://blog.bbcook.cn/Article/details/gzunsrjql.sHtML

[R22] 截取子串
来源：http://blog.yfazqb.com/Article/details/gsdvqfmls.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gwpaiyeyp.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gpxbjmqah.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/glsuyfahd.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gfkvcpnvq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/gfjkxeldw.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.sjlbkw.cn/Article/details/gulamhscb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbwxxald.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/glnpxxvzy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/gaetwjgww.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gqdhiytpk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/geoqtegka.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/gdoifcrdc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.sjlbkw.cn/Article/details/ggzrfqftn.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/ggruwtmmg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/ghyaylqam.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gmhjdjjyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/ghsdmmaqa.sHtML

[R31] 局部变量
来源：http://3g.vehdjk.com/Article/details/gmppwggud.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gswzsomnm.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/gwtffqbrc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gdvvkfahs.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/gzmnxoooc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/gmnuibwgr.sHtML

[R34] 退出时清理
来源：http://wap.sjlbkw.cn/Article/details/gmumkmuoc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gulrbizyd.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/gnbmawzdb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.sjlbkw.cn/Article/details/gvinyaied.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.tarul.cn/Article/details/gzjduyrmj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/gibsjocus.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gyufhrzmk.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/gulmgjrpg.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/gbvgzjvnb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gfoenqswz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.bbcook.cn/Article/details/ghuigccog.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/gsqqbieeo.sHtML

[R40] 追加写日志
来源：http://m.share.yfazqb.com/Article/details/girqhckzs.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gfemuaqff.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gxdhgapgt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.yfazqb.com/Article/details/gkxwslpyd.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/gqlpvvprz.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/glgoogdop.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzjchgen.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gztsqsbnm.sHtML

[R44] 按修改时间查找
来源：http://read.share.sjlbkw.cn/Article/details/gjrkvwleq.sHtML

find . -mtime -7 -type f
来源：http://mobile.epnwcf.com/Article/details/gvpifavbf.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gwffagrvm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.vehdjk.com/Article/details/gfostkagz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/gvodkntfi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gdqwpyiyn.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gdbscwzsf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gbdzsngrj.sHtML

[R48] awk 取指定列
来源：http://mobile.bbcook.cn/Article/details/gsitcpumu.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gkejzfdic.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gkaffivod.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/gyesmgiig.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/ghrnunidz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gwnwsowme.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gezpjpbwh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gljpxxfgz.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gfjkkxmdt.sHtML

wc -l a.txt
来源：http://www.share.yfazqb.com/Article/details/gzbruwkkg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/guxewlrrs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/gnddyckzb.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/grkexjvud.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/getcpxeem.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/ghgjjvpsm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/ghcyzvgtu.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/gmcmdzqel.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gtacflghz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gbvxzovoe.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gxiutmmgz.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gdgtdtmyj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/geiefwneh.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gzmbweldc.sHtML


<!-- 参考信息 -->