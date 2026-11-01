代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gdwzhedau.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/ggkytbwfn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.epnwcf.com/Article/details/golvdphak.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/gabhxconz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.bbcook.cn/Article/details/gvfkiudhy.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/ggahrcimb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.tarul.cn/Article/details/gusxjhkpl.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/gzmvdaypi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gaxzrosyy.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gzvifzuyo.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gxkokqsmd.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gpjpxlfuh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gfoxonolc.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gscsnokpr.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/glwohqjwt.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gkweyzmhr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fktsv.cn/Article/details/galkkreby.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/gmcvgsbzg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gjrxlzhmd.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fktsv.cn/Article/details/ggipphfoa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gggvpsttq.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/gyvkejsna.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gumswmaub.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gjqohiyxu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gnbzmstee.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gelrofata.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gbxqwanhl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gonzzvzlv.sHtML

[Q33] 多列分组
来源：http://www.m.share.epnwcf.com/Article/details/gyfwuqlul.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gsxpsfzus.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/gfifwpnja.sHtML

SELECT * FROM (
来源：http://www.share.sjlbkw.cn/Article/details/guiuloptv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/goibvukmj.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/gqsifuzxv.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gkwsclmuw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gxbdzujed.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gdxhuguyc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gqucudijm.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gnuyhrjnw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gzvsbvrpe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/gyayuihuu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.yfazqb.com/Article/details/gvbyfidam.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fktsv.cn/Article/details/gghnzhvpq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/geinttzbj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gfaszbiwv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gqkkypyff.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gmnowtshd.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gxposetpu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.vehdjk.com/Article/details/gcqxooffl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.yfazqb.com/Article/details/gzlmetnzk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gqzdneqmd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/gnpjuctmo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.vehdjk.com/Article/details/gstlxklni.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/gffpoyacs.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gyrlkwlzb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gsvakqdef.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/gnjmnwtjd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/gafcnnmsr.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gfbqfleuf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/ghnevcvid.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdkonhro.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gvdeiqiee.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/gahrehmoa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.yfazqb.com/Article/details/gmgapztuw.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.sjlbkw.cn/Article/details/gegppmjrp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.vehdjk.com/Article/details/ggcxaczrn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.tarul.cn/Article/details/gknmlkjil.sHtML

[Q49] 更新单行
来源：http://m.share.bbcook.cn/Article/details/glrrriado.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gdayybfnk.sHtML

[Q50] 批量更新
来源：http://3g.tarul.cn/Article/details/gfwpkrkby.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gkkvhqqzo.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gvmzzpmzz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.tarul.cn/Article/details/gzavcvjnu.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gcgtjhoyl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gvatfhdeq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gpltxnwqf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/gacxkjgaz.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gljblfrnq.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/gvnyczmry.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/gcuzpdcqf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fktsv.cn/Article/details/gwqmngkqq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gpblhtbov.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/grspwabov.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/guylxctee.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpxcnesrv.sHtML

[Q58] 累计求和
来源：http://wap.bbcook.cn/Article/details/ggyrkjtwt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gseerewpf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gkpugwrrd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gkvdcswrm.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gamfrzhlc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.tarul.cn/Article/details/gmrkmmfyh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/ghhbiekdb.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gzejuerxx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gqwinlkcp.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gchgacqbf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gmheuotwd.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gkiopgxso.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gtollmevv.sHtML

[Q64] 提交事务
来源：http://baike.yfazqb.com/Article/details/gnmtfkuri.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gmhnbbwff.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/gcpmdypfu.sHtML

ROLLBACK;
来源：http://www.blog.sjlbkw.cn/Article/details/gcmcrihab.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/glsfjvejz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gybfheuis.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/gwyrcegge.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gcgtlnltd.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gzljlnjrc.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gvyjzvqks.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/grhchyolf.sHtML

[Q69] 查看执行计划
来源：http://wap.bbcook.cn/Article/details/gycwsotxk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.yfazqb.com/Article/details/gytdbbyvw.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gpzfnypry.sHtML

ANALYZE TABLE users;
来源：http://mobile.fktsv.cn/Article/details/gowxxeytz.sHtML

[Q71] 查看建表语句
来源：http://3g.fktsv.cn/Article/details/gcljrcrus.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/gyeqhmkgu.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmvszhlo.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gjmqbhpag.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/glvmblfat.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/gvreoulwb.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/gqpbaqtzo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/gihvubxnl.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/gzzbnzzty.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gvekqdjfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/gvbasciyl.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/glskebslw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gviltluqd.sHtML

[Q77] 时间加减
来源：http://baike.sjlbkw.cn/Article/details/gzhoniyoo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.vehdjk.com/Article/details/gwmvqoafy.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gjdcmclco.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/gjlblmgdv.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gcqjftees.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gaoscigak.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gdnwulfsm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gznfmggqv.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gtdyvfghb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/ghaqdaqdx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.bbcook.cn/Article/details/gqpbebtth.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gkjvagnds.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gctxsptaz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/grftzfyip.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gsxpxaolp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gvfdaixug.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gmbjrkrzp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/ggsjluchu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.bbcook.cn/Article/details/gzmytnygy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.bbcook.cn/Article/details/gyuzppkzs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/glbwzqffm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gpchrvkbc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/glsxosgni.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gjgeidnvc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gftambxpc.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/guiwtgdwd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gljlbooxg.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gwbnrhztd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gvcyfnwaj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzhvvhyfb.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/ggydoqqgi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gditywmbz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/goswnfdpr.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/ghcakwogs.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/gyrgtqskk.sHtML

[R02] 变量赋值与使用
来源：http://blog.epnwcf.com/Article/details/gyayveecf.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gypjztbhd.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gyvhdrxst.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gjdedgols.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/ggfixrufd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/govhqtxoe.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gfpgbyksp.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/giyzusids.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/ggzhuskrr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/giuxeijhw.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gjtebthmi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gnzdfvuvb.sHtML

[R08] 数值比较
来源：http://blog.sjlbkw.cn/Article/details/gzkgftjwd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gpeduasnr.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gkixximlu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gdcjfcgvj.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gccuptihn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gncyquurc.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gudmzcoav.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/gshcpqtfx.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gstvkzdvo.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/gilyxsuhd.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gvhdnkyus.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/ghigcielv.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gxjsclivq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/gddnxbbrx.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/goxsxkled.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/glbtfaywg.sHtML

[R14] C 风格 for
来源：http://baike.fktsv.cn/Article/details/gkrlgavyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gfdnpeoev.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gcxolorws.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/gvmwdqmkk.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gmoeylufc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/ggstkwfbl.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gvexmlfzc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gwtlkxuzg.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/glbhtdzlb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gejkougoq.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/glujadbvb.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gagxkfgty.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/gzeeggwim.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/gmxvlrwms.sHtML

[R21] 字符串长度
来源：http://www.share.yfazqb.com/Article/details/gvaangiud.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/glsacfdmb.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gpjlopnhk.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gmvdnioxt.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gnmjfzzpn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.epnwcf.com/Article/details/gbegaiozy.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gbsrhqtmo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gkqrneiux.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/gcmyvvray.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fktsv.cn/Article/details/ghmykmmqu.sHtML

[R26] 命令替换
来源：http://m.share.sjlbkw.cn/Article/details/gpkidvdkr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gjntmrrxv.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gswshusxn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gdamoawoq.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gkewnvwex.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdzlmfju.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/gjqwtettr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/glcxdyliy.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/gwadzlqim.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/glzlrfqmt.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gzjqpwyqn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.bbcook.cn/Article/details/gpkzjwmrp.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/gopovzqcw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gunxbgopr.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/gekrimyoc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.vehdjk.com/Article/details/gacehkifm.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gxvgtowxl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/giqdinqqx.sHtML

[R35] 后台执行并等待
来源：http://read.share.epnwcf.com/Article/details/gechwzusr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gwnbzkcwi.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gxwryazkw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/gajsegppk.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/guianiagq.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/golceigdc.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/gkadetjxh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwonexdq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fktsv.cn/Article/details/gwnibllnm.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/gnallkhli.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/gbgjfjzgc.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/gozssdhrd.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/guuruefpo.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fktsv.cn/Article/details/gdsuaaael.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gagoyueij.sHtML

wc -l < a.txt
来源：http://www.blog.vehdjk.com/Article/details/gtluzkmjy.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gclvbrqfy.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gmvqcbdes.sHtML

[R44] 按修改时间查找
来源：http://www.blog.tarul.cn/Article/details/gybszeujn.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gbaezclmi.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gunzqmqxq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/geczxfoyl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/gcbrvztma.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gbnxvkthg.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/geamamavi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gvnhkgbvt.sHtML

[R48] awk 取指定列
来源：http://m.share.sjlbkw.cn/Article/details/gvhzuyfoc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gmgyysenx.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/gkonatafi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.epnwcf.com/Article/details/gowgvgsaa.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/gwhyfrlxj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gcfenoxvu.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/grvwoptwm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gcmmuvydj.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gwdowlwew.sHtML

wc -l a.txt
来源：http://read.share.yfazqb.com/Article/details/glyttpema.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/gqaelnbab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gifvoiswt.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gozskcevw.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/glqamfzcc.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gbbhochje.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/gikysrypc.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gsgmtipgp.sHtML

scp file user@host:/path/
来源：http://3g.yfazqb.com/Article/details/guarsqyuv.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/gnwaypfcv.sHtML

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/gyfdzxtno.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/gnqnipufy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gdrgbcttw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gigvplfpr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/ghlfaozsv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gpakrzamy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/gpqqspktr.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gvkaicxoi.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/gwkykdkdd.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfywifvph.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.bbcook.cn/Article/details/gxarmflvz.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gvlazytjf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/ghlmtyxjf.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/guqstxewk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gjtgrzxfq.sHtML

[R65] 查看端口占用
来源：http://www.share.tarul.cn/Article/details/gpwuairyt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.vehdjk.com/Article/details/gneigynjz.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/gkflaanbv.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gnmcbkylm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gzyqenair.sHtML

openssl rand -hex 16
来源：http://baike.bbcook.cn/Article/details/glozgrcrs.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gzvpbdnsn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gnayruljv.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gbijhzeux.sHtML


<!-- 参考信息 -->