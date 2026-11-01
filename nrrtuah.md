代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gyjtygtgz.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/glcdwxddq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gaaciodmz.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/gjxovevcy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/gqorwfzjb.sHtML

[Q20] IN 列表
来源：http://baike.epnwcf.com/Article/details/gztkftzlf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/gdmettxoy.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/ghyrhqrys.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gwvguxxpa.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/ghzsbclty.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gusxrgbax.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gbvtsyeqz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gfcxipyis.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/gsiiqypiv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gfrwfcaob.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gvdhhgwyx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gujjybvpw.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gjsclthwr.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gqheeanog.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/gxhkwpmrl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/geuvirzun.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/gewgebqls.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gdlljtpxa.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/gctocuevb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gnismlwxt.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/goqecooxk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gtbysixpz.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gtinynjlh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.vehdjk.com/Article/details/gqblvmygu.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gbycfwjwv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gqmaitfqt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gqfyycutd.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/gujswcrge.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gbdikpuwp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gvzmqonno.sHtML

SELECT * FROM (
来源：http://www.share.tarul.cn/Article/details/gtgextylk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/gggujtsep.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gfhjyatmu.sHtML

[Q35] 内连接
来源：http://3g.vehdjk.com/Article/details/gofdqugad.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/grtmcpyom.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gdlzlciuh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gsrxhbrko.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/gtnbktial.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gnyadpehr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gujhpodwj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/guctewkmk.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/guwahmtbg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gelcbyzsj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.epnwcf.com/Article/details/gjixlsgab.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gtsehfdsp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/ggnvhrfui.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/goauijwrq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.epnwcf.com/Article/details/ghnoeuvjk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/gzdrgbfpp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/gjxmbfrat.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gouihwkpy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/gjeksrrcm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/ghttcyzfi.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gmnrfqpnk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gysynhcaf.sHtML

[Q44] IN 子查询
来源：http://www.share.epnwcf.com/Article/details/gddfqlsgf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/geubykqsr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fktsv.cn/Article/details/gowbfddsv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gpxrfbprg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.tarul.cn/Article/details/gbkitalzr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gbdlmihrm.sHtML

[Q47] 与平均值比较
来源：http://3g.sjlbkw.cn/Article/details/gyoebicvx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.vehdjk.com/Article/details/gjldwljev.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.sjlbkw.cn/Article/details/gwyvnzjkz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gcektdotb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gvikxjrez.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gzxiocahp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gupdqznnn.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/gehsdipkw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.bbcook.cn/Article/details/gvuctdrix.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gcijfjnib.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/ghszyddbu.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/gqteozsdo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gidrauoif.sHtML

[Q53] 按条件删除
来源：http://3g.tarul.cn/Article/details/gkrndbzta.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.tarul.cn/Article/details/geohaesal.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gokruvysm.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/grzrfobdt.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/ghogmnseh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gkcszxmjc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/gktolzdda.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/gtiouamdj.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/gctdkjuqh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.sjlbkw.cn/Article/details/golzzebiw.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gbsrgwaob.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/ghwoqthpm.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/glbblzyhx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gzfjcutfv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.yfazqb.com/Article/details/gqqqkdmyy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/gciuqclxk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gcfmivakb.sHtML

[Q61] 移动平均
来源：http://read.share.fktsv.cn/Article/details/ghcfzivpy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gixfoqhbk.sHtML

[Q62] 分组占比
来源：http://read.share.vehdjk.com/Article/details/gdqpihxza.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gdvukakdj.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/gccfmdmcm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gfzhkchpl.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gzhxrwfon.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/gqxustuoj.sHtML

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gtgrjouhj.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/grldwcrgf.sHtML

[Q66] 行锁查询
来源：http://mobile.sjlbkw.cn/Article/details/gdqglbbxf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gtiavtjfz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/gmqsoijrd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.sjlbkw.cn/Article/details/gknxykrbt.sHtML

[Q68] 保存点
来源：http://blog.epnwcf.com/Article/details/gcnmucqbc.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/goivwsxqo.sHtML

ROLLBACK TO sp1;
来源：http://blog.epnwcf.com/Article/details/gjtdxkztu.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/gsfkupuff.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.yfazqb.com/Article/details/glacasbpd.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/gqivlacoq.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/gfbodgdus.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gqcfxzkki.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/govuxuxqv.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gqdzvjiql.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gcljutbxg.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gcflilxzh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gjybpgoxa.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gothgbyhi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/gvktlzwho.sHtML

[Q75] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gsuvyvext.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gsnviqitx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/googinmnu.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gwyzluacm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/glovctjia.sHtML

[Q77] 时间加减
来源：http://mobile.tarul.cn/Article/details/gfbbgubrg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/gqcqswpkq.sHtML

[Q78] 当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gczdbypxj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.yfazqb.com/Article/details/gdwzhzoaj.sHtML

[Q79] 字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gpmrfyolt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.sjlbkw.cn/Article/details/gmumzdkxg.sHtML

[Q80] 字符串截取
来源：http://www.blog.epnwcf.com/Article/details/gjlwqlqyx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/gvkzctsed.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gchlooxzs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ggokrvsvr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gdnychgds.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/getkzavog.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gdzwdkxxa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gfeemkogk.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gtzrrkfln.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gtpquerxi.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/gakrlzknc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gnaensvcy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gokbteslo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.epnwcf.com/Article/details/gprazegpq.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/gyollbepr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/gnbzmivdp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gzcjzggce.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/gmbfsaddo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.vehdjk.com/Article/details/ggzixvfoi.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gzqhesbxp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gurylmwis.sHtML

[Q90] 生成序号列
来源：http://3g.bbcook.cn/Article/details/gfzecwzbx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gwbamsush.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwycxogvf.sHtML

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/gzblksfrk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqgdrmvqw.sHtML

[R01] shebang 与严格模式
来源：http://blog.tarul.cn/Article/details/ghxncpxfz.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gqkrnpmlb.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gblvunckt.sHtML

[R02] 变量赋值与使用
来源：http://www.share.sjlbkw.cn/Article/details/gvrlztctl.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gmblkvxwq.sHtML

[R03] 只读变量
来源：http://baike.yfazqb.com/Article/details/gxzmpvrzw.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/glpemyiix.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/gbvchrblb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/geqnzmtfo.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gyetyvzlz.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/glltxgubx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gyamxiooj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gfirffjtb.sHtML

[R07] if 判断文件
来源：http://baike.fktsv.cn/Article/details/ghjxfhjud.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/gfclqvukv.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/gglpwhqgu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gurchmrmv.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gvgujathb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gxqicygag.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gjxohrxrx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.yfazqb.com/Article/details/gtkdjdasx.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/glkxigwxo.sHtML

case "$1" in
来源：http://blog.fktsv.cn/Article/details/gemchfeqf.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gxsapqmnu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gxzzecnxy.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.tarul.cn/Article/details/gqbjhezzr.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/glurtteav.sHtML

[R12] for 遍历文件
来源：http://baike.sjlbkw.cn/Article/details/gmgdnctng.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.vehdjk.com/Article/details/glodouocb.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gfwocfjjl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gjwcksrii.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/gkeyaxoip.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gxrzfhnyd.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gtuloyhwa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/gvrekqjwc.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gzzjbilab.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gpidqbwxv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gxqjzvvlh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/gvmpgmcpy.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gionqotxo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gbzpfrdpl.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/gtesoyajh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.vehdjk.com/Article/details/gzvwuemly.sHtML

[R20] 关联数组（字典）
来源：http://wap.tarul.cn/Article/details/gfiunmebd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/gfanvakas.sHtML

[R21] 字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gwwalzpma.sHtML

echo "${#s}"
来源：http://blog.fktsv.cn/Article/details/gpdyvpcbo.sHtML

[R22] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gqpgpzyhp.sHtML

echo "${s:0:5}"
来源：http://www.share.vehdjk.com/Article/details/gwknzyrrj.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gpzrbmqpe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gcbedanbn.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gzrbvnsgx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gdghzjujh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.bbcook.cn/Article/details/gazrgntyr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gchfcijcw.sHtML

[R26] 命令替换
来源：http://www.blog.tarul.cn/Article/details/gjnofzdns.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/gtmzsdtgv.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/gkxmcieio.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gjjkpebkk.sHtML

[R28] 浮点运算
来源：http://www.m.share.epnwcf.com/Article/details/gmecmbjwz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.bbcook.cn/Article/details/givwdxwcq.sHtML

[R29] 定义函数
来源：http://m.share.tarul.cn/Article/details/giwjefcpn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.tarul.cn/Article/details/gbfryzgzb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gnrqvchap.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/geuhtakvw.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gahmbjfjw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/gbphypadm.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gsontsalq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gpkibtrgj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gtpiwccad.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.sjlbkw.cn/Article/details/gbhfmjnho.sHtML

[R34] 退出时清理
来源：http://read.share.epnwcf.com/Article/details/gyokkxyhh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gfduupbir.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gudqeaxjq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gdiconlhp.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gwndeiicn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/ggxwepsup.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/gcrtkncbn.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/ghqeloxpw.sHtML

[R38] 管道串联
来源：http://baike.tarul.cn/Article/details/gjrsenrnr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gynldagjz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gjkrdlpbp.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gzdklopai.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gestogpie.sHtML

echo "log" >> out.log
来源：http://3g.yfazqb.com/Article/details/gqpnfwntm.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gnwzkfrmo.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.bbcook.cn/Article/details/gzqadznse.sHtML

[R42] 输入重定向
来源：http://www.m.share.epnwcf.com/Article/details/ggqdqiuzc.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/ggpvccgvg.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gqrexoiwt.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gphqnkdzh.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gwsjpdjzx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/gtcdklwsy.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gpfmkrqlo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/goqtshclz.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gcgnyiexe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gsbcrrdrw.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gohgsqhzu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gxdsldere.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gfwgkkrgd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gbybuusvk.sHtML

[R49] awk 带条件
来源：http://blog.tarul.cn/Article/details/gnmbtagyh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/ghbpviwxe.sHtML

[R50] awk 求和
来源：http://mobile.sjlbkw.cn/Article/details/gjgeztqdd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gjeowzkoz.sHtML

[R51] 排序去重取前几
来源：http://mobile.sjlbkw.cn/Article/details/gsjyeqhsd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.bbcook.cn/Article/details/gzgyhlvrz.sHtML

[R52] 统计行数
来源：http://baike.bbcook.cn/Article/details/guexjjkuz.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gygqhjtxk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/golnufodc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfhuoiod.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/grazetsms.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gfxamghra.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/grcoffkcg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/glnpcaysg.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/ghuddgmnm.sHtML

scp file user@host:/path/
来源：http://www.m.share.tarul.cn/Article/details/gwcarxvcg.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gsbrucdhc.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/ggbsquauy.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/ggqxmkphg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.sjlbkw.cn/Article/details/gwununzmv.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gdhnkmsvx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/gyrxtbcuq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gvrdnxfzl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gxqtuqfpi.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gcexcuzsc.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gwarykiqz.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gtjfdexfq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.sjlbkw.cn/Article/details/ggccyreav.sHtML

[R63] 内存与进程
来源：http://wap.vehdjk.com/Article/details/gnjuzazzb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/gkwtetoco.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gavkvkqhp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/gdcrntfgu.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gqpflrefn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/gmtlktfcx.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gnwmpsacn.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/ghllqlopk.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.sjlbkw.cn/Article/details/gnabpkjhf.sHtML


<!-- 参考信息 -->