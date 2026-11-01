代发 wailian999

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gzicghrha.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gyqkhymfs.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/gebchgigs.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/glvnhdhzk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/giykoppsc.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/ghcrmsaqk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gbottbqsy.sHtML

[Q19] 范围查询
来源：http://www.m.share.bbcook.cn/Article/details/gkxgaqssq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.tarul.cn/Article/details/gvfwixcsr.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gusymwmvb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/gicyluqog.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gmfirotsi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/gbpgvyxbb.sHtML

[Q22] 排序
来源：http://baike.yfazqb.com/Article/details/gwdqeibvq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/geuyhxakh.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/geonujcdk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.epnwcf.com/Article/details/glxjqbabz.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gpznxvzhv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gdfqbneyf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/goathasgi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gcvxysuxy.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/gsxffiiem.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gfqfininb.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gggaypvgx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gadbnlhfl.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/gxzwumcdw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gzkzlhfho.sHtML

[Q29] 最大最小值
来源：http://www.m.share.tarul.cn/Article/details/guglxgkaw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gajidjyby.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/glbcuhlgv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/giddjnubs.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gyixcdchr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.vehdjk.com/Article/details/gecyuywdr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gbrgwjvxa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gkshmkgmr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/ggrvdymjp.sHtML

[Q33] 多列分组
来源：http://www.blog.bbcook.cn/Article/details/gjprikboc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/ghraotdsc.sHtML

[Q34] 每组取第一条
来源：http://mobile.vehdjk.com/Article/details/guwnuijle.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gefpnpcfs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/groamqunm.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/gejhyysgv.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gwnqrcxme.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gcbjbaefu.sHtML

[Q36] 左连接
来源：http://www.share.yfazqb.com/Article/details/gfkbzacmt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gsxfsyilp.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gfutyrakg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/gchjtaody.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gyaayrknz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gqlslpzvy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/gtnjzsrwt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.epnwcf.com/Article/details/gptlkjcps.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/giauaicwe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fktsv.cn/Article/details/grdxqvhnt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fktsv.cn/Article/details/gxggmnfdq.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/govqjekwh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gcpfatcco.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gempgprxc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gwegajqrg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fktsv.cn/Article/details/gfzmqoigm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gehsiaslf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.bbcook.cn/Article/details/gnhhfaxdu.sHtML

[Q43] 标量子查询
来源：http://read.share.vehdjk.com/Article/details/gkaksfahk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/goescyenj.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gwnmfonfs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/gryysxpxu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/guuvlgded.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gpnmkezxj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gyahurlcw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gfjrqoopc.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gnilibphi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gbkzwksuz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gjovlknee.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gpcunkffa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gckmywbub.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/gqzhgusde.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gszrvgulx.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gynuxntzq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/gmenapqth.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gtqxwwdpx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gjphtxrhd.sHtML

[Q52] 删除指定行
来源：http://mobile.yfazqb.com/Article/details/gidjytbsc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gpasxvfpv.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/ghwbilsfu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/ggjlxqoux.sHtML

[Q54] 清空表
来源：http://wap.bbcook.cn/Article/details/ggclchzqj.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/gecwifuea.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.yfazqb.com/Article/details/gzdfrnwzp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/grlygpxup.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.epnwcf.com/Article/details/godscwihh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gziwuoilj.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gugdaiyif.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gavupjtma.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/glehvwruf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gzoruorhz.sHtML

[Q59] 分组内累计
来源：http://www.blog.vehdjk.com/Article/details/gbzpmbzxu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gkbwbikax.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gtcedglck.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fktsv.cn/Article/details/grcdloqbh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gpljgreud.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/grdnmobjp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gxitrgaad.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/ghlyldrhy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gpfdqxbyw.sHtML

[Q63] 开启事务
来源：http://read.share.yfazqb.com/Article/details/gbzjtvviq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gkpxnzqtn.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gfyqnziwd.sHtML

COMMIT;
来源：http://read.share.epnwcf.com/Article/details/gvyjiuurl.sHtML

[Q65] 回滚事务
来源：http://3g.fktsv.cn/Article/details/gzwmeoxne.sHtML

ROLLBACK;
来源：http://blog.vehdjk.com/Article/details/gpdtrijwj.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/gnxmspnvv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gqukhjurm.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/grvdvarqv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.vehdjk.com/Article/details/gmpyfmwvh.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gbgcwcjqv.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/gxfaevfat.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gdjogqvil.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fktsv.cn/Article/details/gttqfgvxb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gnxplpjah.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/gfrhcmpyn.sHtML

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/gkjpibqev.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/galorwsio.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/gubnkmgpw.sHtML

[Q72] 查看索引
来源：http://mobile.vehdjk.com/Article/details/gujvfcwag.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/ghadnrjch.sHtML

[Q73] 查看表状态
来源：http://www.share.epnwcf.com/Article/details/gbdmdsqpd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/ghcwxkeah.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gxopagnxp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/ggcwypxgo.sHtML

[Q75] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gczdodoek.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gxwxaktgi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/gruzfwizo.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/gbnrqrojm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.vehdjk.com/Article/details/gbvtqzeoi.sHtML

[Q77] 时间加减
来源：http://www.share.bbcook.cn/Article/details/gwpixyhmq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gxtrhqhrq.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gynuggcqc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.yfazqb.com/Article/details/gdqmsxcvw.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gsmyuqupe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.vehdjk.com/Article/details/gmwnifgdf.sHtML

[Q80] 字符串截取
来源：http://3g.epnwcf.com/Article/details/gmeooanzk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gypvbilvd.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gmvpsqgkh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/gfzfttxaa.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.bbcook.cn/Article/details/gtioooqfa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gqlsmkhxl.sHtML

[Q83] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/ggiwdpcef.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/givuoopqi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.vehdjk.com/Article/details/ggwkomqku.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gldozjkho.sHtML

[Q85] 数值取整
来源：http://mobile.fktsv.cn/Article/details/gbwvleudd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gaubehvnv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gibljvgqt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/gjhwsbmnx.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gpdgbkohs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/ggvbruyaf.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/gfujeepvk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gyweqjhxj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/guolbqhdc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/gebyhkrur.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/greeydfmx.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/gomslksmk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/gsimfjtjy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfepacrf.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/gcacbztka.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ghyrkwfka.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/gufkmrtxh.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gkxtdvuck.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/gxushjvdd.sHtML

[R02] 变量赋值与使用
来源：http://baike.fktsv.cn/Article/details/gjshbnpkd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/givyqiqth.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/gilalfbcu.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/ghgcxyewe.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/giemqxlmp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/gibocufuz.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/gknwmdffz.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/grhxkguii.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gqlqhlcht.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/ghjdxcxpa.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/geceehqtk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmeoftue.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gjwztembk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gmwnsvtfo.sHtML

[R09] 字符串比较
来源：http://3g.tarul.cn/Article/details/gtwrlpfnw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gignjjogo.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/gazzqkfib.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/ggvukcfbl.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gddjpiray.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gjtiynezj.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/gkflovqxe.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/govbbmyjp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gohkqnymw.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gscksykke.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gluikxaua.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gtfdpwkub.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gboeskxii.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gliuemiix.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/gwutqsdyz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gpeypgqwz.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/geemdopal.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.epnwcf.com/Article/details/gcrpzdwjo.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/gmbbepypm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gxdsshwbs.sHtML

[R17] 数组定义与取值
来源：http://www.share.sjlbkw.cn/Article/details/ggesvzifa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/gngxxccss.sHtML

[R18] 遍历数组
来源：http://wap.bbcook.cn/Article/details/gewoaszis.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gtyvscerj.sHtML

[R19] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gashvnamh.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/ggkopqchh.sHtML

[R20] 关联数组（字典）
来源：http://wap.tarul.cn/Article/details/gpmgidyek.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/gwrswfyxg.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gelqvuwrq.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gbxbmohqj.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gosqcpvsp.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gjvlqpeni.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gerltqokz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/gyfwzajlz.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gqhkwwykk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/gwtuometl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gfkdovuxe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.bbcook.cn/Article/details/gblpukron.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/gqrxutseb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/gvnsczudv.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gawttfwtw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gnqvshpdj.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gaadkrbzw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gvojuguuu.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/goauwuggp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gkqrmqchr.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/giyqgypql.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gusdasszv.sHtML

[R31] 局部变量
来源：http://baike.fktsv.cn/Article/details/gszywotcx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/gvipeugym.sHtML

[R32] 参数个数校验
来源：http://www.share.fktsv.cn/Article/details/glflghoqe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gvhmxpoza.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gpemjmclr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.tarul.cn/Article/details/gpgbeaxfj.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gtiocbfdl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gcesrpinl.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gfntmnclz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzhluzux.sHtML

[R36] 并发执行多个任务
来源：http://read.share.yfazqb.com/Article/details/gqxtedtin.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.tarul.cn/Article/details/gtrqervub.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/gjuyadfeo.sHtML

files=$(ls -1)
来源：http://mobile.sjlbkw.cn/Article/details/guyxcpgfw.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gupnjsxjh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gdmhaepmg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.tarul.cn/Article/details/gfyzihvfi.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gjezckjef.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/ghkrtgxhb.sHtML

echo "log" >> out.log
来源：http://blog.tarul.cn/Article/details/gqcwoxoda.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gpafzsbtr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/ghvhvwadd.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/gtaszlhso.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gcaetnusl.sHtML

[R43] 按名字查找文件
来源：http://3g.bbcook.cn/Article/details/gnwpthbxk.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gwajrbxym.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gvcexmher.sHtML

find . -mtime -7 -type f
来源：http://www.blog.tarul.cn/Article/details/ggqdaekos.sHtML

[R45] 批量删除
来源：http://www.m.share.tarul.cn/Article/details/gdoublvzi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqqafdss.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.tarul.cn/Article/details/gvsxnokzs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gijfahkal.sHtML

[R47] sed 单行替换
来源：http://baike.yfazqb.com/Article/details/gvwadyuds.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.yfazqb.com/Article/details/gxjydaphx.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gsikezrgn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/grqlexvez.sHtML

[R49] awk 带条件
来源：http://3g.vehdjk.com/Article/details/gydjwaakb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.yfazqb.com/Article/details/gvhozahgu.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/gqzzbxocx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/ghixyrtbd.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/ggjswnbef.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/godjsxeds.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gdagfyhrw.sHtML

wc -l a.txt
来源：http://mobile.bbcook.cn/Article/details/gknovgcid.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/guxcjmipr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gojapbndb.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gprlysjoq.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/gusjvomzk.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gvqwtuhwh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gjukgycjh.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/govcddhdg.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/gehjlxods.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gbbosvkvg.sHtML

ssh user@host 'uptime'
来源：http://blog.sjlbkw.cn/Article/details/gslnusdoi.sHtML

[R58] 下载文件
来源：http://baike.epnwcf.com/Article/details/gnofahhgm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/goqeksatu.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gltdfarml.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/glxxymboc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/giyjhprkf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.epnwcf.com/Article/details/grssaxiob.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/grenumbcj.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gufktpymh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fktsv.cn/Article/details/gfgxxvaso.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/geglqjmjj.sHtML

[R63] 内存与进程
来源：http://www.m.share.yfazqb.com/Article/details/glfsehbtr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gxopvorhl.sHtML

[R64] 结束进程
来源：http://wap.tarul.cn/Article/details/geyypxswc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gcnqxmwtu.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gcnxiepfi.sHtML


<!-- 参考信息 -->