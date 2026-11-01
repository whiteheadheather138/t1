代发 wailian999

SELECT * FROM users;
来源：http://read.share.vehdjk.com/Article/details/grapdiyec.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gwjiadpbs.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqrmrdifk.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gtidxikzx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gmumejwmv.sHtML

[Q18] 模糊匹配
来源：http://baike.epnwcf.com/Article/details/gxqdbzgyd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gjynchqie.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gwaxzstcb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/gdykhdwer.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/ghxykmsee.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.epnwcf.com/Article/details/gkgvuwhom.sHtML

[Q21] 空值判断
来源：http://m.share.epnwcf.com/Article/details/gefsksvcl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gcormspmm.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gvqayzfhk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/gutgwaypw.sHtML

[Q23] 分页
来源：http://3g.tarul.cn/Article/details/gparsldlo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gcrjlbsgd.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/ggpxdwclk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.bbcook.cn/Article/details/ggltdjelc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/ggtvwxamk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gwgouplxq.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/ghexthmpd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gxylrzjmv.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/gmytxmetg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkqctklja.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/gpgcwnyvj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gwnoiqugl.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/goyuxjgfi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gsapyzkuu.sHtML

[Q30] 分组统计
来源：http://www.m.share.epnwcf.com/Article/details/glqzavkoi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gxznenapp.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gjqvauggy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/geinqlssc.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gwgrbldto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gfivaddqr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fktsv.cn/Article/details/gcjqdppac.sHtML

[Q33] 多列分组
来源：http://blog.fktsv.cn/Article/details/gnyraveqs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/gmjqzwgzq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gqmdbiote.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/gioviduyc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gfgvhqrlt.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gknpsuuul.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gkzblmuhx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gzypkqlju.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gbmxepqad.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.tarul.cn/Article/details/gsfentowd.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/glwgmabvm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.yfazqb.com/Article/details/gdejlrnzz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/galtbtrcy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gyllthjjx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gcpkpvmdg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.epnwcf.com/Article/details/gwjshnfhc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.tarul.cn/Article/details/goezpspkz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fktsv.cn/Article/details/gqfenfvnp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gxgcearsl.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/geaqtqddj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gutarnecr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fktsv.cn/Article/details/gthtpwxct.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/guqujogem.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/glcisagzv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.tarul.cn/Article/details/gbkzqmxwf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/giullzgum.sHtML

[Q43] 标量子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gyievomgy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/gtblvoojm.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gxyvmwrgd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fktsv.cn/Article/details/gipfrbulk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/gcyyjwcij.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gfhcioqob.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkrnyxiw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gycjafdsy.sHtML

[Q47] 与平均值比较
来源：http://www.share.bbcook.cn/Article/details/gcdotrpqe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.tarul.cn/Article/details/gtihffnzo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.sjlbkw.cn/Article/details/gnkipmmot.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gdteledfg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gskhdfeav.sHtML

[Q49] 更新单行
来源：http://www.m.share.tarul.cn/Article/details/gdcunmdwx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gaejnpcua.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gartyuash.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/ghzdvceiv.sHtML

[Q51] 用子查询更新
来源：http://3g.bbcook.cn/Article/details/gyliwoizb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.vehdjk.com/Article/details/gynminqyp.sHtML

[Q52] 删除指定行
来源：http://wap.vehdjk.com/Article/details/gsfbjtdfb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gnjazmsey.sHtML

[Q53] 按条件删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcfpudgr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gzsmaetcm.sHtML

[Q54] 清空表
来源：http://www.m.share.yfazqb.com/Article/details/gfwpusqfe.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gkadqaxap.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gylprqrtb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gubbwkres.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gnzpaumqu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gpakglfke.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gexvdfrhs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/gyzsxqhaz.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gekvytyzz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gxjudklro.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gelcvkkmv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gjktskhfc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.sjlbkw.cn/Article/details/gfgqguqsv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gegywamoz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gpqlhffkr.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/gepzxmrkr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/gsicyocjq.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/ghqjjkpvv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gnvbafhvc.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/grwlziwhq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.epnwcf.com/Article/details/gcyyexuxa.sHtML

[Q64] 提交事务
来源：http://www.m.share.fktsv.cn/Article/details/getpmmtgk.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/ghxitmyhn.sHtML

[Q65] 回滚事务
来源：http://blog.fktsv.cn/Article/details/gilxhlpwh.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gvkpjpwdn.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/gsdhzvgld.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gewzxqpvb.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gajpzcueo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/genfjnwgc.sHtML

[Q68] 保存点
来源：http://3g.sjlbkw.cn/Article/details/geqkynqnt.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/grdptcjad.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gssixmgpa.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/grfwxuqqf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gtpsetldp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gtsozdzrr.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gmjluwmff.sHtML

[Q71] 查看建表语句
来源：http://blog.fktsv.cn/Article/details/gqqmhheix.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.bbcook.cn/Article/details/gvondmekh.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gqcngqace.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/gfdixrrfi.sHtML

[Q73] 查看表状态
来源：http://blog.tarul.cn/Article/details/gzplhhcxp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gtuhqgyty.sHtML

[Q74] 强制使用索引
来源：http://baike.yfazqb.com/Article/details/gtyjvtthx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.epnwcf.com/Article/details/gvmdmoefc.sHtML

[Q75] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gferajcax.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gtbwfeajp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.vehdjk.com/Article/details/gsxygrvqo.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/geodpamgp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/glxglbnjl.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gquokxrev.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/gtigdkupz.sHtML

[Q78] 当前时间
来源：http://wap.epnwcf.com/Article/details/gacykklxx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.vehdjk.com/Article/details/gyhoemmhl.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gfaqkenox.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/gmywfinus.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gbtjajqon.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gyifsosyt.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gczahluvo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fktsv.cn/Article/details/gmjtzmarn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gjjrrgjom.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/glmovshbl.sHtML

[Q83] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gjdsgmxcn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/glttyfqwk.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gjgvnvcux.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gaiuixvax.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/gaxeolzex.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/gxshbqjtd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gguemkkcx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gslhdnrez.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/gdxahjnfo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gwgxcbjfw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.bbcook.cn/Article/details/gculfzicy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/ggchmlvwk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.vehdjk.com/Article/details/ghnzqobza.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gyvhnyuwu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.bbcook.cn/Article/details/ggqtzpdxz.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gxdclhgrj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/gulyyeyvg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/goseqqgtk.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/gqxgfqwny.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/guwlbxsjk.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gxgydybch.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/gcfsnxtxk.sHtML

set -euo pipefail
来源：http://www.m.share.vehdjk.com/Article/details/gadwmbndd.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/geznifgll.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gaxncsied.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/ghawpizvt.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gdkpmtsnz.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gnyfvhrye.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/glewbzrey.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gtaiozvde.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/goomdwqpy.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/gqogjkjbr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gmtykarqv.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gyoucximd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fktsv.cn/Article/details/gqcgoikft.sHtML

[R08] 数值比较
来源：http://www.blog.bbcook.cn/Article/details/gcyyetipa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.bbcook.cn/Article/details/gqziuhwdw.sHtML

[R09] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gfjmdgfnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/gjnsjrutz.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/gyqnnxqzx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.epnwcf.com/Article/details/gkuaialja.sHtML

[R11] case 多分支
来源：http://m.share.epnwcf.com/Article/details/gnqufszrm.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/gfntakzkz.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/gxyvurbwq.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gkiodptzl.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gahosjnol.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/gyrnruqae.sHtML

[R12] for 遍历文件
来源：http://mobile.vehdjk.com/Article/details/goibtcgvy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gaugcyepb.sHtML

[R13] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gowfsuohs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gcqbtkbyj.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gerpurraf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gllnpavqa.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gujrjdyvc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gwytlciys.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/gzejcmijv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gxakxnsql.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gipebjzpz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gwcwoubgd.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gqacajaqk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/glyndkjji.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gghawfhid.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gmpeuivpe.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/ggkrwaerj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.epnwcf.com/Article/details/gkhsagjdg.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/gdvcwbkfa.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gglxqcwkz.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/grklbknim.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gdkgropdn.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gkajyeino.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gkjwqkxaz.sHtML

[R24] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gliblhbkk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/grrzfkfhd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/glkqippnz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gwgvkeetj.sHtML

[R26] 命令替换
来源：http://www.share.yfazqb.com/Article/details/givvxlfwn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.tarul.cn/Article/details/gqgnomzii.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gqdycbvuf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.yfazqb.com/Article/details/gswfrapor.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gdgfdgypo.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/grqlapdsm.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/garmyzvxl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/gsqbnduzl.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/gijclmyea.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gpmfztniz.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gonbeuvje.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/gqikcfbkf.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/ghnjjgifx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gbeodxxml.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gxhdtotev.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gvlzyjnrx.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gsrfsvvva.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gpbcdtlht.sHtML

[R35] 后台执行并等待
来源：http://www.blog.tarul.cn/Article/details/ggjmswion.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.sjlbkw.cn/Article/details/gipvksurl.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gugqyhcpp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.sjlbkw.cn/Article/details/gxmpmzvdj.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/gimthigal.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gtiyzbrey.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/guigmwgpo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gdpphcfkg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gcvljswto.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gokqyquin.sHtML

[R40] 追加写日志
来源：http://baike.fktsv.cn/Article/details/geatbftqr.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/guzbhzfvi.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/gfmunecvg.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gvgggwlsv.sHtML

[R42] 输入重定向
来源：http://www.blog.sjlbkw.cn/Article/details/gbhdtlaqz.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/gpbdrycsd.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gsjxelifz.sHtML

find . -name "*.log" -type f
来源：http://blog.fktsv.cn/Article/details/gctkfyysm.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/ghwraoqpj.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gcwwfpmmd.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/ghgmzamcw.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/gwpaevocr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gnfedvbqu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/gyvawkzgf.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gizdlmxdt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gxoocsdlu.sHtML

[R48] awk 取指定列
来源：http://mobile.fktsv.cn/Article/details/gylubaenk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gqbizghkb.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gvmurylpi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/ghgjkdtmc.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/gvltmupiy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/goutavlvs.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gqdvqcyeh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/giyvwgtnt.sHtML

[R52] 统计行数
来源：http://3g.fktsv.cn/Article/details/gphckaktu.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gvooibtbb.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/goazqdfhx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/ggobadofb.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/guylnyyqr.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/gtozrrokx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbxlujkv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/grdxulqhw.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gabfkprlu.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/ghsmwzppc.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/gondssgix.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gnhjdbkaf.sHtML

[R58] 下载文件
来源：http://wap.sjlbkw.cn/Article/details/gnkclayij.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fktsv.cn/Article/details/gkcaavsrv.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/ghhlcamuu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gmszjdusv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/goawlozsf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/gpsuyohcs.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gynosjzja.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gjbcwdsti.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gumkglbkw.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/gzrkitufl.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gltfajvxw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gipxqrsgo.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gzlablpek.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/gascvbcrj.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gossvfsup.sHtML


<!-- 参考信息 -->