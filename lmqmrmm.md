代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/guajmgmui.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/gisahnjju.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/geqaatuoq.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gdocynyqw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gkngxtxvp.sHtML

[Q30] 分组统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqhxaseu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gbxlugbsy.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gofysqlaw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.epnwcf.com/Article/details/gycgwyvns.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gmbmkoxgi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gjvihceax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/grgwoxieu.sHtML

[Q33] 多列分组
来源：http://m.share.bbcook.cn/Article/details/gvpuljsyq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/gndcecbzp.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gyvdajpuu.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gpsnfwcgs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.yfazqb.com/Article/details/gpozldycc.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/grrbrebpg.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gjymjemsn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gxmirrxgr.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gaustzmgl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gbyawpyus.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gvfmdunon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fktsv.cn/Article/details/gwnlupssr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fktsv.cn/Article/details/grtemkubq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/giqaqymkm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fktsv.cn/Article/details/gitkpuvyq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.tarul.cn/Article/details/gdfilvdit.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/grurljjor.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gurjklitp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gfwjjnuhw.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/gywchcvic.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gcajlzrvt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.yfazqb.com/Article/details/gphublncl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.sjlbkw.cn/Article/details/geiazzcrp.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gygessdxw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.tarul.cn/Article/details/gtsxkrlqi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gzrisgfcz.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gmnxpdenf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fktsv.cn/Article/details/gkwrekyfv.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gqkducelj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gnitkwrbg.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gepigyjxw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gbzwzvvxt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.sjlbkw.cn/Article/details/gasvtolxx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gqawzqmwb.sHtML

[Q47] 与平均值比较
来源：http://3g.yfazqb.com/Article/details/gybgcpxzo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.vehdjk.com/Article/details/gjhpisqvs.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.sjlbkw.cn/Article/details/gjxsspwyp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gkrexjayn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fktsv.cn/Article/details/gzdkisjbw.sHtML

[Q49] 更新单行
来源：http://mobile.sjlbkw.cn/Article/details/gxbpdussj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gntbgealq.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/gbxaqekzw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/gbryuwjic.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/glpjjpxfx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.vehdjk.com/Article/details/gripgrmmz.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/gxbaxdcvx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/grjzlnmeb.sHtML

[Q53] 按条件删除
来源：http://www.share.epnwcf.com/Article/details/gwoinjoov.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/guaikyord.sHtML

[Q54] 清空表
来源：http://www.share.yfazqb.com/Article/details/gwuyhnxnr.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gzsuoatyh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.sjlbkw.cn/Article/details/gimyzafde.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/grnwjbwel.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.epnwcf.com/Article/details/gtbivgzvl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gxfuewbil.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gblqxvyzq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gttbgyfnv.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/ghvdwtxno.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gyevxgqlk.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/ghszhhsdn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gpkpkokqu.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gtalabysa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.epnwcf.com/Article/details/gdxyzhrbf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.vehdjk.com/Article/details/gptgokcvi.sHtML

[Q61] 移动平均
来源：http://www.m.share.epnwcf.com/Article/details/gdnbmlgxv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gnawfginj.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gqtjvdilb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/glvvavqoe.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/ghlqqgjhj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gvqmenezv.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/gqyyfhabx.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/gckagdruj.sHtML

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gtdqsrtdl.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/glixxxcpb.sHtML

[Q66] 行锁查询
来源：http://www.share.tarul.cn/Article/details/gjinkpdal.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/guzwluyvu.sHtML

[Q67] 设置隔离级别
来源：http://blog.tarul.cn/Article/details/gkhholqcc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.vehdjk.com/Article/details/gtaddhgzw.sHtML

[Q68] 保存点
来源：http://read.share.yfazqb.com/Article/details/gxguvvguj.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gsrumvzra.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gmaxgqmlm.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/gnuujlynj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/gmtgrrxmk.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gzbjascwy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.tarul.cn/Article/details/gqmqkcjhu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gfvewiinb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gwdlhgsdx.sHtML

[Q72] 查看索引
来源：http://mobile.vehdjk.com/Article/details/gexamhrax.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/ghakjejff.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gsttehaqt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gpjplusiq.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/gmhzieewn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gjclrfecg.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gnftmcdxx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/gmuhmvmqd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/ggivsscpd.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/gsrnpoctj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.epnwcf.com/Article/details/gstmibylz.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gvkvpzckx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gklfglnpq.sHtML

[Q78] 当前时间
来源：http://baike.tarul.cn/Article/details/gmymqorug.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gcumyxiqc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gszzjnmpu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gtfpgxxrt.sHtML

[Q80] 字符串截取
来源：http://m.share.vehdjk.com/Article/details/gxhndqahq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gadbylerv.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gffnynoav.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.tarul.cn/Article/details/gngrjxrkq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gfugfwign.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gdgmddjzn.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gpukxqfsx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gedzhxygb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.bbcook.cn/Article/details/ghulddmnn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gwqvohflh.sHtML

[Q85] 数值取整
来源：http://www.blog.bbcook.cn/Article/details/gpvzoeemh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.sjlbkw.cn/Article/details/gjgdnsiza.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gwpuzbxrj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gsmzxkrlt.sHtML

[Q87] JSON 字段做条件
来源：http://wap.vehdjk.com/Article/details/gzvbyhtus.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gcomnjrmg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gjtujcnqb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gszgipgdu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gwlooytdo.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/gkwkeuohu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fktsv.cn/Article/details/grqrznllk.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/glvwxskok.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/gwfimlgfc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcczldxwh.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gpjvefhvn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/guxxesldq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gvyqalxib.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/golkaspsf.sHtML

set -euo pipefail
来源：http://mobile.sjlbkw.cn/Article/details/glcsscnwf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/gavvgeqex.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/goiwmlrfl.sHtML

[R03] 只读变量
来源：http://www.m.share.fktsv.cn/Article/details/gcfpurhrr.sHtML

readonly PI=3.14
来源：http://read.share.epnwcf.com/Article/details/ggxlotwrx.sHtML

[R04] 位置参数
来源：http://blog.tarul.cn/Article/details/gmgqyenht.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gezpfizqf.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gulfdjutl.sHtML

name="${1:-default}"
来源：http://m.share.yfazqb.com/Article/details/gzclyhpln.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/gkredjhfa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gcdndgktb.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/gmyzraksf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/gxtrmluix.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/grvjcepac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gbwioooez.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiaojkxs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gtsncfacd.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/gocaqygbr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/gyqzexpcu.sHtML

[R11] case 多分支
来源：http://blog.sjlbkw.cn/Article/details/gfcrklakf.sHtML

case "$1" in
来源：http://baike.bbcook.cn/Article/details/grepxhqzr.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gdgfeqxbf.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gjwljnwkk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gdnawkbok.sHtML

esac
来源：http://3g.bbcook.cn/Article/details/gvhzlvfwj.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gdxsefnfn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gkdkpwvrv.sHtML

[R13] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gomvopyeq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/grfzylbrp.sHtML

[R14] C 风格 for
来源：http://wap.tarul.cn/Article/details/gefaiovbr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gzfaffyrc.sHtML

[R15] while 逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gtgyvcrvm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gzmmiquuc.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/gbkdpsffd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/glyawjdxe.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gkcjoxoib.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/ghnwsgzoq.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gmflczyiv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.bbcook.cn/Article/details/gplvttcvi.sHtML

[R19] 数组长度
来源：http://wap.tarul.cn/Article/details/gpoukdypa.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gzvfnnnuk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/gcurnurlj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gkzuimkyh.sHtML

[R21] 字符串长度
来源：http://wap.fktsv.cn/Article/details/guizifjwz.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gbktbbhvr.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/ggxjonzed.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/guidkqioa.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gsgpvgehg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gbkszrgbe.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/grnncbdjf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gmngegsla.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/gusyyfpin.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gwawcogkh.sHtML

[R26] 命令替换
来源：http://www.blog.epnwcf.com/Article/details/gdqyauvxw.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fktsv.cn/Article/details/geduieebz.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/genicbelu.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gcbtwsygj.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gmqkzktpc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gtkgzoace.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/gxqydmzuo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gvydkymyc.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gtaarfmxh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.epnwcf.com/Article/details/gxawthvnd.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gcvrnxqaf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/grbahjhmy.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/grxklipoe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gsfferifa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.yfazqb.com/Article/details/gabyfbgnl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/gqyllxplo.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gjxvpsayi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gyrkibftd.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gaazfffcu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gzhfaumlx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.tarul.cn/Article/details/gnfzrgzqt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/glajlbvfj.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/gpospaaun.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/goudhpmqb.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/gwaacvvup.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gvankrkmy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gxdoxbqyf.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gdygegbwf.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/gtueafkhn.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/gvzxxuisk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gbymjvgew.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/gfpaldbpt.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/gslmvtqwv.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/ggjnmnrnb.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/gjpldikno.sHtML

find . -name "*.log" -type f
来源：http://read.share.tarul.cn/Article/details/grjjltpfs.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gjbsysvtx.sHtML

find . -mtime -7 -type f
来源：http://read.share.bbcook.cn/Article/details/gsvbiybkk.sHtML

[R45] 批量删除
来源：http://wap.tarul.cn/Article/details/gglurenpg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gatwoghql.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gasvllvhu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gdsfmrpvr.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gzqqtnnfo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/glixnvkdj.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gbxyewean.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gmpbztjuf.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/gnffdajxd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gjoijiczg.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/gjwvsdftk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gqgeinkrd.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/ghvnnevgv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/govaxwihs.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gvyfkmizh.sHtML

wc -l a.txt
来源：http://read.share.bbcook.cn/Article/details/gtqzrqmle.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fktsv.cn/Article/details/gnwezdyni.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/girnailjy.sHtML

[R54] 比较两个文件
来源：http://wap.fktsv.cn/Article/details/gndnslgue.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/gekbxwzlb.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/gqgwwkqxs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gtkgbdzxb.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/gdphwpzpo.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gykdczhte.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/ghzyihpjj.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/glojedkgm.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gubrsdrjo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/gyxzdkpmi.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gzqkmteqb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/gyjbqaycf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gucqnpkbb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/gxfxufuqx.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gleyqmzpg.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/gctgvcddw.sHtML

[R62] 找最占空间的文件
来源：http://blog.epnwcf.com/Article/details/ghatotfix.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/ghjpkxnwo.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gnzwfckpm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/glkuseumd.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gyyshuarg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gjrrfepio.sHtML

[R65] 查看端口占用
来源：http://mobile.vehdjk.com/Article/details/gdssfizwx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gdlyjhkbt.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gkrboqtqh.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gtswixguc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/gtzzveknh.sHtML

openssl rand -hex 16
来源：http://3g.yfazqb.com/Article/details/gqylakygv.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gtmxzylil.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/ggmezbjkw.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gwqoofxkb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/gxiqcracv.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gfrxdugft.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gknfxhznh.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gcjokbceq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/gfqzlxnfd.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gbeuujsap.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gbohqgpnp.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gmluvbrxe.sHtML

split -l 1000 big.log part_
来源：http://blog.fktsv.cn/Article/details/gsicktqyi.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gjpwqtscp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/gdenyzrge.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/guolgrgsk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/ghukqxfvf.sHtML

[R76] 使用临时文件
来源：http://m.share.yfazqb.com/Article/details/gvhrkwdqz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/ghcadpcqc.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/glqlcyavx.sHtML


<!-- 参考信息 -->