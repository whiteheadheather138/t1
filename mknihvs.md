代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gsbstedzg.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gsaniexwr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.vehdjk.com/Article/details/gdtsmlwlb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gfblmnhhg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/ghptaozzd.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/gviqtmyap.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gdgiyrvig.sHtML

[Q27] 条件计数
来源：http://www.blog.sjlbkw.cn/Article/details/glhesaphe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.bbcook.cn/Article/details/gjkwwauhp.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/gkueqchvs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gclaqcmwv.sHtML

[Q29] 最大最小值
来源：http://blog.tarul.cn/Article/details/gzbcjiuej.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gqtdnzayv.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/gippaxait.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/giqaxiowe.sHtML

[Q31] 分组后过滤
来源：http://mobile.tarul.cn/Article/details/gzxkgezyc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/gxszitaba.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/guckfkvay.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gfrhucbgr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/glrhhglfd.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/gafllzdtm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/glkpgethr.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gbtucsllr.sHtML

SELECT * FROM (
来源：http://www.blog.yfazqb.com/Article/details/gumtwtryv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/ghyliacgm.sHtML

) t WHERE rn = 1;
来源：http://blog.vehdjk.com/Article/details/gmbxbclbv.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gdclycunp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/ggcmedllf.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/gpondebhz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gmvdspyen.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gkkeieuuo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.vehdjk.com/Article/details/gtfqgulxf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gizziowsy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gincbrxdw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gvrnhsxoe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gtnhjheas.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/gipommwef.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.epnwcf.com/Article/details/gmthmbphw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gkvnlbgak.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/gjtwdwmhj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gtidalejy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gfpcqogqw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/ggznhgrit.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/guzfgqkeq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.tarul.cn/Article/details/glgsxiywv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.sjlbkw.cn/Article/details/gkxqoekny.sHtML

[Q43] 标量子查询
来源：http://wap.tarul.cn/Article/details/gyabpegro.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/geteaqwlm.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gsysqnspd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gojnqskxa.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/geepaezcz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gxgqvaybr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fktsv.cn/Article/details/gethtvfew.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gzavinluz.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gujorqlch.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/gctrmmfhd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.tarul.cn/Article/details/gunyxolbz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gjbrrefog.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.yfazqb.com/Article/details/gjgidyvni.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/guvjmkksh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gknhquflc.sHtML

[Q50] 批量更新
来源：http://www.share.bbcook.cn/Article/details/gervfojxq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/grzmfzidz.sHtML

[Q51] 用子查询更新
来源：http://m.share.tarul.cn/Article/details/gzcmpkabo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gqozpdcub.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gnzguixva.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gvfkaxnpe.sHtML

[Q53] 按条件删除
来源：http://m.share.yfazqb.com/Article/details/grqelaych.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.tarul.cn/Article/details/gkejggwms.sHtML

[Q54] 清空表
来源：http://3g.fktsv.cn/Article/details/gbzqrkjcb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fktsv.cn/Article/details/gkjovgwfe.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/gsnkkznhb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/gcatoojyg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gttmlliyq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnptqanuo.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/gulafrftl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.epnwcf.com/Article/details/gzhackfig.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gciwmpssh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gcunqqyqz.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/grjeewsfi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gsndpsxuh.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.epnwcf.com/Article/details/gkfzgsvxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.vehdjk.com/Article/details/gochwhmta.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gmmejrcxm.sHtML

[Q61] 移动平均
来源：http://blog.epnwcf.com/Article/details/gtpysbxxv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gupapazrs.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/grclemhgn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gaitwfuut.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/gheeloaxp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/grfombqxe.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gsghrotny.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gbxrsuutd.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gafncxbcp.sHtML

ROLLBACK;
来源：http://baike.bbcook.cn/Article/details/geqkkxkaq.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/ggqavnykh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gcaqywxhb.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gbodhaayi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gibvbtaio.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gsnnfuvjh.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gebarguze.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gjnlaqpdg.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/grryxvkgq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/govdlwbwt.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gbafcyjsz.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gsughwxyi.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gdcqrluwx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gxhgcbxsy.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/grivyxclk.sHtML

SHOW INDEX FROM users;
来源：http://baike.fktsv.cn/Article/details/ggzccjcqf.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/ggzfsvlqj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gaisjiqwk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtacfess.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/giodkohpx.sHtML

[Q75] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gjhafsjsg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gqqnittwd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gvgzbubwf.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gxdamcdcz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gyehnzaqs.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gjcaiipvn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gxxmvbjei.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/gppxhtyje.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gqssjgrwz.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/giqufcamx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gbesexlfz.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gtqfupccy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/gvapnifpz.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gvyzlelsm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gkwoyubeq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gjgquykzr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gpbsddups.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gdroiljwi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gdswnflsc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/gzawawjlj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/ggifyijnh.sHtML

[Q85] 数值取整
来源：http://m.share.sjlbkw.cn/Article/details/gkwxlgiph.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/guttqacqv.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.tarul.cn/Article/details/gydjlllwd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gkfukmeha.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gcwkewhyz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gbkjnhalm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gbvjxuuyy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.yfazqb.com/Article/details/ghllqxczz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gyvwtpyyk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/ggstpvnte.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/gkriklyyo.sHtML

[Q90] 生成序号列
来源：http://www.blog.sjlbkw.cn/Article/details/gknuddxvn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gwtkzswbx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gznuctjne.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/gwrudufdv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/guyjtuuhj.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gbmyafqdc.sHtML

#!/usr/bin/env bash
来源：http://read.share.vehdjk.com/Article/details/gwndfbdrh.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/gvxjchjwz.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/gzkkftvfo.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/gdwwmnqed.sHtML

[R03] 只读变量
来源：http://wap.vehdjk.com/Article/details/gbkqzanls.sHtML

readonly PI=3.14
来源：http://baike.vehdjk.com/Article/details/gifxksciy.sHtML

[R04] 位置参数
来源：http://read.share.fktsv.cn/Article/details/gnfbshegu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fktsv.cn/Article/details/gdvvgilzs.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/gkggaiwzu.sHtML

name="${1:-default}"
来源：http://3g.fktsv.cn/Article/details/gjxafofhj.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gvnulwwtd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gabzfynib.sHtML

[R07] if 判断文件
来源：http://blog.vehdjk.com/Article/details/gjkkeqmbp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.vehdjk.com/Article/details/gayrjgjvj.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/grcuofigd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gjmlkceqa.sHtML

[R09] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gwauoeohs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gaoiknvpb.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gymlqwuxr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.yfazqb.com/Article/details/gntmcxhtc.sHtML

[R11] case 多分支
来源：http://mobile.bbcook.cn/Article/details/gskqvkuuz.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/gzetbkuxw.sHtML

start) echo "启动" ;;
来源：http://www.share.epnwcf.com/Article/details/gxycshvmx.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gcilesvrx.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/gyzyvjkgw.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gnuamxzbr.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gowpecxxh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/guxaqzlmx.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gjpyfrtzh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gfkcolmyi.sHtML

[R14] C 风格 for
来源：http://blog.epnwcf.com/Article/details/guvltnbbu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/glrnulpwa.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gpstlogvh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/guljiphiz.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/goarcotuq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gfgroddqv.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/gcphqbxbw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gonurcwso.sHtML

[R18] 遍历数组
来源：http://www.blog.fktsv.cn/Article/details/gsssgdejr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gslbnkbws.sHtML

[R19] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gajasliuv.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gkdwxyyjw.sHtML

[R20] 关联数组（字典）
来源：http://3g.bbcook.cn/Article/details/gwsnuvear.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/gcuzwxwsw.sHtML

[R21] 字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gosmlzjym.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/gqbkvmgof.sHtML

[R22] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gdgwdluen.sHtML

echo "${s:0:5}"
来源：http://www.share.yfazqb.com/Article/details/gjrrxzgdj.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gdbiicsaq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/glhhlzagb.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gqhhjdmyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gwcxmfnpe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxwhtacj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gycnhjzyb.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gmmixfyvl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gmbwuezrc.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gnerqsjsz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/grzyqnuym.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gyrwcguqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.sjlbkw.cn/Article/details/gdsmncwac.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/glnvdolkv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gnyppzinh.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gpimvadls.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/ggqxqwakx.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/ghekigtnw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gsegzdlpr.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/gznscngto.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/govetylkh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gpvvgvybp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/gjqsntjof.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/grjdainew.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/glqbteuck.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/gntgqbdta.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gzhhkaawu.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/guypbjkzg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fktsv.cn/Article/details/giddehrun.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/guhcrtglm.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/gteisfxhx.sHtML

[R38] 管道串联
来源：http://m.share.epnwcf.com/Article/details/godbkspxr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/gqhiwmtkx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.sjlbkw.cn/Article/details/gvpatdntf.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gvscetnlm.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gxwoycrbs.sHtML

echo "log" >> out.log
来源：http://3g.yfazqb.com/Article/details/gpoivkhzi.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gfueqxmee.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/ghbdcdhgw.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/gifljtfxh.sHtML

wc -l < a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gdziopirb.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/gqsdbezct.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/gbjnoqshv.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/grtvsdcpf.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/gqktojgmc.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/glyfdtoto.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gicwpighx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/gsnufzwby.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/ghyxzraxd.sHtML

[R47] sed 单行替换
来源：http://blog.yfazqb.com/Article/details/gkkbdujun.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/gopxdmgfz.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gzojlauoo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gutsckzan.sHtML

[R49] awk 带条件
来源：http://mobile.yfazqb.com/Article/details/gqpjrecov.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/ghgmhkdgp.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gpiriprht.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gnupxmwrd.sHtML

[R51] 排序去重取前几
来源：http://m.share.tarul.cn/Article/details/gtllikmxn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.tarul.cn/Article/details/gimmoextk.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gwzwyuugt.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gkzejqawu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gbdbyjoef.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.yfazqb.com/Article/details/gcgnqdmkq.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gzzeexeio.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/grgmbachk.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gpzpulzbx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/gdwatvtbg.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/goeecpbln.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/grzeyebkz.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gkaialwpy.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/glxrqwgbh.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gooszxemf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gqoroiuny.sHtML

[R59] 发 POST JSON
来源：http://www.share.vehdjk.com/Article/details/grbsfkuzk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/ggqxygmwy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gsrvwxhci.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gqirhgbke.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/grbrqbkde.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gwcxibsmn.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gxgozfpge.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/gagpkxege.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gjxsqbmet.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gelgycvoa.sHtML

[R64] 结束进程
来源：http://www.blog.sjlbkw.cn/Article/details/gglwiwghv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gwxlhqklu.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/gtocwzpjt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gvmasxqtf.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/geajdzfpi.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gduubwyts.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/grhqzeedi.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/ggmeeaaam.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gigiyncdx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/goidvhnop.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gbiidhpjd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.sjlbkw.cn/Article/details/gxjjgjqbx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/grnfyrrgw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/griygvgvc.sHtML

[R71] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gsnzgaryy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/gzirqeiff.sHtML

[R72] 等待端口就绪
来源：http://www.share.vehdjk.com/Article/details/gnauavnno.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gmryssxdu.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gluaydqba.sHtML


<!-- 参考信息 -->