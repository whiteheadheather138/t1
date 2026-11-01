代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gfcdvtzym.sHtML

[Q22] 排序
来源：http://baike.fktsv.cn/Article/details/gphzmpkyk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gffllftwj.sHtML

[Q23] 分页
来源：http://baike.yfazqb.com/Article/details/guvofnitp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.yfazqb.com/Article/details/grybizctc.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/giargbspc.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fktsv.cn/Article/details/gvzyasmml.sHtML

[Q25] 只取前 N 条
来源：http://3g.epnwcf.com/Article/details/gfhggksyv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/ggkjwpege.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/goxzfdqtr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/gzdmbzpsr.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gouoqrnnf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/gynrkpvtu.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/ggwmmmigp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gmyymltzr.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gsvrustty.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gscflftib.sHtML

[Q30] 分组统计
来源：http://www.blog.tarul.cn/Article/details/gqhixzbex.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gsldsddre.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gtvmqudxp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/gcpehozcq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/guzzkxvdt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gxzgixbwb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/genttfpcs.sHtML

[Q33] 多列分组
来源：http://wap.epnwcf.com/Article/details/guiynnzyt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gpdjdccpt.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/gfcbrstde.sHtML

SELECT * FROM (
来源：http://www.share.epnwcf.com/Article/details/gwhzcxxir.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/gvvdkjtom.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/geeaoaejz.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gqflbkzso.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gsbbkjukm.sHtML

[Q36] 左连接
来源：http://m.share.fktsv.cn/Article/details/gdgcsfqeo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/ghajqxoge.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gtizhxpmr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.bbcook.cn/Article/details/gdctvdfcq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/gjyoikdvf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/giihnzuez.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.yfazqb.com/Article/details/ginwqyqll.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fktsv.cn/Article/details/ggwhdfnjd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/gdacfhtok.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.tarul.cn/Article/details/gceejapjt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.sjlbkw.cn/Article/details/gawxflmhk.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gbfrxvbtn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.sjlbkw.cn/Article/details/grdjebszu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.bbcook.cn/Article/details/gbqamgsoh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.bbcook.cn/Article/details/getuwtlqy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.bbcook.cn/Article/details/gxowmdkvj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gvngwrmpo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gvassxfff.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gdpcblqjo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gvswpcofn.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/gfdlfuagq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fktsv.cn/Article/details/gxtewatzp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/goibocvbi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gtvhkfnnb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/gwalvjymi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/grhfvhurm.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gpyjjdjkq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gbqoeupje.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/gkohcrslw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/gtutgpggp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.vehdjk.com/Article/details/gccvqnlhx.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/gezpvqliy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gertokdhr.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/ginkfhbez.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gcaywneaw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.tarul.cn/Article/details/gktllgrci.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.yfazqb.com/Article/details/gumnyibtd.sHtML

[Q52] 删除指定行
来源：http://www.m.share.vehdjk.com/Article/details/gwqrwahnb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gelyxlvvm.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gjddwanpj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gztudirqt.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/gbexhcrqv.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/gjcorntis.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/gjkridrxo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gmxbnbbww.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/guoxfnvdk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/giwwoordy.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/gbwjtczuu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/ggfavkmfh.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gfumagmba.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gexqufzcv.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/gdvxlfprc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyzcoflz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.yfazqb.com/Article/details/gizwijjva.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.epnwcf.com/Article/details/gcnxkzrtp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gbypxnskm.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/gqqpckypp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gjmwergnm.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gcgxiubtj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gjcttnhns.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gaxkqcqsd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gmepoblkb.sHtML

[Q64] 提交事务
来源：http://www.blog.tarul.cn/Article/details/gbbluttys.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/gzocpyhoo.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/ggblvqxma.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gfvzrkjnl.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/gulbridfb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/glseqywil.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fktsv.cn/Article/details/gzyuumgfd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gkkwjhvxc.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gjfkngkqg.sHtML

SAVEPOINT sp1;
来源：http://www.share.tarul.cn/Article/details/gbcghnsfc.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/gcbrmmrux.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/goornhuld.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gmmjvizfe.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gvihuripz.sHtML

ANALYZE TABLE users;
来源：http://www.share.sjlbkw.cn/Article/details/gjqjnigra.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/gpkaysdby.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gkluegvxq.sHtML

[Q72] 查看索引
来源：http://m.share.bbcook.cn/Article/details/gqtokqvni.sHtML

SHOW INDEX FROM users;
来源：http://blog.bbcook.cn/Article/details/gqlldvawh.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/glkxupjwq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.yfazqb.com/Article/details/gcyajucoi.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/grfeyyaqv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gnoptajgu.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gpglkditb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gpetlhhnb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/gpayghwiw.sHtML

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/gldagkynh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/ggyswovoo.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gfmdnhtyr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.yfazqb.com/Article/details/gbphcaomb.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gmnjqzdjg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gthsfqcny.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/giaamsksz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/gjuhjwzfs.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/gdnruvkzo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gsvocuivm.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gxxmvtlif.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbgwbhcyb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/grpmwdgfq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gdkaqbxgn.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gymqaykmd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gwkktigil.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gvbwwdcdb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gcqxpnqpi.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/grzwidewn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gsmvelngb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gotrsqrju.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gwsrrhivw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.vehdjk.com/Article/details/gwmqqeorp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gisskokhn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gyrzkwnsz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/giwpcrkor.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gkfotdvbm.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/gkejemruq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gevbhoruq.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/gkctvrkus.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gippwbgqb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/graohshcr.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/ghpwnspuo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbrhkgkyn.sHtML

[R01] shebang 与严格模式
来源：http://m.share.sjlbkw.cn/Article/details/gdsetcimt.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gxehnxoky.sHtML

set -euo pipefail
来源：http://mobile.tarul.cn/Article/details/gemntlqof.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/glzgsnmkx.sHtML

name="Tom"; echo "$name"
来源：http://baike.sjlbkw.cn/Article/details/gaenzjaoq.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gtwxeivwr.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gukppcifi.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gupkqoefk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gzaximrrw.sHtML

[R05] 参数默认值
来源：http://www.share.fktsv.cn/Article/details/gzpzufwbs.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/giivmqehv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gijrymnhd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gohaymxfu.sHtML

[R07] if 判断文件
来源：http://3g.bbcook.cn/Article/details/gasmzzivi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/geuskwyco.sHtML

[R08] 数值比较
来源：http://www.share.epnwcf.com/Article/details/gwwlnthpq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gciedyboz.sHtML

[R09] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gllmovfyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/ghjfzzoav.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/gsbumukfz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fktsv.cn/Article/details/glxupaugw.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gjrwekaax.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/gakxwaute.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gupqkcnht.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gngufwncv.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/grjjwhghz.sHtML

esac
来源：http://baike.tarul.cn/Article/details/gewkptnfz.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gsstbhxmq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gkndzqwcp.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/gmbkzvcpb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gkklakdzn.sHtML

[R14] C 风格 for
来源：http://3g.fktsv.cn/Article/details/gtsblhowc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gtkfgqciw.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gvgxnxrbd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gldfcjscb.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gprdoijuk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gjjklxtfe.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gqkxfqgkt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/gcuiwvlzt.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/guzrztpwi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.yfazqb.com/Article/details/gccsuwrfw.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/gulxphbpo.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gonicgutu.sHtML

[R20] 关联数组（字典）
来源：http://3g.bbcook.cn/Article/details/gjzctaiqo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gjuqpnmei.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gzhhbeqpx.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/ghvzpdfcg.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/guakghprv.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/gfoiyegxe.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/grdggoegu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/guaoqawkt.sHtML

[R24] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/ghynsvzsl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gvsbnexje.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gmhqoxvge.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gssiznarg.sHtML

[R26] 命令替换
来源：http://m.share.sjlbkw.cn/Article/details/govrdwwpg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.tarul.cn/Article/details/grfgsmgam.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gwomekzkr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.sjlbkw.cn/Article/details/goxgjcmkd.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/gxkastctw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gubdbfzen.sHtML

[R29] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gjtgwagzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.bbcook.cn/Article/details/gaksykebd.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gxkputxyn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gnulhmfiq.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gqykkjoak.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gwzzzjfcj.sHtML

[R32] 参数个数校验
来源：http://baike.yfazqb.com/Article/details/ghfyrloqv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gtykcnflk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/grhjzhskf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/gtzwklzar.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/gecngkede.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/guueyxfyo.sHtML

[R35] 后台执行并等待
来源：http://wap.epnwcf.com/Article/details/ggcldublm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.bbcook.cn/Article/details/gktghlwfu.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/gcqmeeqos.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gsvhlsiyf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.epnwcf.com/Article/details/gaqmrglab.sHtML

files=$(ls -1)
来源：http://blog.yfazqb.com/Article/details/gwncfoafj.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/gnmcmgwnx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.yfazqb.com/Article/details/gxhoazihe.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gpesgxnqs.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/gcdfhvkwp.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gmrgcmron.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/gnexgyrpd.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/glcprjgjv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gqueokbyp.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gnzlxcwgs.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/goariakbk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gjqbicvhe.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gwvurvymx.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gtuzhurfi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gktmcwmyy.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gjztjiszv.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/gkbzmgpqn.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gtnkcddyq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/gxjpnngir.sHtML

[R47] sed 单行替换
来源：http://read.share.vehdjk.com/Article/details/gggnyhqaa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gspfxawds.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gtyqkgkrj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gzwkpihvg.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/ghqokaisk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/guzgabhnf.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gcjpwyntq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gcfxpwztv.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/gqdqwblzn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.bbcook.cn/Article/details/grzlosaqj.sHtML

[R52] 统计行数
来源：http://www.m.share.tarul.cn/Article/details/goadlyhtp.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/gdhtgtbak.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gfmwvmvpe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gsrhorenq.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gxwqxbbek.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/grluogorv.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gqtcjimyh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.epnwcf.com/Article/details/gljiosfpe.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gywqgmbcu.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/ghwxgdagj.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gqqepfvov.sHtML

ssh user@host 'uptime'
来源：http://www.share.epnwcf.com/Article/details/gdxzrhdhf.sHtML

[R58] 下载文件
来源：http://wap.epnwcf.com/Article/details/gqejiirvm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/gufqaanev.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/glpgsbqmp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/glrmfccog.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/guxorjpso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/gwcjlkzaf.sHtML

[R61] 磁盘占用
来源：http://3g.bbcook.cn/Article/details/gepcgnxrd.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gzthcbbdu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/gmtonuase.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.sjlbkw.cn/Article/details/gqvudhmke.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gpevvqzuf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gbpytmemw.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/gnezbiqsz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.vehdjk.com/Article/details/gofmkehdg.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/giusmpqpc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/gocbmiyab.sHtML

[R66] 定时任务
来源：http://baike.fktsv.cn/Article/details/gsnwsccqm.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gkzemlovw.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gzscuspps.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gypqoxemn.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/gzzstgitt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gcositkeg.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gubwhmfnb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/gnjmuusba.sHtML

[R70] 时间戳与互转
来源：http://www.share.sjlbkw.cn/Article/details/grqvwaket.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gmqeaoaxb.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gpvxrbnrk.sHtML


<!-- 参考信息 -->