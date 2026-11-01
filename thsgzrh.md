代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fktsv.cn/Article/details/gugzghatm.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gusqcikvq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gciqklepv.sHtML

[Q29] 最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmnpeakm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/govosntyj.sHtML

[Q30] 分组统计
来源：http://www.m.share.epnwcf.com/Article/details/gdexcbvvx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gdxovoifo.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/gujpmzruk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gynzijvap.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/grciqgjvg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/glldsjjkh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.yfazqb.com/Article/details/ggnpoqqon.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gkritzxls.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gzajtcbzh.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/gxyzltbwc.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gyipkmiug.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.vehdjk.com/Article/details/gpvagweme.sHtML

) t WHERE rn = 1;
来源：http://baike.bbcook.cn/Article/details/gtdlfbord.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gwchjraiw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gpqmewwny.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gowusnfsd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/grnwkadaa.sHtML

[Q37] 右连接
来源：http://read.share.tarul.cn/Article/details/gznzypabk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gkekjvxpe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fktsv.cn/Article/details/ghdrcagji.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.epnwcf.com/Article/details/gztkchagt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.epnwcf.com/Article/details/gtmkquoys.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gqpajvqvj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.sjlbkw.cn/Article/details/gvuixrjur.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.yfazqb.com/Article/details/gamevrfpb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/grabcbeyo.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gdsmrvxae.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.bbcook.cn/Article/details/ghvhcvxpm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/garqoptlc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.yfazqb.com/Article/details/gxrygboaw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gplakwqab.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/gfmndtweu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/gkrsdjwqx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/glxukrgpl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.sjlbkw.cn/Article/details/gjvbbwyug.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gibzyiljq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/ghcanpbsn.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/gylohybij.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/giifcuqwa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/gpcrycdsp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gijclcnzj.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/giuniegir.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxchvlarn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gdarrlfzi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gqbdblxtx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/glaggcmnc.sHtML

[Q49] 更新单行
来源：http://mobile.epnwcf.com/Article/details/grwvnpopt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gzfywftff.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gultsmqvh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gscdlzbjp.sHtML

[Q51] 用子查询更新
来源：http://m.share.yfazqb.com/Article/details/glbnpnenb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gofngxnhb.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/glkkyuvpi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gglpeacdd.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/ghpqiestc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fktsv.cn/Article/details/gtbqevpih.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/glnrtaijk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/ganzsqjzr.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gxkbrnthp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gdtgqxphi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.vehdjk.com/Article/details/gdlqxmqkb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/gxrboqdgw.sHtML

[Q57] 行号
来源：http://www.m.share.tarul.cn/Article/details/gtehmidge.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gtaidlgyo.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gbckziezq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gyceyzkhh.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gevzhaiic.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gttpcmqhc.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gbihvorxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/glbecdsjn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/glpmrgime.sHtML

[Q61] 移动平均
来源：http://baike.yfazqb.com/Article/details/gjpirdttt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/ggdmrllik.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/ggyekzxtm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/guojbipco.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/goimfgfjz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fktsv.cn/Article/details/gsrriwacr.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gwdwsveru.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gqtkckfvi.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gsslbjsmi.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gbvmqwhng.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gttcbxqwt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/glywygkdj.sHtML

[Q67] 设置隔离级别
来源：http://wap.vehdjk.com/Article/details/gdgdbugdy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/grfxenagg.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gsofwgiit.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gwxerifsr.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gszbwzkfq.sHtML

[Q69] 查看执行计划
来源：http://blog.tarul.cn/Article/details/grmprvjpk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.sjlbkw.cn/Article/details/gnnssqdiq.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/gmzrrhssp.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/goukgswhx.sHtML

[Q71] 查看建表语句
来源：http://wap.tarul.cn/Article/details/gozxjxaac.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gaxiluzty.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/gkdaybtwu.sHtML

SHOW INDEX FROM users;
来源：http://baike.tarul.cn/Article/details/guwbbkwjs.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gcuzxsagg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.bbcook.cn/Article/details/gohimjrmv.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/ghxyomeru.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gkwkuidhu.sHtML

[Q75] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gatfdtghw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gfgmwxmsp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gslpjxkmj.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/gohdoguut.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gjgbaxaln.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/gfbzrdakn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gxlbqcsky.sHtML

[Q78] 当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gugbrqspf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gvihndcro.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/ghlpmpxxf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gykwfhtfx.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gfmydgyeu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gfmxowfgx.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gcucnvfkm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gslgokvqf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gjztgvops.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gzdvnzzkg.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gcmoswtli.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gkodzbhlp.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gmuphunnb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gnmpyjewu.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gniahnkox.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/gqwnhgojc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/gtvememqd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.bbcook.cn/Article/details/gfjxozypx.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/gsnluimpv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gfvdcgtcs.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/gyrkjdrxw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gkefagpjd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.bbcook.cn/Article/details/gktzynylq.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/gmjeicapy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.bbcook.cn/Article/details/guhyxukkl.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/glrprzgvu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/gfkfvgoay.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkmtggvwa.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gvustdicl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcblyowxg.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/grxmvuqco.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gqhtzidje.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gialhgbfm.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/gaspegbfz.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/gznxskmeg.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gfsaccibs.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/giswenqzt.sHtML

[R04] 位置参数
来源：http://mobile.yfazqb.com/Article/details/grnylrpsk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/ghcacimps.sHtML

[R05] 参数默认值
来源：http://blog.tarul.cn/Article/details/gqhagefzn.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/gbpocbiku.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gdtfddrmp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gqohbxlbr.sHtML

[R07] if 判断文件
来源：http://blog.yfazqb.com/Article/details/gsvahnzun.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.tarul.cn/Article/details/gefjjqsey.sHtML

[R08] 数值比较
来源：http://www.share.bbcook.cn/Article/details/gfkfrwgrt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.bbcook.cn/Article/details/gisxgzlir.sHtML

[R09] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/grezilbhp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/govlrbtkx.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/ggmgdmyco.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gsilhpffd.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gzkrcmhyy.sHtML

case "$1" in
来源：http://blog.sjlbkw.cn/Article/details/gsnzeelsp.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcsibwsr.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/gryasnaze.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gavvtyfli.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gvuyokiop.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/ghpqzqopt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.yfazqb.com/Article/details/grplfzsuf.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gjrdolteb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gbtwfbsec.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/gunfqzicx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbkukyso.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/glufqyycb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/guknkfztz.sHtML

[R16] until 等待条件
来源：http://mobile.bbcook.cn/Article/details/gsepqwlzv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/grhtgibdx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.yfazqb.com/Article/details/gcuylbmge.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gqwdfdsij.sHtML

[R18] 遍历数组
来源：http://www.m.share.epnwcf.com/Article/details/gchxlptqb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/gfribaygs.sHtML

[R19] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gyxvgyshf.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gxzwojccr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gpatmbzqw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/gciqoscds.sHtML

[R21] 字符串长度
来源：http://wap.tarul.cn/Article/details/goroqgcqs.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/gdithxqoe.sHtML

[R22] 截取子串
来源：http://www.share.tarul.cn/Article/details/gnxcaomqp.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gfwkfhrsk.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gpauowtei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/glvzavnyf.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gbeapxwcx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/gwmdxwlmv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/gtjhplkaj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gqfuannnz.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/gjwrbkhmk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gusrnebnb.sHtML

[R27] 算术展开
来源：http://3g.sjlbkw.cn/Article/details/gcapobkds.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gossnuobe.sHtML

[R28] 浮点运算
来源：http://blog.tarul.cn/Article/details/gkvokxnrq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gkexjgdlw.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/grroavuoe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gjqcbnjcg.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gukqscfoe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gxwgagzpt.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/getfntups.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/grvzjgnox.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gjqmnggil.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gyzgzfbff.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.vehdjk.com/Article/details/gwkvwcplx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/gaqhljfpt.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gjktbyqmt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gwkwsxjyk.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/ggwvlolbc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gnwrinusj.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gygmilbpx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/gjxgifvmt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gbchjpguv.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/gglzmmztl.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/gsaztjwxs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gstpvhmub.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gomwfsngo.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/grmxahsvi.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/ghgnaancr.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gmulxlaei.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/ggiubjzmh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gqpyqjivq.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gqbjpwexp.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gnqyvehii.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gqucwftdz.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gfmjhpalf.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/gusbogdgj.sHtML

find . -mtime -7 -type f
来源：http://mobile.tarul.cn/Article/details/gbmyuufbr.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gzotewezn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gqzboabku.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/gluircjbe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/glsnjqsvo.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/ggjvqruxt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.vehdjk.com/Article/details/gumohasjp.sHtML

[R48] awk 取指定列
来源：http://m.share.sjlbkw.cn/Article/details/gemevjpvl.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gendfxmof.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/grifpjtgk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/gjlnpqtqf.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/gzqnmsjkv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/ghoedqvrc.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/gwidvcdlq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/ggetxmzky.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gejcbyibg.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gpdlspbqu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/gnuyjbzmc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gkyneplav.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/gzmjppibs.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/goeysdejd.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/gflfqpksc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.vehdjk.com/Article/details/gdubvlriz.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/gqnpdczyc.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gtpygsaph.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gljyusxoq.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gxnyjjjso.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/glfgzlpsm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/goisxtihq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gjunvhqha.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gkxqoyxje.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gsucszceg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/giyfuehkr.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gtsfcmjto.sHtML

df -h;  du -sh *
来源：http://3g.sjlbkw.cn/Article/details/gztdkonka.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/gtejkkytq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fktsv.cn/Article/details/gtcjrdvjx.sHtML

[R63] 内存与进程
来源：http://mobile.vehdjk.com/Article/details/gjlfqtika.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/grsouikqv.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gjlpkkvdc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.sjlbkw.cn/Article/details/gbddprdrb.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gotkvodwc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gzgaaeshk.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/gbabskolp.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gzetkuocb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gzbmndmhq.sHtML

openssl rand -hex 16
来源：http://blog.fktsv.cn/Article/details/gtjyxcmtz.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gubvulbjn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gsgtvgtmx.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/gzalvrkmp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/gszplfbhv.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gremjfvtl.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.bbcook.cn/Article/details/gosqjgjck.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/ggtrazkln.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gkfajwzpc.sHtML

[R72] 等待端口就绪
来源：http://baike.sjlbkw.cn/Article/details/goqjsagdc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/glevrhcvi.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gljfwnxcr.sHtML

split -l 1000 big.log part_
来源：http://www.share.fktsv.cn/Article/details/gankblcwj.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/glmtntdkz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.sjlbkw.cn/Article/details/ggzrwutui.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gvwqkgxyc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gqrpbdxtl.sHtML

[R76] 使用临时文件
来源：http://3g.vehdjk.com/Article/details/gggxmezqt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gwxnjjmcd.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gamwstuac.sHtML


<!-- 参考信息 -->