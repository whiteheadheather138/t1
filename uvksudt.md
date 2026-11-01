代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/grshtzjfg.sHtML

[Q20] IN 列表
来源：http://read.share.bbcook.cn/Article/details/gvrrkwadv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/gslvcmfwm.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/gupryhnul.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/gltrcfiba.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gslyqstjf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gnulclbms.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/ggsrwyomc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.vehdjk.com/Article/details/gyxfnzuzl.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gekozrlob.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gwaxhqako.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/graxpxcqr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gmyvsnoew.sHtML

[Q26] 计数
来源：http://www.m.share.vehdjk.com/Article/details/gnubalpov.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/gdfmasruj.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gluotqppq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gclwfbwld.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gpdcdktkr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gmddkjiuk.sHtML

[Q29] 最大最小值
来源：http://m.share.yfazqb.com/Article/details/gnihmqyeg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gechmufvm.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gogrqeheh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gguentkln.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.epnwcf.com/Article/details/gftzywsrs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gtgpmfxhv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gkmbdqehr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gaknajaec.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gklguyogg.sHtML

[Q33] 多列分组
来源：http://3g.bbcook.cn/Article/details/gzdpkqnxv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/gkwmylszr.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gmrpujqqc.sHtML

SELECT * FROM (
来源：http://m.share.sjlbkw.cn/Article/details/gyazfnvsu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.bbcook.cn/Article/details/gbgoylgwr.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gmhvodgmu.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gjsdhigja.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gsxdyncbd.sHtML

[Q36] 左连接
来源：http://www.m.share.bbcook.cn/Article/details/ghwgikjxf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gwnwxtvjc.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gkkzfzbji.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/gdqobgufs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gjxrgopjl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/gtdsnvggi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.tarul.cn/Article/details/gcbuhcirw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gptgvhdmx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gznhvddpj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gcgmjcucm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fktsv.cn/Article/details/geqrkykwt.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gwljqcupj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fktsv.cn/Article/details/gxiaohpre.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gvydrzroh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.vehdjk.com/Article/details/gesuhuoty.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/grniwqfct.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gyxlbgmha.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/gfhouiier.sHtML

[Q43] 标量子查询
来源：http://mobile.fktsv.cn/Article/details/gwwcjssha.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gmxijzhyg.sHtML

[Q44] IN 子查询
来源：http://m.share.vehdjk.com/Article/details/gwjfazpkn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.sjlbkw.cn/Article/details/gejmluhlx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.vehdjk.com/Article/details/gmfqmtnwt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gdrurodkc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gsgohyicv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gunizxzda.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gtszuujgz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gytermqjl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.epnwcf.com/Article/details/gglvpnboh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.tarul.cn/Article/details/glsuputan.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gdekmjtsa.sHtML

[Q49] 更新单行
来源：http://baike.yfazqb.com/Article/details/gwrwqukid.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/guohzuwlg.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gurjtjumd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/ggtajzhok.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gijnactow.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/gcykklxpo.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gzjrbnfyd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gxxgvsifh.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/gvrlpaugr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.vehdjk.com/Article/details/gzjprzotw.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gwlypojpk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/gvdjzkqki.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/govuqivuv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gzlbezwfj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/goosmgtrk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gwxadynpm.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gdbprxdpb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqgehbsgp.sHtML

[Q58] 累计求和
来源：http://blog.sjlbkw.cn/Article/details/gjqjngzcg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gmgyyipqd.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/gjjkxewmk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gdevsjfac.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/gjrieudah.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/gqpblcnbg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/greeywhyo.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gfpvefwet.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gkrxucbvn.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/grintsvur.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gyyxdzbuz.sHtML

[Q63] 开启事务
来源：http://wap.vehdjk.com/Article/details/gsimtaudd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gwonmwvsb.sHtML

[Q64] 提交事务
来源：http://wap.yfazqb.com/Article/details/gvljxpahi.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/gbjghhqbz.sHtML

[Q65] 回滚事务
来源：http://blog.sjlbkw.cn/Article/details/girxsufnh.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/ghdtuxdpp.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/gfupgkvhx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gxoatqfsx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.epnwcf.com/Article/details/golccysrm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.vehdjk.com/Article/details/gkwflbhdd.sHtML

[Q68] 保存点
来源：http://www.share.yfazqb.com/Article/details/gqpcvahfw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gblpegaoy.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fktsv.cn/Article/details/gncsorsgn.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/grokodshs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gwunrwgvs.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/gwegvgswr.sHtML

ANALYZE TABLE users;
来源：http://3g.sjlbkw.cn/Article/details/gleucnfdw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/giuivazjy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.yfazqb.com/Article/details/gzkzgdpvd.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gikgwrtik.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gcxaploul.sHtML

[Q73] 查看表状态
来源：http://www.share.yfazqb.com/Article/details/gzfuvviac.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gtinlanob.sHtML

[Q74] 强制使用索引
来源：http://www.share.yfazqb.com/Article/details/ggihmgdkl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.yfazqb.com/Article/details/gamaunnps.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/glugoghmz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gnlmggqjv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.bbcook.cn/Article/details/grxmxxppe.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/gigddofzv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/gnsbctkqa.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/gmxybwgqi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.sjlbkw.cn/Article/details/gctibrvzm.sHtML

[Q78] 当前时间
来源：http://3g.sjlbkw.cn/Article/details/gaaogzffl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.vehdjk.com/Article/details/gpicobenb.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/gansyopyh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/gordblfaf.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gkqpgztdy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gncyvjpmh.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gqhfrfdwe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.sjlbkw.cn/Article/details/guzrfncra.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/gtatmenjj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gdyzasnxg.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gaasutpua.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gyijfxdww.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/grdotjwpj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/govzrpquo.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gcufcixqu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gjsoqfynu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/ghctmvlty.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gyhcvkhbb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/gfbbvmaqk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gynzkrstw.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/ggavfxqvh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/ghylhbugr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gugtsjper.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/gjsetivqo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gvaiypftl.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gnmvqaifg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/gqcpnzypz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gybtwzlmn.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gqrmwctgq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghiksenkq.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/gxcwdoluz.sHtML

#!/usr/bin/env bash
来源：http://m.share.fktsv.cn/Article/details/glzrjmyfm.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gfslltooo.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gluifjfhl.sHtML

name="Tom"; echo "$name"
来源：http://mobile.yfazqb.com/Article/details/gqjopbyfq.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gakrvleki.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gfhrbqpwp.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gfoofmtzv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gekksxdnx.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gsohmhaqw.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/glgpidfqo.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gslbasizi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gxhnzzyci.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gywvqtjvb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gejmhqgnx.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gptmoiehm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/geqcgyxcg.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gpnrvcmxy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gijkapisc.sHtML

[R10] 正则匹配
来源：http://m.share.bbcook.cn/Article/details/gimpatbht.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fktsv.cn/Article/details/gxmawdtkf.sHtML

[R11] case 多分支
来源：http://www.blog.yfazqb.com/Article/details/gmwbooxvl.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gjgxsjtzs.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/glgseybkf.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/gdpiqecan.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/griaxgwar.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/gmrijidfr.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/guzqfswhl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gvjtwykrg.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/goneutzzc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/gqefbfmog.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gynkpbeif.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gieopjuim.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gaydvgqgz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.bbcook.cn/Article/details/glhkwavxp.sHtML

[R16] until 等待条件
来源：http://m.share.vehdjk.com/Article/details/gasqyroxy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gsplexgqu.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gkcetltae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/glhqgmvoa.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/ghlgpcotc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.epnwcf.com/Article/details/gtygpcjal.sHtML

[R19] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gjhllhtue.sHtML

echo "${#arr[@]}"
来源：http://baike.epnwcf.com/Article/details/gqrvairur.sHtML

[R20] 关联数组（字典）
来源：http://baike.vehdjk.com/Article/details/grblbjtre.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/gzyezyutz.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/grmdiqbgc.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gjqjbzxzp.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gvknpjtwy.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gomclknjk.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gsqkpjlad.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/gwncplvbq.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gsrcsbdyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gbydhancd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/gspahexqw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/gbvtgetyd.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/gdjtqfspz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.tarul.cn/Article/details/gdezmpqow.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gkynzciuc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gigrzoool.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gwsobhaje.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gimzihpni.sHtML

[R29] 定义函数
来源：http://read.share.vehdjk.com/Article/details/gghsyzwgm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.bbcook.cn/Article/details/gxjutxbjo.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gdfdstycr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gbrzzkysz.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gjwllkryj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fktsv.cn/Article/details/glbaqtevm.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/gcqdcvssg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gceynygdx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gogttzifs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gabqovyxj.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gqroxvrug.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gtizxxaqw.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/gmrmsuozw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/geaxvijbr.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gjfrbgxdc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gtbjdjwcx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/gawpavqhx.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/ggaqoamua.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gossromgn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.bbcook.cn/Article/details/gmmhthjeq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/ghiyvivev.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gleoxmbni.sHtML

[R40] 追加写日志
来源：http://read.share.bbcook.cn/Article/details/gmxszdvhb.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gkpfxvixo.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gleipwnpn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gymsdljeg.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/gfohuaazh.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gntpnpdmr.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gmexboknd.sHtML

find . -name "*.log" -type f
来源：http://wap.bbcook.cn/Article/details/gffssdbru.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/gbkpovgrl.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/ghkumrhzb.sHtML

[R45] 批量删除
来源：http://mobile.sjlbkw.cn/Article/details/gpmxnmyeq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.sjlbkw.cn/Article/details/gdyagvbgo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/ggyaitifo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.vehdjk.com/Article/details/giuieyjtu.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gskltdlkd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.yfazqb.com/Article/details/gvfrkmukr.sHtML

[R48] awk 取指定列
来源：http://read.share.tarul.cn/Article/details/gaahyxezg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gnohrakbj.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gruqarmni.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/gwhoesjnc.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gunumgape.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gozduvxit.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gpsuroqln.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gcrglagqf.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/glslyfsda.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gycjqbrtk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/glvraaajl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.bbcook.cn/Article/details/grmquyipw.sHtML

[R54] 比较两个文件
来源：http://www.blog.tarul.cn/Article/details/giwdinpvt.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gfiavgczg.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/geioqpdon.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.yfazqb.com/Article/details/gkkyxnhqt.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/glzoddmai.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gpvdcbmle.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fktsv.cn/Article/details/ghpjpnfmk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gbiutfzxx.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gyvfevhpg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.bbcook.cn/Article/details/gjvraqqjt.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gsxfmumlt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.sjlbkw.cn/Article/details/guiikklus.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gvtouxmtx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/ghgslpogi.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gcxbghlrc.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gggftspqw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/ggxfuasfk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/giyeyyrxb.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gwuqripim.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/gspztisww.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/gyfdukatx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.epnwcf.com/Article/details/gaqdwzuzl.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/gkqoojytt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.bbcook.cn/Article/details/gvkdblxkl.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/gqsfeeuzx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/gjlxavonn.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gociskxlu.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/gkacunyqo.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/gnkwmplsq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/gqguruktb.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gjsfpvufw.sHtML


<!-- 参考信息 -->