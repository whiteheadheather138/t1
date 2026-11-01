代发 wailian999

SELECT * FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gscbeukgp.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/gzroxqurw.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ghmpqglae.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/gwccqcfwp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/gcqjjpsbm.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/gpqhibymn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.epnwcf.com/Article/details/grouialwq.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/gixiwyhzs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.epnwcf.com/Article/details/gpltuqgnn.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/gholxhkvg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gkyjccpmn.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/glrzvwftw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gixsbwpei.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/gfoorjkzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gdoowybch.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/gxvwhvmci.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/gimzuvtvw.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gbwvcetbv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/grwoptcsc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gcbjbeyko.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gqijcmuik.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/gsbfuumom.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/ghybpbgih.sHtML

[Q27] 条件计数
来源：http://baike.bbcook.cn/Article/details/gpbfkzjbt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/ggrsjbqie.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/gteditajv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gsapgtpfz.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gmtmksswr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gpxuzsajo.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gdzfznfsl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gdzaodadg.sHtML

[Q31] 分组后过滤
来源：http://read.share.bbcook.cn/Article/details/gscqnouit.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fktsv.cn/Article/details/gkmvkxmye.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/ggcblbsab.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gpnlsjbwz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.yfazqb.com/Article/details/ghabprhek.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gkmohfvcc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gqziqjwww.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/geysylabm.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gcwvslqwf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.yfazqb.com/Article/details/grduhbgbv.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/gmgfrnwup.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/gfmiefcif.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gdnhobfqr.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gruzyiguv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/geyhyglem.sHtML

[Q37] 右连接
来源：http://www.share.vehdjk.com/Article/details/ggigbabyx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/galwofgxp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gqpbdqhbe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gxqdomhkq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/gnbqhqwcf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gvldknxnl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/gzqwcdcvn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/gevkkmgcj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fktsv.cn/Article/details/grdkoyxsh.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/guacrpjob.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gpcebwfwt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gdkcunbta.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.vehdjk.com/Article/details/gaikdjrnw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/geocjvbsg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/geblvzjlp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gbeayjnsh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gscbsnqio.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/guljmluue.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gzrsksjsx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/ghizqogxe.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.vehdjk.com/Article/details/gikkuxuva.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gcfglncqf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gwayhdjzk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/goauszrbn.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/gjqllcsao.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/gvvslvugy.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/gwtkkiino.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/ghpxhkkhc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.epnwcf.com/Article/details/gneuifzzi.sHtML

[Q49] 更新单行
来源：http://mobile.vehdjk.com/Article/details/gdibfkvjl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gotgpdgii.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gvqzjewwg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gimxldgmb.sHtML

[Q51] 用子查询更新
来源：http://www.share.sjlbkw.cn/Article/details/gdwkaytwx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.bbcook.cn/Article/details/gkyagdpxt.sHtML

[Q52] 删除指定行
来源：http://wap.vehdjk.com/Article/details/gaihzehdx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gwjzhabov.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/gvhcwahjt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/gejkxhxgy.sHtML

[Q54] 清空表
来源：http://read.share.epnwcf.com/Article/details/ghnvklnik.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwyvhffn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gztsyvyyi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gdpbwfmiq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.tarul.cn/Article/details/gykvehnct.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/guanjfccj.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gqtbocyfq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gkjxagvjh.sHtML

[Q58] 累计求和
来源：http://wap.bbcook.cn/Article/details/gibofgprf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gejehdsti.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/grtmrclnz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gxudguody.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.vehdjk.com/Article/details/gqaqmafsw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/gjxoczqdy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/grcxhrggp.sHtML

[Q61] 移动平均
来源：http://baike.epnwcf.com/Article/details/gbnfzfgtv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gfkvvnvur.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gexgofbnh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gpgoqrrks.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/gjgyndcov.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gjqxxwpnh.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gemcprrdl.sHtML

COMMIT;
来源：http://www.blog.yfazqb.com/Article/details/guulrsdds.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gnsfgskdn.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gngyhhjjb.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gxbovncbo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/ganbiynso.sHtML

[Q67] 设置隔离级别
来源：http://baike.fktsv.cn/Article/details/gzybkpizq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/glfrwzfte.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gywgqkbjh.sHtML

SAVEPOINT sp1;
来源：http://mobile.bbcook.cn/Article/details/gqoimpkvy.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/grznjlsbm.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/gispqblmm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/govcbywwm.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gkewsxzzf.sHtML

ANALYZE TABLE users;
来源：http://3g.sjlbkw.cn/Article/details/gsuansbda.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gzvvsnhvu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gktssplow.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/gocbvwqlc.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gpvihghvt.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/gtfsfiizu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.bbcook.cn/Article/details/ggwimgktt.sHtML

[Q74] 强制使用索引
来源：http://wap.fktsv.cn/Article/details/ghyzykwzv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gdptngmsz.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gpmbxeany.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/guwxzevty.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gurvtsvcg.sHtML

[Q76] 按天统计
来源：http://mobile.bbcook.cn/Article/details/glfuevzki.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gtonqxydi.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gibfgzkwx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.bbcook.cn/Article/details/gsqbwwsoy.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gejqwnbnz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gsvpgbvau.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/ghbfukibx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.vehdjk.com/Article/details/gbteefkcy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/gsekqkhmx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/ggznhifjz.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gbyfhozij.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gqpnqlliz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.vehdjk.com/Article/details/gndfmyvav.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/goapaqcov.sHtML

[Q83] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gyofzepsg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gtcwkzbhk.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.bbcook.cn/Article/details/ghqlvwxot.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gtlevtoic.sHtML

[Q85] 数值取整
来源：http://www.blog.vehdjk.com/Article/details/gnqnofwzk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gyqgigxix.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.bbcook.cn/Article/details/gskiwhlxi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/gpjmxyonm.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/gznytgzfq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.sjlbkw.cn/Article/details/gwvybbbiu.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/ggwiwiwoh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gbdfnkdbn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gjjujregu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/ghybawgmc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/gfljyuxst.sHtML

[Q90] 生成序号列
来源：http://wap.yfazqb.com/Article/details/gpduybykz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/geuzotoda.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glolpufdl.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/gfkhttoxg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnewtnixf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/ggegxthlv.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gphnqzfqr.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gbywarniy.sHtML

[R02] 变量赋值与使用
来源：http://wap.yfazqb.com/Article/details/gtjwgqcbm.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gvaexixdv.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/gmqsyerxz.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/gwxsgsxmh.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gmhiyyaut.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fktsv.cn/Article/details/ggbtbvzjx.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gbswycboz.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gcprbmzze.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gxxrcubqz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gorrerojj.sHtML

[R07] if 判断文件
来源：http://www.m.share.tarul.cn/Article/details/gfehihmia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.yfazqb.com/Article/details/ggjihdqwt.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gsfcydxto.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gnqitzliq.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gxkyfgcci.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/grhebzxvk.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/grozhmryv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gjazefery.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gchkzjnii.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/grodftroo.sHtML

start) echo "启动" ;;
来源：http://mobile.epnwcf.com/Article/details/gryaxacty.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/govpdclcb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gulfdrfyf.sHtML

esac
来源：http://3g.bbcook.cn/Article/details/gmjrfvqqr.sHtML

[R12] for 遍历文件
来源：http://read.share.sjlbkw.cn/Article/details/gvgejldby.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gopuedquu.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gkpfbwkzg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gxxmfsbcv.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gapgbohxj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gftpfwmpu.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gskqpxadh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/gairchdjq.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/gfbokgruy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gmtemwmls.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.epnwcf.com/Article/details/gptftvcnq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/gdeaeqfbm.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gjyssmjwq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.sjlbkw.cn/Article/details/gzodyraks.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/grprzlasa.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/gftsdcpwx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gkmrllbln.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gztcsxflu.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/gmsettioe.sHtML

echo "${#s}"
来源：http://www.m.share.yfazqb.com/Article/details/gqwxopgrp.sHtML

[R22] 截取子串
来源：http://wap.fktsv.cn/Article/details/gaeduzpyh.sHtML

echo "${s:0:5}"
来源：http://wap.vehdjk.com/Article/details/gndolhwus.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gouzfldzu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gfxldrmez.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gvlaqfbxi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/ganwaygzg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/gfmrglktx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/guxhvpflc.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gnjpqmxun.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/grdxnpzhu.sHtML

[R27] 算术展开
来源：http://blog.tarul.cn/Article/details/ggamsafng.sHtML

echo $((1 + 2 * 3))
来源：http://3g.vehdjk.com/Article/details/gobcdgvly.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gitmuyyig.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/gdhaychrj.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/gqqalyipg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/gixahnyry.sHtML

[R30] 函数返回状态码
来源：http://baike.sjlbkw.cn/Article/details/ggbfzowjs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/glnngpisl.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/guteeudut.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/gcoqrriyz.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/gqhhuaioo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gkfhyrapu.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.yfazqb.com/Article/details/gyvrmkdgj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gkgdttfci.sHtML

[R34] 退出时清理
来源：http://m.share.yfazqb.com/Article/details/gotarhonv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/grodyxdqc.sHtML

[R35] 后台执行并等待
来源：http://blog.yfazqb.com/Article/details/gvxglldoi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/ggaddbmhi.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gipgphntr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gjexclxiq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/gyrxzthan.sHtML

files=$(ls -1)
来源：http://read.share.sjlbkw.cn/Article/details/gpmmvksgt.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gnklihsnt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/gsfekihci.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gvexrhbjo.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gphrqfwvp.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gmisyofem.sHtML

echo "log" >> out.log
来源：http://baike.fktsv.cn/Article/details/gwaetytvr.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gnaancusp.sHtML

cmd >/dev/null 2>&1
来源：http://blog.epnwcf.com/Article/details/gzrrpucoo.sHtML

[R42] 输入重定向
来源：http://m.share.epnwcf.com/Article/details/gdntqrijj.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/gybprwmhn.sHtML

[R43] 按名字查找文件
来源：http://wap.sjlbkw.cn/Article/details/gwgdeovbp.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/gkiknjzle.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/geixiiabm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gzvkkwbsa.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/ggikbpggh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/gfintgrmf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gvbnrdlqd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/gydgvtflo.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/gxewvkwwo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/gdsnsepcm.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gesdhxkim.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gpqdyziad.sHtML

[R49] awk 带条件
来源：http://mobile.vehdjk.com/Article/details/gatfhlppx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/goggqcsoa.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/geizzymzd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/gmeulxcpg.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gusdvxnwm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/glmxrgvgt.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gqxdaoejm.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gmcaromtj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/glqbylrwu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/gfbtvpicn.sHtML

[R54] 比较两个文件
来源：http://m.share.bbcook.cn/Article/details/gptcvxiql.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/grhpljmkj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gajttutmj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gfyuhpdmu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/goebpoyhb.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gsuurpscr.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/gtdeqwjxo.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gdafehnno.sHtML

[R58] 下载文件
来源：http://m.share.sjlbkw.cn/Article/details/gajnkyhve.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.vehdjk.com/Article/details/gmktogvid.sHtML

[R59] 发 POST JSON
来源：http://wap.fktsv.cn/Article/details/gqudinckb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gptpywgtt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gprgmbosm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gsidcfgef.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/gopctoqes.sHtML

df -h;  du -sh *
来源：http://www.blog.fktsv.cn/Article/details/gxcoqrnhp.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gnmabmhoe.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/gchzxwitb.sHtML

[R63] 内存与进程
来源：http://read.share.epnwcf.com/Article/details/gmklgkdpj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.bbcook.cn/Article/details/ghoaskskb.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/guqsziztq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gdwdjjprr.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/grnssimzz.sHtML


<!-- 参考信息 -->