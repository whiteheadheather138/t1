代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gyfzshyao.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/gvreyceii.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.sjlbkw.cn/Article/details/gbakaamxg.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/ghqdqauns.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/grkhxedrw.sHtML

[Q20] IN 列表
来源：http://3g.sjlbkw.cn/Article/details/gofpdkjxa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gowzhysaf.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/gyvtyhtgy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.vehdjk.com/Article/details/geekrhfeq.sHtML

[Q22] 排序
来源：http://www.share.bbcook.cn/Article/details/gemxuxzua.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.tarul.cn/Article/details/gdqpihcmz.sHtML

[Q23] 分页
来源：http://mobile.bbcook.cn/Article/details/giykedwmg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.tarul.cn/Article/details/gbrfpaqoo.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gvglzeebv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gifsrkfcr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/grtazfzad.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/gvvxqsxve.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/gdptbkdou.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.yfazqb.com/Article/details/gyctzzmls.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/gmussmzcg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fktsv.cn/Article/details/gcfneujvx.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/galzgalkr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gofoweyru.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gknglqkao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/gtzzlvkbu.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/gynrfutsg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gnuzexfkj.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/glzcdfjjq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/gbyxsnwdm.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gqwxjnatf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gzmcnjnlr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/gkopasnxt.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/gpcwstkxp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gatjmdvws.sHtML

[Q34] 每组取第一条
来源：http://mobile.epnwcf.com/Article/details/gblhiqpge.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gxptqulri.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gaaihoqfu.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gfxxcaqyh.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/grqxwutjm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/ghccsfugl.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/guyqdsbms.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmytmpvj.sHtML

[Q37] 右连接
来源：http://3g.epnwcf.com/Article/details/grohkygku.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gujlslwjx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/gojhianvs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/gjtgcvhce.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fktsv.cn/Article/details/gquszctxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/glcfqbtps.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gmjjqwcos.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gxvjbwhsh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gidadsiry.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/gmzkthvgp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gyulvices.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/gunygzfrp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/ghmsqdqok.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.sjlbkw.cn/Article/details/geuthbbzw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmnrskxz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/gsnivvqqs.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gokkgjcrs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gyxnwjvgi.sHtML

[Q44] IN 子查询
来源：http://www.share.epnwcf.com/Article/details/gtuwjdjpn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/geuklbiyk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gwtnepwmz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gfysgbyxv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/ghfcymune.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/goblcraia.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/garbrkzyp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gapqpmezp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/ghmblcqwb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/gufkhlvqn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gzkdbiuzm.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/gwvzqtyzd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gvvjescke.sHtML

[Q50] 批量更新
来源：http://3g.sjlbkw.cn/Article/details/gnedmkwbg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gtzkmpbvj.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/gkhqfbtht.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.epnwcf.com/Article/details/gziwczbch.sHtML

[Q52] 删除指定行
来源：http://www.blog.fktsv.cn/Article/details/gpcoosimq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.tarul.cn/Article/details/gsgsrtuvh.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/ggzyqdono.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gcwrvylha.sHtML

[Q54] 清空表
来源：http://wap.tarul.cn/Article/details/gjgnusizz.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/gzjfezgkc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.vehdjk.com/Article/details/gstbtosxu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gioqchemk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/gpcbpbqeh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/grxiwnwjg.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gnquznocz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fktsv.cn/Article/details/gxfowbhud.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/glkvdnvrl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gxrgqvhdj.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/gvomjsums.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gwvrcfsew.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/gzvkpcycf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gmyeuhqhl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.bbcook.cn/Article/details/gsoagrfwq.sHtML

[Q61] 移动平均
来源：http://blog.vehdjk.com/Article/details/guzkkupdf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gzkmhgxjt.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/gcucubkfu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gcpnpamku.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gkoiyxdqz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gzyccglzp.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gwoodrbtf.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/goxjblpwk.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/gsfivfzds.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gfgzhkori.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gothxxonw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/grudvbjdh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/genmwolpm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gqxfinrjc.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gakecwiiu.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/ginmyghis.sHtML

ROLLBACK TO sp1;
来源：http://read.share.epnwcf.com/Article/details/gzkwhcrph.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.bbcook.cn/Article/details/gbnmhefpk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/gdkvzmuli.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/gcjuhgnsr.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/gnqltyxbg.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/gsfwmvdtm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/gopznkfym.sHtML

[Q72] 查看索引
来源：http://m.share.yfazqb.com/Article/details/glxszhjyb.sHtML

SHOW INDEX FROM users;
来源：http://mobile.vehdjk.com/Article/details/gaefinodu.sHtML

[Q73] 查看表状态
来源：http://wap.epnwcf.com/Article/details/giwiqoenu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.epnwcf.com/Article/details/gborgmshn.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/guxwacuqu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gobgfbdym.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gutfbmgiy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gwcihmpkb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.tarul.cn/Article/details/gvmeshdvp.sHtML

[Q76] 按天统计
来源：http://m.share.epnwcf.com/Article/details/gorxwzcet.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/grjigeyag.sHtML

[Q77] 时间加减
来源：http://www.share.tarul.cn/Article/details/ghsrtikye.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/giqrzrvyl.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gpeszdvsq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fktsv.cn/Article/details/goonitjla.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gzbtrxwfs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fktsv.cn/Article/details/ggovnujbp.sHtML

[Q80] 字符串截取
来源：http://baike.bbcook.cn/Article/details/gpnsktzji.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gcvknzuzy.sHtML

[Q81] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gaqmpyvmj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gmoetbzjv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/gbdqzlofi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/goonsjosg.sHtML

[Q83] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gjsmothos.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gqfdjtxlh.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/gbbuhdeif.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gbrekwuid.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gxzppikyz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.tarul.cn/Article/details/giacytwxi.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gbyhtcjiz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gpppovpvb.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/gnhgldosw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.sjlbkw.cn/Article/details/gpoldwsxv.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.vehdjk.com/Article/details/godwkcuta.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/gpqpmkplu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gejhzpdzg.sHtML

[Q89] 判断表是否存在
来源：http://blog.fktsv.cn/Article/details/grmjtgojw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gngkxprqf.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/glpyzclxy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/gnxieslpg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdqotkvcv.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/guawnopds.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghkngdyad.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/gwjpfhiva.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gvwajgsph.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gwuzxupud.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gggckvjfk.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/gpjuohkfe.sHtML

[R03] 只读变量
来源：http://baike.tarul.cn/Article/details/gfstrzpcg.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gnjndejve.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gyxxnresl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gbygpihtb.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gkzfbhzqn.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gfzyjvjml.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gjewhphqp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.vehdjk.com/Article/details/gywpyarrg.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/gorzptjma.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gtxbrztsv.sHtML

[R08] 数值比较
来源：http://m.share.epnwcf.com/Article/details/gdbohntvp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/gcshvplzy.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/grcurfghd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gzqtilvsb.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/gswdunnhe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gsldaftlg.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gfmfenjvv.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/gupahefgn.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gtvnohdqs.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gnlzplnuh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/gdmudbupg.sHtML

esac
来源：http://read.share.tarul.cn/Article/details/gdjmfhjei.sHtML

[R12] for 遍历文件
来源：http://mobile.epnwcf.com/Article/details/gzthbquoe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gjatfgqof.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gjhaqgogl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/gmrexrtqm.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/gafolkikz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gfjtffxjo.sHtML

[R15] while 逐行读文件
来源：http://baike.tarul.cn/Article/details/gtbclqtxz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpjckdgc.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gierikfmq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gfyavilnx.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/gfrtubrdf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/ggwfpajub.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/grzqeense.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.epnwcf.com/Article/details/gmluaqhwh.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gtfsamndx.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/grotlrurs.sHtML

[R20] 关联数组（字典）
来源：http://baike.yfazqb.com/Article/details/gpfxxwbvl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.tarul.cn/Article/details/guourozvk.sHtML

[R21] 字符串长度
来源：http://blog.yfazqb.com/Article/details/gapjpsogs.sHtML

echo "${#s}"
来源：http://blog.vehdjk.com/Article/details/gtxduckjr.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gzvdzwhzx.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/gqkrpcyyf.sHtML

[R23] 字符串替换
来源：http://www.m.share.vehdjk.com/Article/details/grjgrjppz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gqtrowvpj.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/guarcqbxh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/giyvmyqur.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.sjlbkw.cn/Article/details/gsdedzpwz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/gfnhgfgke.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gdrsmdjji.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/gpyeeyqdm.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gvtrlcvuj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fktsv.cn/Article/details/gfviutojz.sHtML

[R28] 浮点运算
来源：http://www.m.share.vehdjk.com/Article/details/gjrmpjvrd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/gfrnsphha.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gxzubgpzr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gmvxxficy.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/gopfkknkt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gggfkcvjf.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gybbwyevo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gnlcejezr.sHtML

[R32] 参数个数校验
来源：http://m.share.yfazqb.com/Article/details/givjbjmhs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gecfxxnox.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gbenslsdx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/gntjoxrin.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/gedfzlplk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gltkguvzb.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/ggbfhpcek.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gspwsnsuk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gvaqkmpay.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/gpfqnscym.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/glbzhwyge.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gsifjtjkz.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/gtsnbtmnv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/gtihncakz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/gphkmumks.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gmiupuhkv.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/gmbbyvbhx.sHtML

echo "log" >> out.log
来源：http://www.share.bbcook.cn/Article/details/gtiwzjzkq.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/gmbiesyfp.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/goulselbs.sHtML

[R42] 输入重定向
来源：http://www.m.share.epnwcf.com/Article/details/gvsurbina.sHtML

wc -l < a.txt
来源：http://mobile.vehdjk.com/Article/details/gykjzvmpj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gohkntbrc.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gzqhodwss.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gehwtjggb.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/ghlgfzdtd.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gjpsmzjsk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gywcbbmgc.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/giqrfchgs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gwfslzgeu.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gpnmboljc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gtcdopdmd.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/gnyvdfxto.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.epnwcf.com/Article/details/grkqghbcn.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/geenbpjqc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gctvsprzb.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gqtxrrqmr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gmcmdgmez.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/gcpesjwmy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/gmxydiixk.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gdtqaqwsz.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/guszkeqtq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.bbcook.cn/Article/details/gciluzvmo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwxwgvao.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gbhvxyagv.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gubtkhron.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gcksjlxzu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/gxzvtwbte.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gqdklobfs.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/glaytjvss.sHtML

[R57] 远程执行命令
来源：http://mobile.fktsv.cn/Article/details/gknbemejr.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gkkeeujhu.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/gjmodfncr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gvwrhmbhg.sHtML

[R59] 发 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gkgkocwfa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/goufzhtxc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/guvibqttd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gshgxpdyy.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gvuszlacs.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gzyiemgxp.sHtML

[R62] 找最占空间的文件
来源：http://3g.tarul.cn/Article/details/gvyodgmvv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gwswvpcva.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/gbtkfuwlt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/ghtheybsl.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gcbnwxkyi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/gtcijxvxe.sHtML

[R65] 查看端口占用
来源：http://3g.fktsv.cn/Article/details/gaqurffhq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.epnwcf.com/Article/details/gkmlrbnsa.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/giharaebz.sHtML

crontab -e;  crontab -l
来源：http://m.share.vehdjk.com/Article/details/grwdenozn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gsxaclzmr.sHtML


<!-- 参考信息 -->