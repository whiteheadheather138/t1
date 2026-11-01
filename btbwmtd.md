代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fktsv.cn/Article/details/gfbhqorca.sHtML

[Q26] 计数
来源：http://mobile.tarul.cn/Article/details/geaxtwykv.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gxulmewft.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gdzynhkun.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/grqvewmso.sHtML

[Q28] 求和与平均
来源：http://m.share.sjlbkw.cn/Article/details/gsacsfipi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gxfkbubqt.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gfzobirgc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gtozdhxzk.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gzbzbomrd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gwzvjbxjz.sHtML

[Q31] 分组后过滤
来源：http://blog.epnwcf.com/Article/details/gdyzpstsd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gulzkufiz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.epnwcf.com/Article/details/gyrvmgnyc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gpbwcfern.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/gmtzsqsif.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/gkyxgfepx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gssmaezqc.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gurnnuwft.sHtML

SELECT * FROM (
来源：http://www.share.vehdjk.com/Article/details/ghifyvcfb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.tarul.cn/Article/details/gghjneegf.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gnbujwiep.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gjwmtlhoy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/grazsvzew.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/ghtqsslim.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gtmteghie.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/gzlajccyh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/giklfkvrs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gjzcejwpw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gjljrtjll.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gdlqsuvko.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/goapdzqtp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.yfazqb.com/Article/details/gzvyyukxw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/gltndshzj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gsgxrtgkg.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/giaudqksv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gluquafwp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gydmsujck.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.vehdjk.com/Article/details/gvdmqrlbu.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.bbcook.cn/Article/details/gwwixraih.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.bbcook.cn/Article/details/glxhejwsn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/guayixgbq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjgumicp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gxwqjngmv.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/gitbighax.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/gymwheiit.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.vehdjk.com/Article/details/gpdptyspc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/grmedpccs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/grsvulsxd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gzuibrrpm.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gklwbrtwi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/ghidexvaf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/gihhrcthc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.yfazqb.com/Article/details/gcpcincuj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gajmkmjjp.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/ggguthmao.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/guyhlbglr.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gfenxtbag.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gaaftmhsf.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/geebcdsja.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/grdpizyni.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gbdpauzum.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/guruouetf.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/gwyumdlap.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gjgjhasca.sHtML

[Q54] 清空表
来源：http://www.m.share.yfazqb.com/Article/details/gpjmzykhy.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fktsv.cn/Article/details/gcfkystcr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/gtighugvb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gtcmmlwoe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/glzwopgnd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/gtpqfoooj.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gsealkdmi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gkktndqcv.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gzzzmhbni.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.tarul.cn/Article/details/gekklmzdw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gtmqfpgtr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gzmcpjjce.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/gitfetulz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/gejkxsbfa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/ggpojcetf.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/gamrnezul.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/gqqqtjwle.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/gtagrxhah.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/guwocclti.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/gpkjcjtdv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.tarul.cn/Article/details/gjmgpqkbq.sHtML

[Q64] 提交事务
来源：http://read.share.fktsv.cn/Article/details/gjonbvczu.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/godwrcqnm.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gkbsxjylk.sHtML

ROLLBACK;
来源：http://mobile.yfazqb.com/Article/details/gejhyxsvc.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gojlwbdfx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gsldrzabh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gvdbzympq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/grkgvugdc.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gluryaunj.sHtML

SAVEPOINT sp1;
来源：http://read.share.sjlbkw.cn/Article/details/geekbsxgb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.tarul.cn/Article/details/ggcfozmcw.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/gogbfyuae.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.vehdjk.com/Article/details/gzwezczpk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gzgfqpvfm.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/goiaviqhm.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/ggqseohyl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.sjlbkw.cn/Article/details/ghczzglbg.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/gpbhersfa.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/goqgozdxd.sHtML

[Q73] 查看表状态
来源：http://www.share.yfazqb.com/Article/details/gyjyklwqw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.epnwcf.com/Article/details/gfrvtimpk.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gnajiykmv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gsqxvyzlj.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gnonsgqlu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gnxbwnske.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.yfazqb.com/Article/details/gdqrarjmi.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gylzugpxg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fktsv.cn/Article/details/gbpdplvqu.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/gipqcfzkn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gnknheanb.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/ggkpihrfs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gmkygkwbm.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/gmqskxzuo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gepqndkjh.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/gclvccjre.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/glaliffqd.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/ggvuukapj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gufnbdyjv.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gvexixzuk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gywqxchox.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gahfozojz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/goykwvmxz.sHtML

[Q84] 去除首尾空格
来源：http://blog.epnwcf.com/Article/details/gmyrlegvb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gdadgouan.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gysihmzbg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.bbcook.cn/Article/details/grtfjjldr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/gkhcxlocm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gutqfqlav.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/ghvjgrdfx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.tarul.cn/Article/details/gurikoxxg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/gwejryymh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/gwzqwkxkw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.yfazqb.com/Article/details/gqfaplyuo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.yfazqb.com/Article/details/gxatxqgjm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/gdtrrpyhn.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gfvprmoac.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/gnpksnsqd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ghkyrdqcl.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gllhcqwtj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqmorxjcc.sHtML

[R01] shebang 与严格模式
来源：http://blog.fktsv.cn/Article/details/grxhysldy.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gvcjyvgcq.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gnjryuhsf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.bbcook.cn/Article/details/gglttekhl.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gaiujmqsk.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gvgckamwv.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/guakddjry.sHtML

[R04] 位置参数
来源：http://www.share.fktsv.cn/Article/details/gqfhrnthy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/gzllydclk.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/genvqpeym.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gzbigtuss.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmhtwyzs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyfxwmmo.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gxqqwregi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/glsesmrry.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gykdutefn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gkwncdkvy.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gmifvrffk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.bbcook.cn/Article/details/gcfyjbhrs.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gtvhmkerv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gmhjicmne.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/ghszehxqu.sHtML

case "$1" in
来源：http://www.m.share.vehdjk.com/Article/details/guoczklkp.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/gkclddaep.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gmpkwhiff.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/ghbcjcsmu.sHtML

esac
来源：http://read.share.sjlbkw.cn/Article/details/ghzsbjujh.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gwjojodov.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gjuspgmhm.sHtML

[R13] for 计数循环
来源：http://blog.epnwcf.com/Article/details/ggcjtpxqp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gnuolbgvc.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gsvjkwsdu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/guuezfyeg.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/geppomqdo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/geecllvdm.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gmpbvowle.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gjoybalub.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gjgmkmcpf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gswtznpsz.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/gjtwgtceg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.vehdjk.com/Article/details/geuyjfopl.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/gjgvlsvxs.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/gxgseixis.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.tarul.cn/Article/details/gqrprsxlg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gyyusejnv.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/gylyrixqs.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gsxxgqtth.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/glqjzywmo.sHtML

echo "${s:0:5}"
来源：http://www.share.epnwcf.com/Article/details/govsfffth.sHtML

[R23] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gbmrpiykw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gggudhvsg.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gjmuvwklg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gsjfbhlsi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.sjlbkw.cn/Article/details/gfpqbssbb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gjpdecsom.sHtML

[R26] 命令替换
来源：http://www.blog.tarul.cn/Article/details/gysrmkapa.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gjoibwmvs.sHtML

[R27] 算术展开
来源：http://blog.tarul.cn/Article/details/gfzmjoamb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/grmpntnun.sHtML

[R28] 浮点运算
来源：http://blog.vehdjk.com/Article/details/gsjxosskf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gihjzlbqk.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gwguigmyk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gbuyppjiq.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gatqjemqd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/gkevvkffu.sHtML

[R31] 局部变量
来源：http://www.blog.fktsv.cn/Article/details/grqjtbkhj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/gnqhnwwbc.sHtML

[R32] 参数个数校验
来源：http://mobile.vehdjk.com/Article/details/glsoubiul.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/grafvukkn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/gbnwthfld.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.vehdjk.com/Article/details/gpkwutcbo.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gpcfzjsah.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/glvllhmsb.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/goutlhivh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gkrtgkqyc.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gausposke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.tarul.cn/Article/details/gjugvknik.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/ganiccgjq.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/gdbsdymjj.sHtML

[R38] 管道串联
来源：http://m.share.fktsv.cn/Article/details/gpfddohgl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/ggfexuiex.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gbfutliao.sHtML

cmd > out.log 2>&1
来源：http://m.share.yfazqb.com/Article/details/gcyjozvwp.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/gottkksxh.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gsthyrase.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gryjlqiaz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gevfwxzte.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gmwbjursq.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gjxhweigo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gobaqjmpt.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/gdxniydgw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gukyfucme.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gwfpceipp.sHtML

[R45] 批量删除
来源：http://baike.epnwcf.com/Article/details/gxxufyway.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gvrqsdmfz.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/goltmkles.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/gaixntqgv.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/gssxllqfm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gihvtacgb.sHtML

[R48] awk 取指定列
来源：http://read.share.vehdjk.com/Article/details/gwkacmihx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gfsplkips.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/gyeiuqqqf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/gozoqomdn.sHtML

[R50] awk 求和
来源：http://baike.yfazqb.com/Article/details/gumbsyxza.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gnmotapcp.sHtML

[R51] 排序去重取前几
来源：http://blog.epnwcf.com/Article/details/ggyuixuhy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gloqfnjmq.sHtML

[R52] 统计行数
来源：http://www.share.fktsv.cn/Article/details/genfyqvra.sHtML

wc -l a.txt
来源：http://www.m.share.tarul.cn/Article/details/gmqoqzufu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.yfazqb.com/Article/details/gsgmosdhb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/ggqkavlco.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gldaubtgp.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gtjjgqswr.sHtML

[R55] 压缩与解压
来源：http://www.share.tarul.cn/Article/details/gzqcqsxxk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fktsv.cn/Article/details/genopkunq.sHtML

[R56] 远程拷贝
来源：http://wap.sjlbkw.cn/Article/details/gpcfyqzqr.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gaiqyvbwc.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gqudwnldl.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.epnwcf.com/Article/details/ghxivmzpz.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/gpkcmtyfy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/gyrrimpql.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gbolnecjj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gpenhbnpf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/ghywrajhq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gnlnqbivm.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gqavpcdxy.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/ggrxmchjd.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/gqrwrbxps.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gvmsgqzxa.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/ghrdfncbu.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.yfazqb.com/Article/details/glbxafypp.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/gmrljjapy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gxsapzprz.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/gyrxivsbz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gctryrsat.sHtML

[R66] 定时任务
来源：http://blog.epnwcf.com/Article/details/gxdlapqaf.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gktakfcom.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gnkwtpndk.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gqpigbwxg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gjoojwduo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gylwtvnxm.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/ghgsfcesb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gpulfopzr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/gfcigrppl.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/gxplkvthj.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/ghqirshak.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gagheeilt.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/guoojpjmk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gyzgcbbhk.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gzzgmpeci.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/giwactxjb.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gtrvjphcd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gxwgzpwpe.sHtML

[R75] 导出环境变量
来源：http://mobile.fktsv.cn/Article/details/gedifxbct.sHtML


<!-- 参考信息 -->