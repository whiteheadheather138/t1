代发 wailian999

SELECT * FROM users;
来源：http://m.share.yfazqb.com/Article/details/gbtgwukpk.sHtML

[Q16] 查询指定列
来源：http://www.blog.yfazqb.com/Article/details/gbvfdwgsl.sHtML

SELECT id, name FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/glfzonvhe.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gvjkoioiv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.epnwcf.com/Article/details/gacwopcoz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.epnwcf.com/Article/details/gxqwyemgw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gkutrrnub.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/gonrjyppj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/gzfxwbwxu.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/gzjytliyh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/gfokudnhm.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/gokfoeqbo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/gigqpblus.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gpknmldyu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.tarul.cn/Article/details/gjtnikvgl.sHtML

[Q23] 分页
来源：http://wap.yfazqb.com/Article/details/gzsxqqrcn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fktsv.cn/Article/details/gseraqzfs.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/gudfkvzwo.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fktsv.cn/Article/details/gcmhmihqn.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/girujeoct.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.vehdjk.com/Article/details/gvgiizssy.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/gclqwfatv.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gxyzjmiml.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gmdluozhg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.yfazqb.com/Article/details/guljeuztc.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/godvtvlhr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gjadfgqpb.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/ghvhgdxlz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gjuyvmzkq.sHtML

[Q30] 分组统计
来源：http://read.share.sjlbkw.cn/Article/details/gnbqvshsf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gasfhgqnq.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gganpuvun.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gasavhsmb.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gyzfumuyd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gxzwmzekv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gogksdepn.sHtML

[Q33] 多列分组
来源：http://blog.fktsv.cn/Article/details/gfaartnyc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gsmqhtutq.sHtML

[Q34] 每组取第一条
来源：http://3g.sjlbkw.cn/Article/details/gojoszmlc.sHtML

SELECT * FROM (
来源：http://www.share.sjlbkw.cn/Article/details/gyjygegbd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/giomrerox.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/gjegimhzn.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gdoksiebk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gypadnewf.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/gtbtzhymc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gjzakifob.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gxjbgwjiw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/gvmofkklv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gajhqrnam.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.yfazqb.com/Article/details/grwzlwppz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fktsv.cn/Article/details/gsiowmzay.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/gbaoagici.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fktsv.cn/Article/details/gqhxpegqr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.bbcook.cn/Article/details/gwjbvrosw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gtqtyzmon.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gdrxoeniv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fktsv.cn/Article/details/glucnuhyb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fktsv.cn/Article/details/gmhdtwahy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fktsv.cn/Article/details/gusulmfgp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gebwxpypf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.sjlbkw.cn/Article/details/gjauquult.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.tarul.cn/Article/details/grglnqlva.sHtML

[Q43] 标量子查询
来源：http://read.share.yfazqb.com/Article/details/gppxscqow.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/ghkrztkya.sHtML

[Q44] IN 子查询
来源：http://www.m.share.yfazqb.com/Article/details/gmgunsuxq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/gqtrgujmp.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/gokzsieig.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gqtufurmj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/gflmurgzf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gdkevxshj.sHtML

[Q47] 与平均值比较
来源：http://www.blog.vehdjk.com/Article/details/gqzwbnwgb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/gcebcddzz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gjgjuodga.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gpeoscwnj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gdhlzwutw.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/gwlkikxeu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gkvrwdtgi.sHtML

[Q50] 批量更新
来源：http://baike.yfazqb.com/Article/details/gkndikflj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.tarul.cn/Article/details/gflphpmtk.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gpkwvsevu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/gcuaqipfk.sHtML

[Q52] 删除指定行
来源：http://mobile.bbcook.cn/Article/details/gldguzxyl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gxupmiidp.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/gxahcpjoh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gnzvcrlgz.sHtML

[Q54] 清空表
来源：http://read.share.fktsv.cn/Article/details/gsbfusnad.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/gyrrohphq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.sjlbkw.cn/Article/details/gocgijunx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gsxibnzyn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.vehdjk.com/Article/details/gpgxnhbor.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gxtswqrzc.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/ggwywneve.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gyjsazcqw.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gbfxkwvuo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/ggcfbjbpk.sHtML

[Q59] 分组内累计
来源：http://www.blog.yfazqb.com/Article/details/gbvlplnce.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fktsv.cn/Article/details/ghvqcmdgc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/gmsmqtahw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.sjlbkw.cn/Article/details/gjweicfmf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gnivdrlsb.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/ggbwdmkhz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gdznwajmt.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/gmrlvwscy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/geodhlozm.sHtML

[Q63] 开启事务
来源：http://blog.fktsv.cn/Article/details/gqrqghcuk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gzfhlmuvr.sHtML

[Q64] 提交事务
来源：http://www.m.share.fktsv.cn/Article/details/gcetiuolw.sHtML

COMMIT;
来源：http://www.m.share.fktsv.cn/Article/details/gaztqbgnl.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gkmmhlskg.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/gxxwjtxou.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gzmnhywim.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/grocihtyn.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/gyesuzhdd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/gjqznusds.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gmhxzqnaq.sHtML

SAVEPOINT sp1;
来源：http://read.share.fktsv.cn/Article/details/gypfzhvis.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gtzvxwgfj.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gqttyggsx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/grszdbljw.sHtML

[Q70] 更新统计信息
来源：http://read.share.vehdjk.com/Article/details/gdwfuomze.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gbfdaaceb.sHtML

[Q71] 查看建表语句
来源：http://www.blog.yfazqb.com/Article/details/gbilyetmr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gnevuqjtm.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/gnfakjrrw.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/gzcdwkagf.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/ggcqvjsus.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fktsv.cn/Article/details/gftwchzen.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gmtaxvejl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/gcbstltoz.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gpnrfhodf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/gffpxfvpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gugqobmks.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gfmssfalm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/grzdcqjrl.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/gcixfrpsj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gayootdns.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/gskxyjydd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gsskdjvyk.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gpemtfxcr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/goxduqahb.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmdojook.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/ggxpvelmy.sHtML

[Q81] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gtkgkbvqd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/ghasfenum.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/ggggkjyna.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/galxpcujm.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gvejpilha.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gmbprskiy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/gyvxfdyvv.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gimfavqtn.sHtML

[Q85] 数值取整
来源：http://www.m.share.epnwcf.com/Article/details/gbmaolmre.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/gaiifhoow.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/ggrlcgndi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/gzusbloib.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fktsv.cn/Article/details/glibgezsd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.vehdjk.com/Article/details/gjrbebdfo.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/grueuipbg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.vehdjk.com/Article/details/goujvtlzg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gninktwcq.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/gojwvowfq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gjglfdnek.sHtML

[Q90] 生成序号列
来源：http://m.share.epnwcf.com/Article/details/geffikllk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/gexxwttza.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpxbbyhsi.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gqyerqcso.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glcosxmbr.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/goorsvyva.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gmwvqbofo.sHtML

set -euo pipefail
来源：http://blog.sjlbkw.cn/Article/details/gvmkjwavy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gwbhauozx.sHtML

name="Tom"; echo "$name"
来源：http://3g.sjlbkw.cn/Article/details/gevkgkdis.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gmqgxrctg.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gnqquyukj.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/gdkdnfljm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/gyezhwjuw.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gopvgzzif.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gygkqbgcn.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/gjuffgwei.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gvcssmwrp.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gkymfwdfj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/ggxxzeieq.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/gwlnnivyk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gdrdrpulq.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/ggdxibwbm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/giqnsjoqn.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gevhlgjcf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gfsipbnng.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/gxobmshpi.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/gvrqhrimp.sHtML

start) echo "启动" ;;
来源：http://www.m.share.tarul.cn/Article/details/ghogxvaoj.sHtML

stop)  echo "停止" ;;
来源：http://baike.vehdjk.com/Article/details/gkacnraak.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gytlyukue.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gpoqusxnz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/gsabfwfud.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fktsv.cn/Article/details/gcxijviug.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/garmhdlnk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gdwdwwagu.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gwhzuqqtq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gcuxcqfzu.sHtML

[R15] while 逐行读文件
来源：http://3g.yfazqb.com/Article/details/gqggnzucf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gzjprsarp.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gmihdruci.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gmmamxgwe.sHtML

[R17] 数组定义与取值
来源：http://blog.bbcook.cn/Article/details/gdgbnojox.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/gdsmohubx.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/goapbhvsc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gxgtxjskr.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/glowgltuo.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/gmrthmloo.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/glzugchqs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gwunsbbbw.sHtML

[R21] 字符串长度
来源：http://read.share.fktsv.cn/Article/details/gkmxazwha.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gsvgvxphs.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/gniduhcsm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/grlzhopqo.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gfpsdmsoc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gbkdjtgiz.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gcdlqcuyy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/goficfbiu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.yfazqb.com/Article/details/gzznkbdzw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/gaezjolxb.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gguodsftr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/ghlanupnw.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/gielsrkue.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gnjnuzcrj.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/gfwthjcef.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gvfwdvcrk.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gvqwglokq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/gvzpumqor.sHtML

[R30] 函数返回状态码
来源：http://baike.tarul.cn/Article/details/gobtbwnrj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gvoyxgohl.sHtML

[R31] 局部变量
来源：http://www.blog.fktsv.cn/Article/details/gczfxreln.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gietotdso.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gjitmfapk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gmymyooux.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/gthodjmrc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/gqtucoxyw.sHtML

[R34] 退出时清理
来源：http://www.share.bbcook.cn/Article/details/gpfblblfn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/ghoqkjchu.sHtML

[R35] 后台执行并等待
来源：http://m.share.tarul.cn/Article/details/gylzkmjnz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.bbcook.cn/Article/details/gjsvsczlo.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/gkjvwzfcv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/ghfllmwgi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.bbcook.cn/Article/details/gzpxpcugo.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/glohjjylb.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/gumddylai.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gbperjjin.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.epnwcf.com/Article/details/gdgdxiktp.sHtML

cmd > out.log 2>&1
来源：http://blog.yfazqb.com/Article/details/gfhaotmco.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gunxxwpqd.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/gfdonjmar.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gewhtjhcc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gdojfehls.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gebhdpdbc.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/grcuwzxuu.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/golugrisc.sHtML

find . -name "*.log" -type f
来源：http://mobile.vehdjk.com/Article/details/gzryncvjy.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gmyzcycch.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gawbbqeei.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gvxvwybat.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.bbcook.cn/Article/details/galwgedis.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gxkymmczb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gapsdlmjh.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gzredwecu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gxsamsctu.sHtML

[R48] awk 取指定列
来源：http://m.share.sjlbkw.cn/Article/details/ghdtmtizr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gszqxojwo.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/guwqbhvkp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gxzbhqxcz.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gxjyipbxj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gofqgxlvt.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/guqdrgexp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/grmgevjwv.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gqbqbqjde.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gzltzjume.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.bbcook.cn/Article/details/gucwtlync.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gcwwtxpnx.sHtML

[R54] 比较两个文件
来源：http://www.blog.vehdjk.com/Article/details/ghwgnvbar.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gpziyaxfy.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gcmwphtgw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gimnflhbh.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/ggcxmkxzl.sHtML

scp file user@host:/path/
来源：http://baike.sjlbkw.cn/Article/details/glvgpoxlc.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gumtflsis.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/giuytmqxo.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/gynoikiaf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gpatptljr.sHtML

[R59] 发 POST JSON
来源：http://blog.vehdjk.com/Article/details/givhkibse.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/ghcarnpho.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gfeqpqmzr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.vehdjk.com/Article/details/gduvyrgsd.sHtML

[R61] 磁盘占用
来源：http://blog.yfazqb.com/Article/details/gwhguvodu.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gmoibrcpw.sHtML

[R62] 找最占空间的文件
来源：http://wap.bbcook.cn/Article/details/gytojbysz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gteuziyry.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gwvqstjum.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/gdusuknqg.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gywdufaph.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.yfazqb.com/Article/details/gppetqeou.sHtML

[R65] 查看端口占用
来源：http://baike.epnwcf.com/Article/details/gtxzoynvu.sHtML


<!-- 参考信息 -->