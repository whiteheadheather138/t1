代发 wailian999

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gnksowkkj.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/gumbbgvfi.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gvdoarugk.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gbnncomoo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gssyztxtw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.epnwcf.com/Article/details/gquudbrop.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/geladqvma.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/gbkhlrdte.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gfhanfddw.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gfnouwmqu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/gkkcrqdze.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/gztcfgygr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/gsmqgauqg.sHtML

[Q22] 排序
来源：http://www.blog.epnwcf.com/Article/details/ghdcavcxg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/graloswla.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/glypdswgh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gvwtpiwhg.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/ghvjywvum.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gcoieztua.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gthuxzbmx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.vehdjk.com/Article/details/gehfvtlct.sHtML

[Q26] 计数
来源：http://baike.sjlbkw.cn/Article/details/glnwaelil.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.vehdjk.com/Article/details/gyrehxssc.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/ggobmopbp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/golkhoblr.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/gfilxsjwz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gstxmxelj.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gjrdhmnvw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gxbjswgck.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gjhaybycs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gyjldutwi.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/gmyqofjpo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.bbcook.cn/Article/details/gnonuhggl.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gudtzuaeo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gxlbowlpm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gehoeqkuf.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gmhbazfix.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.bbcook.cn/Article/details/gdiuymzfc.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/gsxchgwny.sHtML

SELECT * FROM (
来源：http://www.m.share.vehdjk.com/Article/details/gugsmrqdi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.bbcook.cn/Article/details/getllpdtn.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gdhszgjkv.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gkmmprxby.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gwxuviwig.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gkwziewwp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gubqyoqzs.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gvcqgywle.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.yfazqb.com/Article/details/glimbaslp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gulyxzdvk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/gtvnbnket.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.sjlbkw.cn/Article/details/gnubhiaid.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.tarul.cn/Article/details/gderyihyz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.vehdjk.com/Article/details/gyiwfrpgc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gjujgixyg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fktsv.cn/Article/details/gzlkwykyk.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gjikpqpdm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gbxdduqtc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gkwihgerr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.bbcook.cn/Article/details/gsvughfmi.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/gnyafntws.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/glrndrdeq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/gswtkiilz.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gbsnhvsbn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/gvkppzwbw.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gianchkqf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gubkmfuht.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/givimftac.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gtmqmilqu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gwrhjeuoj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/grcrcrwcb.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gjfqsqbeh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gxfthtkpz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/grruvlohr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gjqnmhfsv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gxmbbdskz.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/gufcqbdvo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gxzmcazjh.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gmrrnkgfh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/gzjogrmsr.sHtML

[Q51] 用子查询更新
来源：http://blog.fktsv.cn/Article/details/glzrzrrba.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.sjlbkw.cn/Article/details/gflojnthc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/grelxxztm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gzfvoxslw.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/gbclswtsy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/glrgxfnka.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/gmmyisusk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/gqedgohyt.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/gccutmlcc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gxiiomsbf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.yfazqb.com/Article/details/gatkhlmvr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.tarul.cn/Article/details/ghtwzxlio.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/gngeuymuz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.vehdjk.com/Article/details/gabvlajro.sHtML

[Q58] 累计求和
来源：http://read.share.tarul.cn/Article/details/gsqvawvso.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gvktrjhym.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gxoctlavu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gdzezfwwq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gmooydyze.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/gfubxsmgd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gdyonzrxs.sHtML

[Q61] 移动平均
来源：http://3g.fktsv.cn/Article/details/gzfbnhgxp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/ghhcvcnan.sHtML

[Q62] 分组占比
来源：http://3g.vehdjk.com/Article/details/gorpncrpb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gecfndetq.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/gmepqquzz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.yfazqb.com/Article/details/gtgqlmhpn.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/glpdvfnih.sHtML

COMMIT;
来源：http://3g.sjlbkw.cn/Article/details/grhhilswu.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/gkjpcnyrb.sHtML

ROLLBACK;
来源：http://wap.fktsv.cn/Article/details/gymuexzah.sHtML

[Q66] 行锁查询
来源：http://m.share.yfazqb.com/Article/details/gckgjxvtb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gjbbcwalm.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gbpkkwbpv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.sjlbkw.cn/Article/details/grcfjqlsm.sHtML

[Q68] 保存点
来源：http://read.share.yfazqb.com/Article/details/gyonjiczj.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gnksbwcwa.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gflavbajo.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gsjentmjm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.sjlbkw.cn/Article/details/gsaereouj.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/gqfpftlfs.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gqsbgmawz.sHtML

[Q71] 查看建表语句
来源：http://www.share.tarul.cn/Article/details/gcvagtzkb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fktsv.cn/Article/details/ginwfihfq.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/gwsbsxxic.sHtML

SHOW INDEX FROM users;
来源：http://read.share.yfazqb.com/Article/details/gboicnsxo.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gppeswbml.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/goyhqeggg.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gckzowapd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gnqkgxymq.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gphwtgzcb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.vehdjk.com/Article/details/gimianxul.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/gdxuauvnk.sHtML

[Q76] 按天统计
来源：http://read.share.sjlbkw.cn/Article/details/gknmozibc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.epnwcf.com/Article/details/grcqitpfq.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/gmukqjdeq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/grzdpkaph.sHtML

[Q78] 当前时间
来源：http://baike.vehdjk.com/Article/details/gmpqjlmgs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/guzonxbjr.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/ghrybgcro.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gbrozopin.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gondigvbx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.yfazqb.com/Article/details/gvblhkosz.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gymosgrae.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fktsv.cn/Article/details/gjhbfaobi.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gtzdhbwti.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gfvpbfdlb.sHtML

[Q83] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gknfazsxa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gknrvltcm.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/gvmjuvfqs.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gcryxsien.sHtML

[Q85] 数值取整
来源：http://www.share.vehdjk.com/Article/details/gtulybqgn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/gvoxiwuko.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gnzkucuqu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.bbcook.cn/Article/details/guxpiflpg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/gknalbqqy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.vehdjk.com/Article/details/gyyvwzqxz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gexjrvadv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.tarul.cn/Article/details/gemyqolhm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/glbmycthy.sHtML

[Q89] 判断表是否存在
来源：http://wap.yfazqb.com/Article/details/gwnclepti.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gezdpjrja.sHtML

[Q90] 生成序号列
来源：http://www.share.vehdjk.com/Article/details/gqunexzhb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/gzcqqkgfe.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjdqezgtl.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gjdfmomug.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtjcutwjz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gdpctvhaz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gzfhlumwu.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/gbkhsnqrh.sHtML

[R02] 变量赋值与使用
来源：http://3g.tarul.cn/Article/details/gpvdcodxh.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gkoslgfzt.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/grvlinskx.sHtML

readonly PI=3.14
来源：http://m.share.fktsv.cn/Article/details/guvdxaiot.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gxyrspoky.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/gyyitlskf.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gphacctfe.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/grvcjalnq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gnzxmygtu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gabqgqmgc.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/gxyyjavce.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/gcggkyfkg.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gcqwahhmo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gwiwdnwgk.sHtML

[R09] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/ggdqtsbga.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gryyhsxwh.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/gexiybmqt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gdvftdvur.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/ghasxoruu.sHtML

case "$1" in
来源：http://www.m.share.fktsv.cn/Article/details/gkcrpkviv.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/geddrlsgk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gzyhyoewc.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gblqnxwba.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gjjwejbfq.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gjvegzhvs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/gunsifqzq.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/ghtaedcrb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gsmykzdob.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/gucnnuiqh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gbacorbcs.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gpsqcanxz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.sjlbkw.cn/Article/details/gmvsnniet.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gflzzfqes.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gyealieau.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/glqbhwejo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.tarul.cn/Article/details/gkihuacqi.sHtML

[R18] 遍历数组
来源：http://m.share.yfazqb.com/Article/details/gzfskhvit.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gyfkeidjd.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gznpzubdf.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gtmsforyk.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/gtzzeyuvd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.sjlbkw.cn/Article/details/gabnzrkmx.sHtML

[R21] 字符串长度
来源：http://mobile.epnwcf.com/Article/details/gmqgpptch.sHtML

echo "${#s}"
来源：http://3g.bbcook.cn/Article/details/gvjpzykab.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/guqjguaed.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gbwtkjfln.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gmafmdvbo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gyofcrrui.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/goscdqhls.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gsuidftxw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gvxyjartf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.yfazqb.com/Article/details/gpqlzbjqp.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gijpyxwtv.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gyjjtvnsu.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gqstjltag.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gmcalitgu.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gvwgwjhne.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.epnwcf.com/Article/details/grpxogbxe.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gtysfuvty.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gxtbexxuz.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gkmhkstlf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.bbcook.cn/Article/details/gpxxtzqdu.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gruptxxkz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gsozypoto.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gbfqhowmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gbwqtlppq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gutbtostu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gwwvekkxa.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gdmwzifur.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gttcaziby.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gtnlcgkdy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/gazsxyzlq.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/gfmnrfbmu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.epnwcf.com/Article/details/gffqvsqrl.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gqvydohax.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/ghmxyjnum.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/gzubnecpq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gxnqaufbt.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/grovhxaoy.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/gyygwfcwc.sHtML

[R40] 追加写日志
来源：http://wap.yfazqb.com/Article/details/gbuxutvgq.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/gobagocoy.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/gatsexvoh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.yfazqb.com/Article/details/gzoqqpxqz.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gtwapjkdz.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gywuousgo.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gwpxqftyu.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/grizdflmu.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gevpfpavl.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gcqkewosf.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/grylqxyfl.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.bbcook.cn/Article/details/gzpekjhjo.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/gtnnvjfco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fktsv.cn/Article/details/gurepabex.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gqyjhtqsv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/gflpqqfcx.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/gkywqsgjx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gkplgnxtm.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/gqgmrmddu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gxmcosdre.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/gzkkcojte.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gsdzxxqyk.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gwotgllbu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gnhhwyrnu.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gnkvbkujt.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gpqxyfdxy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/ghfrocqib.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gyhuscbsk.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gvfatingu.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/gnvyipfmk.sHtML

[R55] 压缩与解压
来源：http://3g.bbcook.cn/Article/details/gcuibmyqq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmtibnhj.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/ggaqxctyt.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gywgefiuq.sHtML

[R57] 远程执行命令
来源：http://mobile.sjlbkw.cn/Article/details/gwkrbfomb.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gsijuizgv.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/grvyngpei.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.bbcook.cn/Article/details/guaqzskgd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gkuetlscr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gqlbtwgfn.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gxpkgjbsi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gvgcphapr.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/grumwykhb.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gacuqrmsn.sHtML

[R62] 找最占空间的文件
来源：http://read.share.epnwcf.com/Article/details/gwpgvmqmd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.vehdjk.com/Article/details/gymgpyvfl.sHtML

[R63] 内存与进程
来源：http://www.m.share.tarul.cn/Article/details/gcvztiqmx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/grewnrkll.sHtML

[R64] 结束进程
来源：http://www.blog.sjlbkw.cn/Article/details/gciiplnuy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gucluwqtw.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/ggukzmkhm.sHtML


<!-- 参考信息 -->