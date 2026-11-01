代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.vehdjk.com/Article/details/gfnessjxk.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/gpnrgvewb.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.vehdjk.com/Article/details/ggcjcnwms.sHtML

[Q27] 条件计数
来源：http://www.m.share.epnwcf.com/Article/details/gsbiorcfw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/gjjfcwjnj.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/gbwkluvzq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gnxpkpuxk.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/glzlaieoh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gltcggpdu.sHtML

[Q30] 分组统计
来源：http://wap.tarul.cn/Article/details/guegobewo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/ghqjbhukh.sHtML

[Q31] 分组后过滤
来源：http://blog.yfazqb.com/Article/details/gmjgevjal.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/ghitjwndt.sHtML

[Q32] 分组拼接字符串
来源：http://wap.epnwcf.com/Article/details/greafezdh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gnafavdan.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gnszowyco.sHtML

[Q33] 多列分组
来源：http://mobile.bbcook.cn/Article/details/garvskszk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/gwmyjkyuk.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gaisptyff.sHtML

SELECT * FROM (
来源：http://m.share.yfazqb.com/Article/details/gcxwnotjo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.vehdjk.com/Article/details/gcencpnrv.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gpizgnsdw.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/gigtyycpf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gexksqiyb.sHtML

[Q36] 左连接
来源：http://www.share.bbcook.cn/Article/details/gcabovrxp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gzfhsjzla.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gykxkqter.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gtzllmyvj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/grqqvoapj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.tarul.cn/Article/details/gzbmvpwum.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/gckvwpisc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.tarul.cn/Article/details/gtgtswjaq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/gugxgocmd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/glddssevz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.vehdjk.com/Article/details/gnghbdugj.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gdisnsttx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gcsmemufz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gudishegz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/gxpivpley.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.yfazqb.com/Article/details/ghqnfnhti.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gduxpzyxc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.epnwcf.com/Article/details/gbvmmyalc.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gqoymhemd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.tarul.cn/Article/details/glnuxunlj.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/gtogsyoeb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/guxsggnzv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.vehdjk.com/Article/details/gfrvvlfbb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/ghgzlbtpl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.epnwcf.com/Article/details/gjfhgqdjb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gfmhjzgmr.sHtML

[Q47] 与平均值比较
来源：http://blog.bbcook.cn/Article/details/gkrpmjpsm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gnqzwdyud.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/ghrahswur.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.bbcook.cn/Article/details/gnvbrfhzd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/giaxrilar.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/gunqiuddp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/geyneqqpb.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gmratgvlg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.vehdjk.com/Article/details/gpvpuheou.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/gcmluwxgd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/gmhpxijam.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/gfennyzqr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/ggofhthsg.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/gktpphxgf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gwfpthmzd.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gbqlkutth.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/gdcscpypb.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/ggdmaqcdr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/gokfqchra.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.yfazqb.com/Article/details/grunwgywy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gkndvhtjt.sHtML

[Q57] 行号
来源：http://mobile.bbcook.cn/Article/details/gjddymeax.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.epnwcf.com/Article/details/gxmoatjvs.sHtML

[Q58] 累计求和
来源：http://read.share.epnwcf.com/Article/details/gaogupnox.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gtwyhjktx.sHtML

[Q59] 分组内累计
来源：http://baike.sjlbkw.cn/Article/details/gynledxzd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gilseexic.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.sjlbkw.cn/Article/details/gxfdywqie.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gbcjdtjxb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gxofwohoj.sHtML

[Q61] 移动平均
来源：http://www.m.share.tarul.cn/Article/details/goauifunf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gqsbclczo.sHtML

[Q62] 分组占比
来源：http://wap.sjlbkw.cn/Article/details/gaexwxnyy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gcjxdldyj.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/gdbwqquzv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.epnwcf.com/Article/details/gesbdzife.sHtML

[Q64] 提交事务
来源：http://3g.yfazqb.com/Article/details/gavqurmji.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/gjahnngxn.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gksdvjpnw.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gbghwxsio.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/gmrgexzfu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/gfgefoxkd.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/gdzbqwfni.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/geowliyft.sHtML

[Q68] 保存点
来源：http://wap.yfazqb.com/Article/details/gwxupegab.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gzjooorpq.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/gcwauxneu.sHtML

[Q69] 查看执行计划
来源：http://www.blog.epnwcf.com/Article/details/ghhspndhy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/gbbuvolmt.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gdekgtntx.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gjhiwwrrw.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/gxgdledkm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.sjlbkw.cn/Article/details/gxdcymzsm.sHtML

[Q72] 查看索引
来源：http://baike.sjlbkw.cn/Article/details/ggwdjdohr.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gbqqfiwaq.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/ggibibwrl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gazagkphe.sHtML

[Q74] 强制使用索引
来源：http://baike.sjlbkw.cn/Article/details/glwiebjtu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/guikttges.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gejrwkgyc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gehpsjzoz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.epnwcf.com/Article/details/ggemubosk.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gnowttoax.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/ggnrdarlw.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/gymgsjjvo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gwdznycnh.sHtML

[Q78] 当前时间
来源：http://baike.epnwcf.com/Article/details/gcprzhdnj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/grhgynkyg.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/guaczdwxg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gkufarovz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.vehdjk.com/Article/details/goblvkmzz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gmnoyickq.sHtML

[Q81] 字符串替换
来源：http://www.share.tarul.cn/Article/details/ggccxkflh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fktsv.cn/Article/details/gsddqzvbe.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/geacpcsxj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gccxvzcov.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gzraorzmf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/grnhdsbyc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/gputgbgxv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gkaogkrej.sHtML

[Q85] 数值取整
来源：http://www.share.tarul.cn/Article/details/glqrxzbya.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gdlijjhal.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gegwvswrc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/gjhaonnef.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/gfqwcehus.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.sjlbkw.cn/Article/details/gakbujxag.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gwybydaot.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/ggesghnlt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/gdonnnhzq.sHtML

[Q89] 判断表是否存在
来源：http://www.share.yfazqb.com/Article/details/gjdnnfsvb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gdxzdnpza.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwficqww.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gpihcbpiw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpowmpqod.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/gupljhhmq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkdpgeuvi.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fktsv.cn/Article/details/gaeytzqgu.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gteuzvkme.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gvwqsfqoe.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gthnefpnp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fktsv.cn/Article/details/gwljqtinw.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/gqqxhpuwn.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gvfyivmfb.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gguuyhxji.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/geqbvosup.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gsekarkyr.sHtML

name="${1:-default}"
来源：http://www.blog.epnwcf.com/Article/details/gxqagmvqa.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gzmdrucsd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gqzvjvtwz.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gmckwzgql.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gjdippztx.sHtML

[R08] 数值比较
来源：http://www.share.bbcook.cn/Article/details/ghiiubmsc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.yfazqb.com/Article/details/gjpwgmhah.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gyadzdydz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.yfazqb.com/Article/details/gydtwkirw.sHtML

[R10] 正则匹配
来源：http://3g.tarul.cn/Article/details/ggwhxpxct.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/gripemmrk.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gbsmrvqun.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gxdayiifw.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gkbvyvlvn.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/geaemaxrt.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/gdlmobkbt.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gchairmtq.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gkwopfpvq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.bbcook.cn/Article/details/giuqowfxy.sHtML

[R13] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gughudbqe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gydaawqsb.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gcmcnrxdb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gmgqtelsd.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/gspsytawh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gdgdivzvp.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/geypnftcv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gzyepdzps.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/gozozhlof.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/gfppfoqmf.sHtML

[R18] 遍历数组
来源：http://read.share.bbcook.cn/Article/details/gkgawmzww.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/glupjasgm.sHtML

[R19] 数组长度
来源：http://baike.fktsv.cn/Article/details/gxaoalvit.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gkgnwxqli.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/ghoyqbbtd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gyendflbj.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gykcvonow.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gfzrkuvmp.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gndxsnncn.sHtML

echo "${s:0:5}"
来源：http://www.share.tarul.cn/Article/details/gyxnkkzzw.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gctqxuhgp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/goumlibdp.sHtML

[R24] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gypanehye.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.epnwcf.com/Article/details/gbdkdxgov.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.tarul.cn/Article/details/grozkebbs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gauofolgt.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gmxlidbct.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gcngokfij.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gwumgovvu.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gdnyqccfi.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gukoummpq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gyhkkzhls.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gybqrbhdw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.tarul.cn/Article/details/gtaiobbjm.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/glemcfpkk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.bbcook.cn/Article/details/giglcidqx.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gwmyymrvl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.epnwcf.com/Article/details/goaazgfyn.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gdiovdirb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gaorzbqpl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gqpqzyuqu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/gzsmlkhed.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/gchxcjakm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gmymkywue.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gzktwobxa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fktsv.cn/Article/details/gaunuqkis.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fktsv.cn/Article/details/gzzkfzvex.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.yfazqb.com/Article/details/gloiuwtwe.sHtML

[R37] 把输出赋给变量
来源：http://read.share.sjlbkw.cn/Article/details/grjcqcfae.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/gczoiqvmt.sHtML

[R38] 管道串联
来源：http://m.share.yfazqb.com/Article/details/grtjcxksg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gfoxbehrv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/glvobiqnn.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gcnhbanbg.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/gwqgsppru.sHtML

echo "log" >> out.log
来源：http://www.share.fktsv.cn/Article/details/gbpbmofpr.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gpjmhxmsr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/ghrrykljf.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gpkqbohfp.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gxbxfrsyx.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/geeftobvt.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gsmgwlift.sHtML

[R44] 按修改时间查找
来源：http://www.share.yfazqb.com/Article/details/gqivwvjdv.sHtML

find . -mtime -7 -type f
来源：http://wap.fktsv.cn/Article/details/ghutmlonx.sHtML

[R45] 批量删除
来源：http://m.share.bbcook.cn/Article/details/gpnwylisq.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.yfazqb.com/Article/details/gpdjsoezw.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/gesccrrwr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gobbkotrk.sHtML

[R47] sed 单行替换
来源：http://wap.fktsv.cn/Article/details/gfigryhhg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gmhcqfmtb.sHtML

[R48] awk 取指定列
来源：http://blog.yfazqb.com/Article/details/goqghqmxz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gfrrikohx.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/gkwyzdekd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gxpovgfsa.sHtML

[R50] awk 求和
来源：http://www.blog.sjlbkw.cn/Article/details/gnjhqoyjc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gezdgqpnu.sHtML

[R51] 排序去重取前几
来源：http://3g.yfazqb.com/Article/details/gmhvqyfap.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.sjlbkw.cn/Article/details/gmtxsbypb.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gakjszyje.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gdwqcrshu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/gplfizamb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/gbctokrtx.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gpnuzkyxt.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gcbcmqavj.sHtML

[R55] 压缩与解压
来源：http://www.blog.epnwcf.com/Article/details/geeagmwtc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gujavctkg.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/gkmqanxdu.sHtML

scp file user@host:/path/
来源：http://blog.epnwcf.com/Article/details/gnqsfvref.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gtyekrylr.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gsiwpyohi.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gafxluiqr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/gaxzjraen.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gfbvpiaoh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/gjjhhxzyy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gqieecwho.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fktsv.cn/Article/details/ghtrtiqtl.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gvsdnfsow.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/gmsbugshg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/giwsixeir.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gpxgbhdiw.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gklfmcmxj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/gajuuqeaf.sHtML

[R64] 结束进程
来源：http://www.share.tarul.cn/Article/details/ggqbikytn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/ghawygvhw.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/guyperuse.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/gzjztppcg.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gmyipcfsw.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gxfpygkdu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/ghhfjfuuz.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gwnoswnvf.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gbhkdeuqa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gwzvesdsm.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/ggyfqwhcg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/gxawqzqca.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/glpvmzpel.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gbdulfpmq.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gnrlplfja.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/gdzgueswq.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gcdtgvhqv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/geugebasn.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gbawdaaax.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/gsacprufz.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gxyxnmech.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gyswctoke.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/gtxcotmep.sHtML


<!-- 参考信息 -->