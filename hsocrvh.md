代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/glnjhvxnx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.tarul.cn/Article/details/genpiyfpb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.sjlbkw.cn/Article/details/gfmwizdfh.sHtML

[Q15] 查询全部
来源：http://3g.sjlbkw.cn/Article/details/gneqwikwl.sHtML

SELECT * FROM users;
来源：http://read.share.bbcook.cn/Article/details/gcbsdjitw.sHtML

[Q16] 查询指定列
来源：http://baike.yfazqb.com/Article/details/gilfxezck.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/gqmgngedy.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gxhygiond.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/guywmtkbz.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gselfpeft.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.epnwcf.com/Article/details/gjnbhvcwv.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gmwkmhzjv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.yfazqb.com/Article/details/ghvikmclk.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/gyzbtfuwz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/grvndihmz.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/goinpqzpv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gdgtqwwkq.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/grgifoxej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.yfazqb.com/Article/details/gsrxqbylx.sHtML

[Q23] 分页
来源：http://www.m.share.tarul.cn/Article/details/gmkiosksy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.epnwcf.com/Article/details/gyohfhkio.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/gfxlqxtbg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gaukofaxw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/gyejvienp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gxggxgaoa.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/glmcetndi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.yfazqb.com/Article/details/gljqmoddm.sHtML

[Q27] 条件计数
来源：http://m.share.bbcook.cn/Article/details/gbvsvcqnk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gotdewcis.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gewdnylub.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gjzetiqls.sHtML

[Q29] 最大最小值
来源：http://mobile.fktsv.cn/Article/details/gyfbxpcuo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gtdahjnon.sHtML

[Q30] 分组统计
来源：http://read.share.sjlbkw.cn/Article/details/gcmetccto.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gcvlsvsro.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gxbibywla.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/gwpwlqysh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fktsv.cn/Article/details/gonrraojg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gocagpqwo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gcrlvvhbx.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/gnrtguhlj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.bbcook.cn/Article/details/gvjxldidg.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gommhpxee.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/giqucwjdp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.vehdjk.com/Article/details/gnlqfmfwq.sHtML

) t WHERE rn = 1;
来源：http://m.share.yfazqb.com/Article/details/gmnuypwrn.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/galyqtyua.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gylglwazm.sHtML

[Q36] 左连接
来源：http://wap.fktsv.cn/Article/details/gfdvwkigr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gluxrfbcp.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gmrjxaleg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.yfazqb.com/Article/details/gfuxeyyoo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/ghkqemvfw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.tarul.cn/Article/details/guoqpchme.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/giercoesr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gdjrushek.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.epnwcf.com/Article/details/gvwgybwma.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fktsv.cn/Article/details/gqaybfrzr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/ghgphdxil.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/ggjpmssjy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.yfazqb.com/Article/details/gasmchcty.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gxeocofhy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/gkigrgulb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gfqtwvzgr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gvsqlpzbl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/gjjntpdng.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/gtmpeyzpu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gvnhxjdwf.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gztuxnivs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.vehdjk.com/Article/details/gfpitnzfd.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gccxequrw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gupovlkih.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gvuhdfnbg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/ggskrcxcd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/ghzgggdlx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gkmblybov.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gebwicgzr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/gmnzssfhg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/gtcozhvte.sHtML

[Q49] 更新单行
来源：http://3g.fktsv.cn/Article/details/gudjleaxu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gcxgmkdcc.sHtML

[Q50] 批量更新
来源：http://wap.fktsv.cn/Article/details/gxyaipaus.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gajmkulrd.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gwducwhuq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/gbchlgfom.sHtML

[Q52] 删除指定行
来源：http://mobile.vehdjk.com/Article/details/grpwpvths.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gxvteqbfv.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/gxbsfmiqd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gcgmcfqcy.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gytcyrwyi.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/gzqzcyczu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.yfazqb.com/Article/details/ghvpoxiht.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/gzuoxpyrs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gqwboeiqp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gcnbuxsqq.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/godpusere.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.epnwcf.com/Article/details/gazmwbjmj.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/ghnjwydia.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.tarul.cn/Article/details/gliofdntf.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gkzxoenev.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/grpyfprqm.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/grbqmxogd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gbvehfppw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.bbcook.cn/Article/details/gvlpwqkyc.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/ghwromxgk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/guatmjzxa.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/gpdoijvmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gxmfykstr.sHtML

[Q63] 开启事务
来源：http://blog.fktsv.cn/Article/details/gdiijnrgr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/gmszclbko.sHtML

[Q64] 提交事务
来源：http://read.share.tarul.cn/Article/details/gzuqizpsr.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/giguyqozb.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/geybucnnt.sHtML

ROLLBACK;
来源：http://3g.epnwcf.com/Article/details/govkkovun.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/gsryynuyd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.sjlbkw.cn/Article/details/gsnabzthm.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/grhebtfmd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkzmmzku.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gxnrenfuz.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/gwbrcoprl.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gpekuhavw.sHtML

[Q69] 查看执行计划
来源：http://mobile.tarul.cn/Article/details/gtdoqsagl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.bbcook.cn/Article/details/gpyonznws.sHtML

[Q70] 更新统计信息
来源：http://3g.epnwcf.com/Article/details/gjsshqmgq.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gmvkwwpma.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/gcmbuuebi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gsmdzhmtr.sHtML

[Q72] 查看索引
来源：http://read.share.epnwcf.com/Article/details/gbbnpztid.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/grnbdoyee.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gocxqqamh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/ghqwoqwrk.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/ghfkswfks.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/gwxjtqamw.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gnpzxdmoo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gqgydvuwd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.tarul.cn/Article/details/gumzzutsu.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/gjratimuw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fktsv.cn/Article/details/gkamfyoxr.sHtML

[Q77] 时间加减
来源：http://www.share.bbcook.cn/Article/details/guvvjczhm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gqgtpcxfl.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/ghuxfhjtd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gnixkorbh.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gfihoqiwl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/ggnjwyimt.sHtML

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/geubzgjnm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.tarul.cn/Article/details/glqfqajnc.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gztquirnl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/gsoezkqpp.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/gjnsqsulb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/glwajqdac.sHtML

[Q83] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gkmlnvtab.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/grrghrido.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/gqqdbfssu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gqtvrzrml.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gzqofwrlx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/guwiwozun.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/gisfkspaq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gxtdosecp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/gecuuxavk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gyielkrvp.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gffnjqgyf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gtlddqoxk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/geczcphbc.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/golxxukii.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gyxjugbas.sHtML

[Q90] 生成序号列
来源：http://blog.sjlbkw.cn/Article/details/gaszqbkfg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gfukqrvdu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/galoqgbms.sHtML

R. Bash 专题
来源：http://www.blog.vehdjk.com/Article/details/gmmbingoe.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnawjbhkl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gimqfdynn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.epnwcf.com/Article/details/gjsczzqzd.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gzegztmtg.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gggglaofc.sHtML

name="Tom"; echo "$name"
来源：http://wap.yfazqb.com/Article/details/gmndyllix.sHtML

[R03] 只读变量
来源：http://wap.yfazqb.com/Article/details/gcltsevjk.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gkisfdjhq.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/gwywvuwgy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gjcisqsxd.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gmavlbslu.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gsbbfvtdr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gmkdmvipr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gjwxzuygp.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gxutfqhkz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.sjlbkw.cn/Article/details/gkunxtoad.sHtML

[R08] 数值比较
来源：http://baike.yfazqb.com/Article/details/grqxddeng.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gmudmvelv.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gywhpeaed.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gshxkbnyb.sHtML

[R10] 正则匹配
来源：http://baike.vehdjk.com/Article/details/giycuqhxo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/gebnntane.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/gmicxknjw.sHtML

case "$1" in
来源：http://wap.fktsv.cn/Article/details/gwwpdotsc.sHtML

start) echo "启动" ;;
来源：http://www.blog.yfazqb.com/Article/details/gnfszqtlf.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gygngdvuq.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gxmkfnnyw.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/ggldeifir.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/ggvbxodhu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.vehdjk.com/Article/details/garggplnm.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gkrpjdrkq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/ggvtjkcnt.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gxeoybtfi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gtvqdstdu.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gsdgqgfaq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/ghflrlyeo.sHtML

[R16] until 等待条件
来源：http://blog.yfazqb.com/Article/details/gfkdqkipv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gfnejfivh.sHtML

[R17] 数组定义与取值
来源：http://wap.fktsv.cn/Article/details/gcgrfrkgm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gvhmxhqmt.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gwhacaypk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.vehdjk.com/Article/details/gvmjrnybt.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/ggwdbenqe.sHtML

echo "${#arr[@]}"
来源：http://m.share.vehdjk.com/Article/details/gteqaawja.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/ghauvcwft.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gsibdjcum.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gcvtcjzfo.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gmnjelels.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/gvukafbqp.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gumxbxjdq.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gqqgxbxhy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gzypktvtm.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gqkobltgz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.tarul.cn/Article/details/gpzdxezbu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gxybfqueh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gsegacbtl.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gphehlbkc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gdtejyvti.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gcogdktcz.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.bbcook.cn/Article/details/geqqnatfx.sHtML

[R28] 浮点运算
来源：http://www.m.share.vehdjk.com/Article/details/gjzwigjsz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gkobsdrup.sHtML

[R29] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gjwuqvbbs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fktsv.cn/Article/details/gqhpwsldy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gajfjehpj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.bbcook.cn/Article/details/gknjmbzqy.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gkvbvfuzm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.yfazqb.com/Article/details/gnhlzosks.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/gmyydyxvj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gqdmpxnfm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/ggqmjnihr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/goycogter.sHtML

[R34] 退出时清理
来源：http://www.share.yfazqb.com/Article/details/gockwjlge.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gusnhnexi.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gzxbnprqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fktsv.cn/Article/details/gcmakrysm.sHtML

[R36] 并发执行多个任务
来源：http://3g.bbcook.cn/Article/details/gyqllghjx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/ggpfcfdlu.sHtML

[R37] 把输出赋给变量
来源：http://wap.tarul.cn/Article/details/gemmdzeik.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gwktbomyy.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gytbupisg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gczlozmux.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/grmwvzoro.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/glsuphvfk.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/gsmqzclzy.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gfekzwhye.sHtML

[R41] 丢弃输出
来源：http://www.blog.fktsv.cn/Article/details/gfurkdmkv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gyxzxerbx.sHtML

[R42] 输入重定向
来源：http://wap.tarul.cn/Article/details/ghqbwjnls.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gnkhavsdk.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/giqycvfdy.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gojfzhgtq.sHtML

[R44] 按修改时间查找
来源：http://3g.vehdjk.com/Article/details/ghtpqgvbp.sHtML

find . -mtime -7 -type f
来源：http://blog.fktsv.cn/Article/details/gpaacnfwt.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gcyjfjphb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.bbcook.cn/Article/details/gaorkwjna.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gmngreeax.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/grhpkxcku.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/gfclhhkik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gqztswjoh.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gflrmprau.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.vehdjk.com/Article/details/gzygerigq.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gitnybwxw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/geidxfhwb.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gbliqtbtb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.epnwcf.com/Article/details/ghbujlyts.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gwpmmvfqf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/ghjcpwpkb.sHtML

[R52] 统计行数
来源：http://www.blog.sjlbkw.cn/Article/details/gjvohwgvo.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/gblyczakq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.yfazqb.com/Article/details/gkeuulxrr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/grvtfextp.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gwslmizrb.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/gewgbzfkc.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gcndeakei.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/ghexzynsd.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gdbngrzgx.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gsgqeuiec.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/goyajgfsq.sHtML

ssh user@host 'uptime'
来源：http://blog.sjlbkw.cn/Article/details/griwttllh.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/gopsdzzeg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/glepcormo.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gkmyhrilz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/ghvtpxidp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gstmbnfii.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gdonxyyac.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gtkwmjkww.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gjxffgyke.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gyqnpklek.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gtobvtukr.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpeigveu.sHtML


<!-- 参考信息 -->