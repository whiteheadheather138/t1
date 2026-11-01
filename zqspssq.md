代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpdpmslf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gtmciiovc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/grzxwvshr.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/gzpeojneu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.sjlbkw.cn/Article/details/gamayxllu.sHtML

[Q20] IN 列表
来源：http://www.blog.tarul.cn/Article/details/gdycymxkd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.bbcook.cn/Article/details/gdoggvkbj.sHtML

[Q21] 空值判断
来源：http://baike.yfazqb.com/Article/details/geblvbpct.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gegqhkajv.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/gdkhdyqck.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/gygbjgsuy.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/guznglbxx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gxfjagynt.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gbhfhsssh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/gerpphzzi.sHtML

[Q25] 只取前 N 条
来源：http://3g.vehdjk.com/Article/details/gfuoqtsts.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/gxfupkuyp.sHtML

[Q26] 计数
来源：http://read.share.vehdjk.com/Article/details/gumbvufil.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gfvafknff.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gfpilzhkr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/grtdkbyyt.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/gyxtouvyq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/glpislauq.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/glyfzboao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/gcdlmhepj.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gvagcxknc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/glogqfxab.sHtML

[Q31] 分组后过滤
来源：http://m.share.sjlbkw.cn/Article/details/gwtugseou.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.vehdjk.com/Article/details/gsvvcwjoa.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gehbbodte.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gdmdszhgc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/goylbmwme.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/glewangoo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/guhqnvlec.sHtML

[Q34] 每组取第一条
来源：http://wap.fktsv.cn/Article/details/ggxfwnsby.sHtML

SELECT * FROM (
来源：http://mobile.sjlbkw.cn/Article/details/gvqdtdxpl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/gdjduhjxb.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/gvvsfibyv.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gtanqjvxi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/ghpwjueui.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gvnvreftw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gkzyvnanm.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gynwvygdf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gqwwfqfav.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gcmiepvhv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.vehdjk.com/Article/details/gaoykdcyp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/graanrqoj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.vehdjk.com/Article/details/gdwmwkypz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gumdsjcqr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gpthrvayb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gjmpmasbp.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/ganafsqdz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.yfazqb.com/Article/details/gvowkmgpv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.epnwcf.com/Article/details/gkebdwuff.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gwaxgiies.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/ggcpkmhos.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.bbcook.cn/Article/details/gglzixqnf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/gscpoykav.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/gxvuyabjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/gfpexhugv.sHtML

[Q44] IN 子查询
来源：http://read.share.yfazqb.com/Article/details/gwetxmkok.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.yfazqb.com/Article/details/gcncduhjf.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.epnwcf.com/Article/details/gaqpqchbc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/ggrbshvhc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/gjmlzawgd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gjuqulnkq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gcnvouwez.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gtjiindli.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/ghfenxdcs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/glhcyzhaf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/gfiodhqql.sHtML

[Q49] 更新单行
来源：http://mobile.sjlbkw.cn/Article/details/ghudlackp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gfqcutjtb.sHtML

[Q50] 批量更新
来源：http://mobile.vehdjk.com/Article/details/grspvassn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gohjtpkgc.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/grkhakupb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/glifwixtj.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gfydpjmom.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/ggfzovdcg.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/ghxmsrxmy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gcpynhchz.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/gjffguxnm.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gagcdcuwe.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/gqhczzbzv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gwaotdqwx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/ggwofffxs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gckoxzykx.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/glyenbtov.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gzfxcqatu.sHtML

[Q58] 累计求和
来源：http://wap.epnwcf.com/Article/details/gsapylesu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.epnwcf.com/Article/details/giyqlvsyi.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gbuuzsrau.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.bbcook.cn/Article/details/ggtdjeyxk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gtaadgitd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gsslggdgg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.bbcook.cn/Article/details/gsiiiczvp.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/gnytfhosu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/ggzdosmqd.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/gjkgigsbs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/glrclvdff.sHtML

[Q63] 开启事务
来源：http://read.share.fktsv.cn/Article/details/ggssvsucm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/ghgiciyib.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/guvqvbcaj.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/geivvvauv.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/gctgqlrdp.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gybxjcxcx.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/gesvwplno.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.tarul.cn/Article/details/geoomjvsy.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gqpfjcovp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/gtbverizo.sHtML

[Q68] 保存点
来源：http://blog.yfazqb.com/Article/details/gzfvgturd.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gdgisvoga.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fktsv.cn/Article/details/ghiwaqdem.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gepokobch.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gskmsrqvw.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/gdlkzccqf.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/guxoukbge.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gjtztwigq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/gkhvqzlzq.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gdqmwfhsr.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/grxibgayx.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gjjsiucki.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gvtofavof.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gmqmkuomg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gdjdwfzji.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gmqywhlxn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gopbleupc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gjlichuyb.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gjmoxsslb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/gsildpmwz.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/gvdqgqfxi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/ghreqxcjf.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gtkyzlpvo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/grwaypkdr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gkdrwyhkw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gqawsuwhw.sHtML

[Q80] 字符串截取
来源：http://baike.sjlbkw.cn/Article/details/gnuwwbvhw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gszignwto.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gikisjkgi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gwffuqbwx.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gllcbjuiw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gienqdvkz.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gryzxvwhg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gytezjphb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/grrhudeal.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gxfljajee.sHtML

[Q85] 数值取整
来源：http://mobile.sjlbkw.cn/Article/details/gkesvpduu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gdzqhlxej.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gkmzgcqrk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.vehdjk.com/Article/details/gqzrusdoj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.sjlbkw.cn/Article/details/gypglddxs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/gtkkbjfap.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gunoledat.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.vehdjk.com/Article/details/gvsnchssl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gmrzsxndr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gcbjpeyuk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/ghdbvgixf.sHtML

[Q90] 生成序号列
来源：http://mobile.bbcook.cn/Article/details/gagzbgwxr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/ggobgletf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gllzrxpsq.sHtML

R. Bash 专题
来源：http://wap.tarul.cn/Article/details/gefdxisnc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gzvntkzxd.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gcnxdvggo.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/gjyzfujci.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/gbsbpilig.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/gmphcfnui.sHtML

name="Tom"; echo "$name"
来源：http://www.share.vehdjk.com/Article/details/ghrrofnps.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gihrdcfij.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gfdtrmtaj.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gisdnrdiw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.sjlbkw.cn/Article/details/ghiksbwuh.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbpwijww.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/ghglfoifr.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/gqgpaeqxc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gptmqlmim.sHtML

[R07] if 判断文件
来源：http://read.share.fktsv.cn/Article/details/girrgciaw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.bbcook.cn/Article/details/gxvwrgdqr.sHtML

[R08] 数值比较
来源：http://www.blog.epnwcf.com/Article/details/guxczkjlf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gvdnowzfb.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/geolbksmx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/gmhmbxauk.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/gidtclaag.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/gzycmakkt.sHtML

[R11] case 多分支
来源：http://read.share.yfazqb.com/Article/details/gzjjohfpr.sHtML

case "$1" in
来源：http://www.m.share.yfazqb.com/Article/details/gefijhqrs.sHtML

start) echo "启动" ;;
来源：http://wap.tarul.cn/Article/details/gslzkmwqc.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gnodoixzf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.vehdjk.com/Article/details/geenmrvzn.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/glotkmoen.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/glqtbydka.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.vehdjk.com/Article/details/gtyfnpcoq.sHtML

[R13] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/gazviaubg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/ghaltyetv.sHtML

[R14] C 风格 for
来源：http://baike.yfazqb.com/Article/details/gdcxxehcc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gzjgwurjl.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gfrihpjtt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gffwiwwsn.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/glnrvbwpp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.bbcook.cn/Article/details/goicxhzhl.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gnlmbiatw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gmrkbrabu.sHtML

[R18] 遍历数组
来源：http://www.blog.vehdjk.com/Article/details/gfakzkyjg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gxbqbnfqr.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gcusszsri.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gphfpkaeu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gskgrrsah.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gtwxhvraf.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gupnpfaoz.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/gvqgvupxy.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/ghbnklami.sHtML

echo "${s:0:5}"
来源：http://3g.bbcook.cn/Article/details/ggdtggdlr.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/ggdcuzxdj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gkclzywji.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gdqdnsuaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/grinlaofh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/gcgswibop.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fktsv.cn/Article/details/ghghbvxjo.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/gvylywaco.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gbcostyjx.sHtML

[R27] 算术展开
来源：http://baike.vehdjk.com/Article/details/gcqepggpg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/gzgjziaom.sHtML

[R28] 浮点运算
来源：http://mobile.sjlbkw.cn/Article/details/ghwrtjfgf.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/gstxwnubi.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gudaxhnku.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.epnwcf.com/Article/details/gqsefizjz.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gwxhkjvbw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/gbuvlfgov.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gzahvilip.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gzyoamwmv.sHtML

[R32] 参数个数校验
来源：http://blog.fktsv.cn/Article/details/gkideqyjp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/ghgbgxcmn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gybdgocjl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.bbcook.cn/Article/details/glgnqrejs.sHtML

[R34] 退出时清理
来源：http://mobile.epnwcf.com/Article/details/gkudmkouq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/gbkdqujfs.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/gowzkuqml.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gdhcrcsqj.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gfvlqfrbr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.sjlbkw.cn/Article/details/gdlucroxs.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/gijakzvyj.sHtML

files=$(ls -1)
来源：http://www.blog.tarul.cn/Article/details/gbohzwjfp.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gsqyowtyr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gpeyqozxj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.yfazqb.com/Article/details/gvhwlvsst.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gavxgiojf.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/gqinloufp.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/gjvlsydoc.sHtML

[R41] 丢弃输出
来源：http://wap.yfazqb.com/Article/details/gxsemrnzq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gbwoibqcl.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gjifhllig.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/geabfbgdj.sHtML

[R43] 按名字查找文件
来源：http://www.share.sjlbkw.cn/Article/details/glrxqgrsx.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gxulcvluf.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gkbbwllgm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gpfgkqzot.sHtML

[R45] 批量删除
来源：http://www.blog.tarul.cn/Article/details/gpdzpdkrk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/gixdhhvvu.sHtML

[R46] 递归替换文件内容
来源：http://read.share.bbcook.cn/Article/details/gsmnbudyx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.bbcook.cn/Article/details/gdgrdlqeq.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gwxkwouqk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gfhflsass.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gzydxbjkw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gkwzvizcn.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gsrgzyatz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gkademdrq.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/gdfgglfgb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gyumbtftb.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/gertjuyow.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gwzlqfpmf.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/grxlmwncm.sHtML

wc -l a.txt
来源：http://www.blog.epnwcf.com/Article/details/ghypuykva.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.yfazqb.com/Article/details/gigqlxtci.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gyspbppax.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gunvbeiuw.sHtML

diff a.txt b.txt
来源：http://baike.sjlbkw.cn/Article/details/ggoaunuuf.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gmmtoskus.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gjbxgjlnz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gcabkhqaa.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gmntqotpd.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gbygrzica.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/glihwsqjd.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gceuztmyk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gdzxxqyuk.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gtsfkpqmn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/goquszzzk.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gnvgokiox.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/ghqiyqzlg.sHtML

[R61] 磁盘占用
来源：http://read.share.vehdjk.com/Article/details/giomutauw.sHtML

df -h;  du -sh *
来源：http://www.share.tarul.cn/Article/details/gjgdswmrn.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/glpyhcnem.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/gmedxksfu.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gcllufaak.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/ghhzxgtqm.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/gapcwdaiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.sjlbkw.cn/Article/details/gyexsitfy.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gcmvofubs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gwqohmzyi.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gfsyuuahd.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/gsrzgjceh.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gszoyeghu.sHtML


<!-- 参考信息 -->