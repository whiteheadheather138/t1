代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gtrnbpjyu.sHtML

[Q22] 排序
来源：http://www.blog.vehdjk.com/Article/details/gifccfnmp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.bbcook.cn/Article/details/ggmfvmejv.sHtML

[Q23] 分页
来源：http://baike.bbcook.cn/Article/details/ghiwidpgp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gvczoujpk.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/ggqroebqt.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gaczdbigs.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gntdvmnns.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gtulogcxx.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gvetduumi.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gvxdrbagb.sHtML

[Q27] 条件计数
来源：http://3g.yfazqb.com/Article/details/gxovnthsh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gpmmnqonx.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/gdbcwtiri.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gqxbpwfre.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/gqzsctxhc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/ghxkhibqk.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/gxyksxqxp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gnzktthkb.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/gqieqyrzj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/gswxybebz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gpiloujup.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gegbguevy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/gnmljgoer.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/guumqmeev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gzvrcssxi.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gpzgwuvyx.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gfosileie.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/ghtzlmfvb.sHtML

) t WHERE rn = 1;
来源：http://3g.vehdjk.com/Article/details/gagczjnog.sHtML

[Q35] 内连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gzndydkii.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.tarul.cn/Article/details/gdibywpno.sHtML

[Q36] 左连接
来源：http://blog.yfazqb.com/Article/details/gzzifioho.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gsycilytx.sHtML

[Q37] 右连接
来源：http://wap.epnwcf.com/Article/details/gdvglqvzk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gugyxelwv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/glwsravxw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gaswpkckt.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.tarul.cn/Article/details/gdfvveqdm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/giwnhjfly.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gvkyfrwki.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.bbcook.cn/Article/details/ghzeblang.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.epnwcf.com/Article/details/gochvdqab.sHtML

[Q41] 多表连接
来源：http://baike.vehdjk.com/Article/details/gxohlxsob.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gafleqshv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/ghtdzshev.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gjgmdkavq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gcgelxptx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.vehdjk.com/Article/details/gxhhnwetg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/gtbnnkglf.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/gjcfkrwca.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gldjabjzs.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/guvyxqlev.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gttvcqnze.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/ggysppqzr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gggzpsoyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gyaymzzxa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gdmypveni.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gccueummx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/grbhnkfqq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/grsppxwbv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gxtlxhnwz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/gdosvxjqo.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gtfpjscng.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gtvvijqot.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/ggxvgdcpa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gmcikaxow.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/gvknnhswz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.bbcook.cn/Article/details/gfjbwuziy.sHtML

[Q52] 删除指定行
来源：http://read.share.sjlbkw.cn/Article/details/gafylxemc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/gedfvjgys.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gdbqlirhe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/gcxitdiic.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/geljhqfit.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gzvijzcgi.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/gmkjdtcxw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/ghlvoskea.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gstywufgg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gkvoubhds.sHtML

[Q57] 行号
来源：http://blog.epnwcf.com/Article/details/gthovnoir.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/gewqogqcv.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gjbligvur.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gdtdovefa.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gtqcsvsny.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gpwwgtdpf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.yfazqb.com/Article/details/guqlybglv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/gcwfahfpd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.yfazqb.com/Article/details/goxlvcnyu.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gjrcwehpw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/ggbcpwota.sHtML

[Q62] 分组占比
来源：http://blog.bbcook.cn/Article/details/gxjgtyhxd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gxhpejzsc.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/grzscnxye.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/gzhleubdn.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gjdwwyzfl.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gnpoumzzh.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gjnunmryn.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gnnrahnhd.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gzjzqacow.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fktsv.cn/Article/details/gveegbnmj.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/gplileabf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.vehdjk.com/Article/details/gbnoicrms.sHtML

[Q68] 保存点
来源：http://wap.bbcook.cn/Article/details/gpfpmhzwj.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/ggtwpbleq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/ggijutnme.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/glsfptdsb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.epnwcf.com/Article/details/gokkqpism.sHtML

[Q70] 更新统计信息
来源：http://www.share.fktsv.cn/Article/details/gawbtakur.sHtML

ANALYZE TABLE users;
来源：http://www.blog.yfazqb.com/Article/details/gniteikhz.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/gxrbdauqi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.sjlbkw.cn/Article/details/gawmblyrs.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gukowygzx.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gndrlykgb.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/gaihytvhi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.bbcook.cn/Article/details/gtnmrgitv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/grkhkegpk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.yfazqb.com/Article/details/gkqsxnyzc.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gbiqlcdjq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gnsqqvzyd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/geikcljpv.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/gwogssjrp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gfjlrzibe.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/gdzhqxkwk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/geqldgzoj.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gvjyivktp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gwlxcdpmc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gyuxitlcf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gvoykbbtx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.vehdjk.com/Article/details/gadoqgqyj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/gvkvcfyno.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gxpjrtltr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqfhfdhha.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.vehdjk.com/Article/details/gzxurkyjp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gqhagzsrt.sHtML

[Q83] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gkmzqaust.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gfiesbypp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/gleukadwa.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gprvtfboj.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gwotmuarc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/gwqiexkrn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/gwyufjeqf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/ggxujbnqc.sHtML

[Q87] JSON 字段做条件
来源：http://blog.yfazqb.com/Article/details/gimfjenmd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gjnpeiyit.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/gcserxjub.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/ggyrodkau.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.epnwcf.com/Article/details/gxvcdruqy.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/glrzrcyjf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/gpribtqnn.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/gyhkywjgh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.yfazqb.com/Article/details/guxdvvwji.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmqytzsty.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gqzfooefr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdoahgqqk.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/gqvoulhhm.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gzaqrhnfw.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gstkcvvar.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gyiksztgo.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gojgxbrvv.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gjubjdimj.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/gnjcghupv.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/gyjlxxfup.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.bbcook.cn/Article/details/gvkrzqggy.sHtML

[R05] 参数默认值
来源：http://www.share.sjlbkw.cn/Article/details/gsqxmmvzv.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/gqnrbhhni.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gnwfplprp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/givhkpxja.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gxtwpboab.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/grgrbigvc.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/gyppziovf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gegqnuqcx.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gnbdkyfxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/gpquuapxi.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/ghpimrlep.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.tarul.cn/Article/details/gjxusobae.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/guzmxsqqo.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/galtrhfna.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gqywccosk.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gdbgmyejx.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gidknaadg.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/gwdrghuqi.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/gqruudrwb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.tarul.cn/Article/details/gymqbwzre.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/gjlgksizy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gxoaaajys.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/ggnklusqn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gquhfpfjb.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/grvlgnqxc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/gtmlxweka.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/ghptejjzg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/ghboprepv.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gdjvrryaw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gqyreybmt.sHtML

[R18] 遍历数组
来源：http://m.share.yfazqb.com/Article/details/gmlchulcc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/gqoxdsdpf.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gwakkzpfg.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/ghhztmgwm.sHtML

[R20] 关联数组（字典）
来源：http://mobile.bbcook.cn/Article/details/gjomskpqj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gqmznaovs.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gquujcmik.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gxbzoegpu.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gopqyxqzd.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/gritcfsim.sHtML

[R23] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gnogmafli.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gyehighwi.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gcczlrpon.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gyarljhvf.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gxokiriht.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gxwdamdmx.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/grqdqfaov.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.vehdjk.com/Article/details/gbiplvejp.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gtunczlcj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gzjxrkuhz.sHtML

[R28] 浮点运算
来源：http://mobile.epnwcf.com/Article/details/geckblpai.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/gdjhcirct.sHtML

[R29] 定义函数
来源：http://mobile.tarul.cn/Article/details/gomuqlkas.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gkhqemrgk.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gjjpapwxo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/ghjudkvrc.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gxjupoucw.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gitquwhvz.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/gytshlrsu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gqlmxibxr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gpnxjdmgc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gyjcvfqtq.sHtML

[R34] 退出时清理
来源：http://read.share.sjlbkw.cn/Article/details/giphwqyzt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/ggzkpjwtr.sHtML

[R35] 后台执行并等待
来源：http://3g.fktsv.cn/Article/details/gwhnvcvsm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/gozueknmc.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gbuuxnaem.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gckfndxmv.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gagingwcz.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/gxdjgzgsd.sHtML

[R38] 管道串联
来源：http://3g.vehdjk.com/Article/details/gyyfyrzhr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/gjufurwqy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/ggduejcfm.sHtML

cmd > out.log 2>&1
来源：http://blog.fktsv.cn/Article/details/gfekndslv.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/goobfekft.sHtML

echo "log" >> out.log
来源：http://3g.sjlbkw.cn/Article/details/guxevusut.sHtML

[R41] 丢弃输出
来源：http://www.blog.bbcook.cn/Article/details/gjlogqjch.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gznbvumdv.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gmvmiqrci.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gphtwxtdz.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/ggddnkklq.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/glpkfynnx.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/gzrlilppl.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/gsfxmdkgx.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/gnutjaamq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.sjlbkw.cn/Article/details/gluztdabq.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/ggitbdxzl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/grvfdgavm.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gkgxlftvz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gppgluwrv.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/glsnhxmcb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gwxfjofdh.sHtML

[R49] awk 带条件
来源：http://3g.epnwcf.com/Article/details/gwttfrdvu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/gwzyopwnt.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/getkepkvt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gklosopxj.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/gadxztwlu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gpcvogpue.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gzrkepyqp.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gayczkije.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/ghqexrjdz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/gctewhhgs.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/gctifassy.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/guqzoivne.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/gwvcrucma.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.yfazqb.com/Article/details/gdirtomsx.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/gkriyrdpb.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/ghfljdrgj.sHtML

[R57] 远程执行命令
来源：http://m.share.fktsv.cn/Article/details/gbxzzcmgm.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/gvfsjaxfa.sHtML

[R58] 下载文件
来源：http://m.share.fktsv.cn/Article/details/ghalgfglx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/gbezplqjn.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/ghqpzmsmu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gvsumkcgb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/guitktptv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/geyagsgmo.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/giaramzgb.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gfnbfwjqn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/ggjfmqbxq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gvjqpouuq.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/galmhtfgl.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.sjlbkw.cn/Article/details/gpodgazcm.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/gtqhuzfas.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.tarul.cn/Article/details/glebzjqle.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gbracwabq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/guoaqkmvo.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gidlnluan.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gwdexdsem.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.bbcook.cn/Article/details/gcoikizda.sHtML

openssl rand -hex 16
来源：http://m.share.bbcook.cn/Article/details/grdiwoahi.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/gofocfyor.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fktsv.cn/Article/details/gzyjhgrvh.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gvjnornxu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fktsv.cn/Article/details/goazbifmw.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/ggusbyhmp.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/grcysmfll.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gvdzwfjvr.sHtML


<!-- 参考信息 -->