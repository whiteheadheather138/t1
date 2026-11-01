代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/gqyqljean.sHtML

[Q24] 去重
来源：http://read.share.vehdjk.com/Article/details/gmowkuyyw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvatdxwwp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gzokalahl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gmekxtzvn.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gvyeiuduf.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.bbcook.cn/Article/details/gzrbqxdym.sHtML

[Q27] 条件计数
来源：http://3g.yfazqb.com/Article/details/gzoghuirw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gmxqorzas.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gslknsgyv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gbjeuvzgt.sHtML

[Q29] 最大最小值
来源：http://www.m.share.tarul.cn/Article/details/gbtyfnjfi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/geosnbxsf.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gsirmdqnr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gvymxsszc.sHtML

[Q31] 分组后过滤
来源：http://baike.epnwcf.com/Article/details/gjeivyyyq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fktsv.cn/Article/details/gaswzvixe.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gktnfvprn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gywdrimme.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.bbcook.cn/Article/details/glpsvypzz.sHtML

[Q33] 多列分组
来源：http://wap.epnwcf.com/Article/details/gtglatjlm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gycbolpat.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gowiamenr.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/guyzkeblt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/ggmfsygei.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/gddxgtykj.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gvulmkptt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gpbvkevdu.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gdwbcuvra.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gvjjngjde.sHtML

[Q37] 右连接
来源：http://3g.tarul.cn/Article/details/gzjqdqmno.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/gwpfzbdqe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.vehdjk.com/Article/details/grdrcbktl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gqjcrgetn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/grhzoizsv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gmwzpsecg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/glqpleoke.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gajknxfcr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/gtknoexfo.sHtML

[Q41] 多表连接
来源：http://mobile.fktsv.cn/Article/details/gufoqmkra.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/glutnjbtt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/gevxnzgsy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gxekffhqb.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/gulwoqvpi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/geskpllai.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gkxoibbky.sHtML

[Q43] 标量子查询
来源：http://www.blog.epnwcf.com/Article/details/gaktfkpde.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.sjlbkw.cn/Article/details/gxektxioo.sHtML

[Q44] IN 子查询
来源：http://wap.epnwcf.com/Article/details/gtyxilhas.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/gfvpmsttu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.epnwcf.com/Article/details/gkulyemzu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gtsrqzwnx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gjbxxlhwz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gfiwwlnjf.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gdmdhboyx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gayvmgycx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gnmnpogxm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gxopvhvbz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gszesreud.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/gtztalrxm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gxndzmjjc.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/gupsmhudg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/ggfkeoxio.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.tarul.cn/Article/details/ggpchuvey.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/gnzzboigg.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/gtjeuhztc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/gehygfoea.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gpjmirukj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gucczvekk.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gpymshbbe.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gxdttonyj.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.yfazqb.com/Article/details/gdfxnijki.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fktsv.cn/Article/details/glbrvchzo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/ghhbwjjrc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gkvojepzt.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgdcarnp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gowrivyqs.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/gccxvnbtq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjghtqpp.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/gsjohnqeg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gqsdxirmq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.sjlbkw.cn/Article/details/gqoklwcru.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/ghwiobhru.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gtyuihcdh.sHtML

[Q61] 移动平均
来源：http://www.m.share.sjlbkw.cn/Article/details/guspptvvc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gybsbrxnk.sHtML

[Q62] 分组占比
来源：http://www.blog.epnwcf.com/Article/details/gjkpcqrpa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gkqjtoklq.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/giezgyiso.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gyvrqqnyb.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gxisfjzbv.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/gpgsabvxr.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gvplyffdq.sHtML

ROLLBACK;
来源：http://3g.epnwcf.com/Article/details/gozqumsgl.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gloqbbnth.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fktsv.cn/Article/details/gzqeztczz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gzsvuepms.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/ggjqyfjss.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gnntcmczh.sHtML

SAVEPOINT sp1;
来源：http://baike.vehdjk.com/Article/details/gteaixkoq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/grlpnbxeb.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/glwsndzcj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.sjlbkw.cn/Article/details/gdarjjgeo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fktsv.cn/Article/details/grhiiaezt.sHtML

ANALYZE TABLE users;
来源：http://baike.vehdjk.com/Article/details/gyugnapgp.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gkfczxvpn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gppbkptno.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gauldpjgd.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/gggrxuwgi.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/gdyksurnb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/gmcaxjttr.sHtML

[Q74] 强制使用索引
来源：http://baike.bbcook.cn/Article/details/glzvemiwv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/gcvtqgpth.sHtML

[Q75] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gmuqrrkrs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.tarul.cn/Article/details/gcoxhiqxz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/ghgugccgq.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gfmxsrdqf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gvgnfdqfs.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/grfesorer.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gbkhffcry.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gqtnkzbiu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.bbcook.cn/Article/details/gobplzvaw.sHtML

[Q79] 字符串拼接
来源：http://mobile.tarul.cn/Article/details/gpfgpfjfb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/gxxwkdqmp.sHtML

[Q80] 字符串截取
来源：http://read.share.tarul.cn/Article/details/gklxbstrp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gfrdftbwb.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gwyhrzjml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gvvgodfru.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gvvvevjtu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gqayqyhdi.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gilvetycn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gcjqvnzui.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gpcodaicd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvmgrqjfh.sHtML

[Q85] 数值取整
来源：http://3g.yfazqb.com/Article/details/gdeuhdwma.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gbgikpjfj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/ghfnhpmzs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gvqsbvebx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gugeyersz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gxxsmuejw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/gydnsrurw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gepsddehj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gfagnnyci.sHtML

[Q89] 判断表是否存在
来源：http://read.share.bbcook.cn/Article/details/gnzzeihwv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gefebvfzj.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gjmqehvpp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.yfazqb.com/Article/details/gdmxkyalp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaponwmin.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gcjoqieek.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxyuudpkt.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.bbcook.cn/Article/details/gpvuyvrip.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gxqiyrwqn.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/gvdoymmoe.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/gbifnfokl.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gjsxxfynb.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gilqlbhey.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gkiasdskr.sHtML

[R04] 位置参数
来源：http://read.share.yfazqb.com/Article/details/guwuvjwlo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gjoptnhkw.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/ghxsbrznz.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/gfrdmyspo.sHtML

[R06] 判断命令是否存在
来源：http://baike.epnwcf.com/Article/details/gxwwtabhm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gzilndsve.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gftibrwab.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.vehdjk.com/Article/details/gctfucdix.sHtML

[R08] 数值比较
来源：http://m.share.yfazqb.com/Article/details/gfbtluhbz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gfzabpmrx.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gmqzbopfm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.bbcook.cn/Article/details/gkdzqzuup.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/gqnnyhvai.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.tarul.cn/Article/details/gkcriiblb.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/grsemiepa.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/ggdiezoel.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gywcamgos.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/glrtzfgbj.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gmlpcetsk.sHtML

esac
来源：http://www.blog.tarul.cn/Article/details/gjdkdhaiv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gqpcbptno.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gfwjvaert.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/geetccopi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gvmxerbjw.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/grxggrnxv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gsmjyuogq.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/guxyicevj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gwkqjhide.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/gfylqsjxj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gqssfvoxs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fktsv.cn/Article/details/gykpdseyw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/gammvchaf.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gqwrefggw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.epnwcf.com/Article/details/guuteybvj.sHtML

[R19] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gkptenwup.sHtML

echo "${#arr[@]}"
来源：http://read.share.bbcook.cn/Article/details/gajngwjll.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gtuwzkvkl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gnyeifggq.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/glxoqbqcf.sHtML

echo "${#s}"
来源：http://wap.epnwcf.com/Article/details/grmnnmruk.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gnaualnln.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/grnwercge.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gsxzjinoj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/gcikdofvh.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gvoifegfh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gjuhlolud.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.yfazqb.com/Article/details/geimxifqb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/gmnhkmyug.sHtML

[R26] 命令替换
来源：http://mobile.tarul.cn/Article/details/grvwskyri.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gvuvaigqp.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gpquitewk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/grdyxrnjp.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/gklmifliq.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gqmxuvgln.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gwbohccou.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/gunquyqro.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gypxkbdru.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.sjlbkw.cn/Article/details/goouyvmgv.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gnrrhgrmf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gpbalulqd.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/gvykrfids.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gombkmugh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gptiztoxy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fktsv.cn/Article/details/gcuhgujbh.sHtML

[R34] 退出时清理
来源：http://baike.vehdjk.com/Article/details/gkprzkrry.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gaasffbpp.sHtML

[R35] 后台执行并等待
来源：http://3g.bbcook.cn/Article/details/gfcrmaqba.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/gestekteh.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gxwpqrkwe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.bbcook.cn/Article/details/gvtoaupsa.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/gnqkltoaq.sHtML

files=$(ls -1)
来源：http://blog.yfazqb.com/Article/details/gyngiwnet.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gkppownfj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/gekckgivf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gxtpzdcce.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gfemfwqiz.sHtML

[R40] 追加写日志
来源：http://baike.tarul.cn/Article/details/gyncxwmrw.sHtML

echo "log" >> out.log
来源：http://www.m.share.bbcook.cn/Article/details/gttxaenjl.sHtML

[R41] 丢弃输出
来源：http://read.share.yfazqb.com/Article/details/ghjcxzdzl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gjxorduta.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gsjqscgyp.sHtML

wc -l < a.txt
来源：http://www.m.share.tarul.cn/Article/details/gxzzbmiif.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gfedgiucu.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gglawkios.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gmunfudlm.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gsvdzctqr.sHtML

[R45] 批量删除
来源：http://www.blog.epnwcf.com/Article/details/gzophtqvu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gdsbfpeca.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/grrntuwar.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/gwuzhwcie.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/grwpttpsp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gbfavlmsq.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/ghegnvlfb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/ggbbwvaah.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gtfjvghmz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fktsv.cn/Article/details/gecjfmsfr.sHtML

[R50] awk 求和
来源：http://blog.yfazqb.com/Article/details/goboljkep.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/gnxwaydoe.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gqkcoostq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdxuylzp.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gsiauikyl.sHtML

wc -l a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gnfnjsuhy.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gsthryiup.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gelmhnyqj.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gbnwgtjzj.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gkcbiwdcb.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/grlxihpxb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/gavdugnry.sHtML

[R56] 远程拷贝
来源：http://baike.vehdjk.com/Article/details/gbrkdkojg.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gcrhpdmbm.sHtML

[R57] 远程执行命令
来源：http://m.share.yfazqb.com/Article/details/grtefrmek.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/goajyztfk.sHtML

[R58] 下载文件
来源：http://www.share.yfazqb.com/Article/details/gqlpvsuyo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/gafybedkh.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/ggbhsfthk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/gqmljvqsy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/geruccdpo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gbepzonea.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gviciphlo.sHtML

df -h;  du -sh *
来源：http://www.share.tarul.cn/Article/details/gflzqbstg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.tarul.cn/Article/details/gfmztudcj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/gtyvhsnxb.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gwrhrwpwo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/gdhjrjrpj.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/gdopscawc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/grexcchmy.sHtML

[R65] 查看端口占用
来源：http://www.blog.epnwcf.com/Article/details/gkyxsfzie.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/gejrdljmv.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/gkqhgnfmt.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gqlcleoqh.sHtML

[R67] 生成随机十六进制串
来源：http://3g.epnwcf.com/Article/details/gkjljtwmi.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/gehqhfdvj.sHtML

[R68] 计算文件校验值
来源：http://read.share.sjlbkw.cn/Article/details/gbwlzutmg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/gixifdwfh.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gcckqvygo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gnzkwdtmn.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/glwaemgst.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/ghcjxcdhz.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/ggferirmt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gqjoltltr.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gnsibmhoj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gdqdnjkfk.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/ggagrkqwk.sHtML


<!-- 参考信息 -->