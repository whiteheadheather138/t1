代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/gulquuxid.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gezjjuozr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gytctdwew.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gjhvcslrn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/gjcatlxjo.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/giprlveon.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gfevskivy.sHtML

[Q25] 只取前 N 条
来源：http://blog.vehdjk.com/Article/details/gdhhhtttr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gitfmuvgi.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gvzjrafbx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/goxlcjagh.sHtML

[Q27] 条件计数
来源：http://3g.fktsv.cn/Article/details/gqdkuivrc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gmwbntsvr.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/gsdurwlvr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gumockfmm.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/ggjlnqlvw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/grkweyaqt.sHtML

[Q30] 分组统计
来源：http://mobile.bbcook.cn/Article/details/gimkcvicz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gsfnfurxn.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gseottbop.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.vehdjk.com/Article/details/gzdcnbntg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/ggypkabri.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gplodgban.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/gevuhdgkz.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gxxtqabty.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/gksnplkpu.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gasyfhcoh.sHtML

SELECT * FROM (
来源：http://www.share.sjlbkw.cn/Article/details/gkbuunqha.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gcdwwyhga.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gcuvqalup.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gupscdfee.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gzwutbhah.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/ggplfkmws.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gflixbdzb.sHtML

[Q37] 右连接
来源：http://read.share.yfazqb.com/Article/details/gtkhonxbi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/gwbfizttq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/gzfivcxnc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gfelzbkyd.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/gdxhckfnh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.sjlbkw.cn/Article/details/gusqizixl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/grqpucgzn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.tarul.cn/Article/details/gljnpqvmi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.epnwcf.com/Article/details/gxkziomoj.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gyokrbmlp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gqnpqltax.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gquhdsaan.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fktsv.cn/Article/details/grevyfoph.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.yfazqb.com/Article/details/gtddnlysx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gxaghiepl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.bbcook.cn/Article/details/gswlrzbgz.sHtML

[Q43] 标量子查询
来源：http://m.share.sjlbkw.cn/Article/details/gpfssdgvj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gxmyqmpvb.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gkfbyefii.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/gptcldjes.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/gnsgnhzzq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gjuzgfrfr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/gmmnggazl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gqqiveirw.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gvdpeowog.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.epnwcf.com/Article/details/gnhdycvey.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/grfonuaff.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.tarul.cn/Article/details/gifvsvkiw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/ghehqsggp.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gwhiuukfx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gmcaysjvj.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/ggcuzjxsf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/gowkpjdoc.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/glgbkopjp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gdluvfjhg.sHtML

[Q52] 删除指定行
来源：http://wap.sjlbkw.cn/Article/details/gtypadlvt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gcpczszvo.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gmugupolo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fktsv.cn/Article/details/gfqkqztph.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gbtheyowo.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gnvodlcrd.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gjvbdlsct.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/ggidkffon.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gntkrkqtx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/ggzaljkcd.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gqemgdtwv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ggyactdbi.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/ghkhtsgtl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/ggzwajezh.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gzqltxiur.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gdwdxtvto.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gvaznxovu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.yfazqb.com/Article/details/gynsgvzfp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/ggmmrkpkn.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/gjgzumfqn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gnzwgyjgx.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/gqxysmell.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/geyuiqzbg.sHtML

[Q63] 开启事务
来源：http://wap.vehdjk.com/Article/details/ghbzoxpdh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/gfacmhfbi.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/gqzzdgyxo.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gajbfhmjq.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/ggemrtrgm.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gwmxqeaqn.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gdreaqfez.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gaqvotrss.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gnkflmywc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/ghmpzjink.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gqebgzkbl.sHtML

SAVEPOINT sp1;
来源：http://baike.vehdjk.com/Article/details/gwdhpglzw.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/guxzryfxz.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/guemouvck.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/gsjpigxer.sHtML

[Q70] 更新统计信息
来源：http://3g.tarul.cn/Article/details/gyyhhqtov.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gxtqmhgxt.sHtML

[Q71] 查看建表语句
来源：http://m.share.bbcook.cn/Article/details/gnjznucxv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.yfazqb.com/Article/details/gyfmgbrla.sHtML

[Q72] 查看索引
来源：http://m.share.yfazqb.com/Article/details/gjqsoyxav.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/guvraxoyw.sHtML

[Q73] 查看表状态
来源：http://baike.sjlbkw.cn/Article/details/ghalbtjvk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/gyvfniyvl.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gmpndqbpc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gexqecltm.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gdeaadthn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/gavgidmmn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gezzdoojx.sHtML

[Q76] 按天统计
来源：http://www.share.yfazqb.com/Article/details/gnntatlnm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/gdbkodgvw.sHtML

[Q77] 时间加减
来源：http://www.share.tarul.cn/Article/details/gpffmvjqf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.epnwcf.com/Article/details/gyfskuhls.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gtaknlixg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.bbcook.cn/Article/details/gznbsojzb.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/grccmvuqe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/gigejzcvr.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/geawxxcye.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fktsv.cn/Article/details/gepscsfox.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gxqmaorbo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbjacnyir.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gztwpxusv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gdnfaatss.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gsbbbkyqp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gtxgqnxkk.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gxgyqadfs.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/ghpgxucag.sHtML

[Q85] 数值取整
来源：http://blog.fktsv.cn/Article/details/gdtgsoyia.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.epnwcf.com/Article/details/gbsydxdsx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/ggxjrvwpe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/gvqovclim.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.epnwcf.com/Article/details/ghtexevjl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.tarul.cn/Article/details/gzsrchyfx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.sjlbkw.cn/Article/details/gqunyyjhk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.tarul.cn/Article/details/gnbrgwekf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gqlmgakth.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/geyxidgwg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fktsv.cn/Article/details/ggyiygdvc.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/gkhwltpct.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/giwosfxne.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/girpvbblf.sHtML

R. Bash 专题
来源：http://www.m.share.vehdjk.com/Article/details/glspfpsvm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gycaxamxg.sHtML

[R01] shebang 与严格模式
来源：http://www.share.bbcook.cn/Article/details/gzlcvyijd.sHtML

#!/usr/bin/env bash
来源：http://baike.yfazqb.com/Article/details/gdfsuzosi.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gmvedlfsa.sHtML

[R02] 变量赋值与使用
来源：http://read.share.bbcook.cn/Article/details/gjxugcdsh.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/ginvagpon.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gomoaamvj.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/gsrctfhmc.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/gcifghxux.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/ghkieaxco.sHtML

[R05] 参数默认值
来源：http://m.share.vehdjk.com/Article/details/gdwjlbtbo.sHtML

name="${1:-default}"
来源：http://www.share.epnwcf.com/Article/details/gfggifsqi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/gadjiftwt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gwuiucdhv.sHtML

[R07] if 判断文件
来源：http://3g.tarul.cn/Article/details/guuaeagye.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/giasqrids.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gqdxlafuf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/gjncsmoqc.sHtML

[R09] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gzpymcdja.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.vehdjk.com/Article/details/gllgsemrq.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gatshboys.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gepgyqdps.sHtML

[R11] case 多分支
来源：http://blog.bbcook.cn/Article/details/gmkwokolk.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gibfcpbyh.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/giziqzful.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gdeumsaqz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/gzoipdpwo.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gdfetsccm.sHtML

[R12] for 遍历文件
来源：http://www.blog.vehdjk.com/Article/details/gwpylyagn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.sjlbkw.cn/Article/details/gmgbpztia.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/glpogzoul.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gxvipdysn.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/ggosotbjy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gkfbgvszh.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/grbcckxpk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gcbfntita.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gtidcclnz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gqccescjw.sHtML

[R17] 数组定义与取值
来源：http://mobile.epnwcf.com/Article/details/gblyudrvq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/geeajqmbw.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/gertnogfn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/gaxpiljtl.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gpnqcuwce.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gdaxffjfc.sHtML

[R20] 关联数组（字典）
来源：http://baike.fktsv.cn/Article/details/gwyxnwcaw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gggpdzind.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/gnzsiuxcc.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/gxyqjoxsh.sHtML

[R22] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gsuokitwy.sHtML

echo "${s:0:5}"
来源：http://baike.fktsv.cn/Article/details/gooxgiyqo.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gedkhaxis.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gcfwfnwrz.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gvhccnjaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/gowiloqai.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gvyuzxwct.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gwubtwgev.sHtML

[R26] 命令替换
来源：http://www.blog.vehdjk.com/Article/details/gwpniilal.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.tarul.cn/Article/details/gnthzuycb.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/gvfauaeih.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gzmykptkg.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/gycznihgc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/gilgvjgsy.sHtML

[R29] 定义函数
来源：http://3g.tarul.cn/Article/details/gdanuzgni.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/gchfdqrqr.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gevlomnbg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/garupwkse.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/gyoolgsqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.bbcook.cn/Article/details/gmhygtgdn.sHtML

[R32] 参数个数校验
来源：http://www.share.fktsv.cn/Article/details/gbetcrxdn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gyemamuwx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/grlsfbjtb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gzbcjtsbu.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/gbgzdtlej.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/ggahosygm.sHtML

[R35] 后台执行并等待
来源：http://mobile.yfazqb.com/Article/details/govvgyikd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gqxqagllv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gujghkzki.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.epnwcf.com/Article/details/gdtocuiad.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/ghjteywxy.sHtML

files=$(ls -1)
来源：http://3g.tarul.cn/Article/details/gzftkjkby.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gbtedrdjn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.epnwcf.com/Article/details/godkosbfo.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gzmfmrgtm.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/gxyxrrnuz.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gcqixfpyb.sHtML

echo "log" >> out.log
来源：http://3g.yfazqb.com/Article/details/gcsisodhk.sHtML

[R41] 丢弃输出
来源：http://3g.vehdjk.com/Article/details/gwakxnnzl.sHtML

cmd >/dev/null 2>&1
来源：http://baike.epnwcf.com/Article/details/giwjhjyow.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gjjdmbpkq.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gcoimnrxn.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gqtazxlxa.sHtML

find . -name "*.log" -type f
来源：http://wap.tarul.cn/Article/details/gamfhwmjr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.bbcook.cn/Article/details/gfddexgpc.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/geltzwusu.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/glathmncq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gwnghknuj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gtdxxbcbh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gmiopnayz.sHtML

[R47] sed 单行替换
来源：http://www.share.vehdjk.com/Article/details/gmegyvijn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.epnwcf.com/Article/details/grebsuggy.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gpgpdqgqz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/glexatqyw.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/ghqmugkru.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/gxqwqsadb.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/ggfibvjwf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gfilnxsyh.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gdmnocvpg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.bbcook.cn/Article/details/gpvdbgnjj.sHtML

[R52] 统计行数
来源：http://m.share.vehdjk.com/Article/details/gsxnlzvul.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/gwatrvlow.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gkawjdyva.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/gjwlqhyju.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/gbzoruxeg.sHtML

diff a.txt b.txt
来源：http://m.share.vehdjk.com/Article/details/gvsntlnmo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlisqoet.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/ghkacaqad.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gxpbjsyit.sHtML

scp file user@host:/path/
来源：http://mobile.yfazqb.com/Article/details/ghrsegihv.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/gsfnfaglx.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/gekyaamlx.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gdgfqjufh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gubrjnvnr.sHtML

[R59] 发 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gnleyzfar.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gxllvzqfn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gsoniiraq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gvjcvxdav.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gtcwyulkw.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gvyriqmbe.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gambycyyw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/grtrdpstf.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/gicselblf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/ghkqjeyrk.sHtML

[R64] 结束进程
来源：http://wap.sjlbkw.cn/Article/details/gxmynhnpz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gsxhpvmtu.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/grxfebguj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.bbcook.cn/Article/details/gmixzqbbr.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/gztmcsqxt.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gwnedjmne.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gprpztrlq.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/gsumvhprs.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gjqnleqmq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gmoqwpgia.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gijouobbw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fktsv.cn/Article/details/guzoucjhi.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gzvhilzqu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gihqibols.sHtML

[R71] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/ggvyxxmjn.sHtML


<!-- 参考信息 -->