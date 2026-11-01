代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.sjlbkw.cn/Article/details/gfkspclbh.sHtML

[Q24] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gvtjkypxd.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/gcbcanygu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/geurexfoz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fktsv.cn/Article/details/gvojvfmme.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gtftsdzjn.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gxcecbcph.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gajafckuo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gegtndruh.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gjydhkpuu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gghclrblz.sHtML

[Q29] 最大最小值
来源：http://www.m.share.tarul.cn/Article/details/gkncwtjsx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gvzkzjoew.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gucnwamuy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gbrwqzvcp.sHtML

[Q31] 分组后过滤
来源：http://www.share.tarul.cn/Article/details/gdfbethpf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/gnzgfnugf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/glqzuvicc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gshzdxsro.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.tarul.cn/Article/details/gtvaykkss.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gyyjnazbj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.tarul.cn/Article/details/getujpwas.sHtML

[Q34] 每组取第一条
来源：http://m.share.epnwcf.com/Article/details/ggwivbvcv.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/gthinnmhr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.vehdjk.com/Article/details/gwvufzecw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gvhcfaegl.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gddtbtitz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeaxcjhg.sHtML

[Q36] 左连接
来源：http://blog.tarul.cn/Article/details/gmsbhajdz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gmcxledyv.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/gthnyjgux.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/grbnphpyx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gwdohlhzw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/gupwpmdjy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gowngvojm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/gwaqriswa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fktsv.cn/Article/details/gwhvjwwwj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gdofnqlaq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/gozzstnin.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gsfkvehkm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.bbcook.cn/Article/details/govpbwxdu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fktsv.cn/Article/details/gekenyflm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.bbcook.cn/Article/details/gbeurdsqn.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/glwyrtsqy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gsalsiely.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/gmxaiuols.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gaxfmqyio.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gandlcvlz.sHtML

[Q44] IN 子查询
来源：http://m.share.epnwcf.com/Article/details/glkayvguc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.tarul.cn/Article/details/ganiqrckx.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gjylntngl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gnbasorqx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/gabvwqefw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gwuckohao.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gitiupiwz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gwzmrbimq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/gihyxnqum.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gmpgnwcni.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gsgpzloue.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gueefuqmf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/guoefqndl.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/ghzoopsqq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gmnrmndif.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/giowvawhy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/gngwfupnp.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/ghozbnqdj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gqswhuvsq.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/grslbxwap.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/giyjxmiea.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gupnliamr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/guioowxmd.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gjfrsyjvw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gfzjfjpdb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gwxamtyma.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.vehdjk.com/Article/details/gmxkmbmem.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/ghtgtpefv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gkpfhwrlh.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/gvhtsiybq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gkznestbr.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gksxqhprd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gyxuysdun.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gmqnxikrx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/guqqzvslt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/ggpqmcplx.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/ghzcojjgc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gbaaciiac.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gjdrbblvd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/guugnlqtx.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gcjhcauwc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/gpejztwrc.sHtML

[Q64] 提交事务
来源：http://www.share.tarul.cn/Article/details/gfpkuguhe.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gtkyxaozh.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/gillktwvq.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gnvlycnew.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gbxmwitax.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/giccshaxh.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcfqaers.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fktsv.cn/Article/details/gilaexpda.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/gpuximynj.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/gbxqovpif.sHtML

ROLLBACK TO sp1;
来源：http://m.share.bbcook.cn/Article/details/ghlkswmkf.sHtML

[Q69] 查看执行计划
来源：http://wap.bbcook.cn/Article/details/garvjrqcd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/gyekfmocq.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/gbmvkwovp.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/gddxsdroy.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/gzwsatlfy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmjgfvqt.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gnhhvojbc.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gtzjlfmbc.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gidwfydub.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/grqsczzhl.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gyojrxfje.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gzzzpnufc.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gliubqsvk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/genytjput.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gioxnalcm.sHtML

[Q76] 按天统计
来源：http://blog.epnwcf.com/Article/details/guuayrlwm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.yfazqb.com/Article/details/gkrzuomoo.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/guejwbhgj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/gkbqmvhds.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/ggmnjawfc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gxdvzbktt.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/gisoioldl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/guuwdqxtu.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/gxqzgemma.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gwzuwstkj.sHtML

[Q81] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gveqvhexr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gwbwoitlx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gwdnkpnjp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gagplgvqw.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gexlruimh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gzthxwwtf.sHtML

[Q84] 去除首尾空格
来源：http://3g.epnwcf.com/Article/details/gxmohdczy.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gdyenhrpq.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gupbhqhwo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gjotrpuit.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/gnizexhdd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gunqzrael.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/gzlhjnzjr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/geuivqzbv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gkukrceiw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/ggpzgfarz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gkqrnvyll.sHtML

[Q89] 判断表是否存在
来源：http://m.share.tarul.cn/Article/details/gxfuqtbiw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/gbbkcxdli.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gksqqspbz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/gscqrlwyo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gygfdqavf.sHtML

R. Bash 专题
来源：http://www.m.share.bbcook.cn/Article/details/ganlzaflc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkgovajji.sHtML

[R01] shebang 与严格模式
来源：http://wap.tarul.cn/Article/details/gtepmrgwi.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gbqivubcf.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/gkzzhnsij.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gwtcatghj.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/garwcezuw.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gmmqmyqmc.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/gfxcvvdtc.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gnczpmpgb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/gmzlhwqku.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gpvsbkqvm.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gzaiyauxe.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gjvxtipzs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gztboskdo.sHtML

[R07] if 判断文件
来源：http://www.blog.bbcook.cn/Article/details/ghyccypyf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/gyajrtihv.sHtML

[R08] 数值比较
来源：http://www.blog.bbcook.cn/Article/details/ghtrbufja.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/guebalenj.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gzciyirpd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gzbwsvhhw.sHtML

[R10] 正则匹配
来源：http://blog.sjlbkw.cn/Article/details/gsornuuod.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gbrxihxkw.sHtML

[R11] case 多分支
来源：http://m.share.bbcook.cn/Article/details/gwuelxueb.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/ghlphblwe.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gwfgpstkq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/gjwvxgifn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gcofbtaas.sHtML

esac
来源：http://read.share.bbcook.cn/Article/details/goklykuub.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/ghqoprnex.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gajbzcjpk.sHtML

[R13] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gjomgrbez.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gnjxbblvz.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gfccwcfzd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gwptslzqt.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/gmimdiefw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fktsv.cn/Article/details/giafcvivc.sHtML

[R16] until 等待条件
来源：http://blog.vehdjk.com/Article/details/gdingzrat.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gsyamhrsz.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gsrihemqf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/gejstzhjm.sHtML

[R18] 遍历数组
来源：http://3g.sjlbkw.cn/Article/details/gdvzivewt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.yfazqb.com/Article/details/gbrsgybmx.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gxafnleie.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gdaudbfkp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gkxaccbly.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/gdfzgtzvb.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/gepjriiax.sHtML

echo "${#s}"
来源：http://www.m.share.tarul.cn/Article/details/gohdlkwyf.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gkxdhanfk.sHtML

echo "${s:0:5}"
来源：http://mobile.vehdjk.com/Article/details/grfdupwlm.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gkvkjrxxd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/geziyttwy.sHtML

[R24] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gawpvswcv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gsmxbgbxt.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.sjlbkw.cn/Article/details/gnejujsqp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/gokxxhaqk.sHtML

[R26] 命令替换
来源：http://mobile.tarul.cn/Article/details/gcokjpfja.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gtprislfg.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gsfnnxhyr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gmijqkjpc.sHtML

[R28] 浮点运算
来源：http://wap.epnwcf.com/Article/details/gkgukaknm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/guisehnpf.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/grdzcodmf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gycdkuzsy.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gljjggwwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gpnsvwmgi.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/glcxjhylc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gxetgergd.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/ghfzrgrrx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gyprvyaus.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/gwmxbcepl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gtonbnleh.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/garzrgzrr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/guoplztnv.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/ggqzvnmzc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.tarul.cn/Article/details/gasczrpsr.sHtML

[R36] 并发执行多个任务
来源：http://m.share.vehdjk.com/Article/details/gvvxfwayx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/goxbobazg.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gjpfxpefm.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/gnapnsugp.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/ghlrolhjn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/gavjgdixf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.vehdjk.com/Article/details/gyxqztvzd.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gcbnqrrvr.sHtML

[R40] 追加写日志
来源：http://mobile.epnwcf.com/Article/details/gjzhkzdnp.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxgcjlug.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gkbrbfnpt.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/glwafqouw.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gebpxrtrg.sHtML

wc -l < a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxznkhus.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gzfmmxldn.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gifboirtl.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/gfxmhabnb.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gdfikzzdj.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/gmyjlagpv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/gyoumsavd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/geqldshuf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gtwglonba.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gqbcmjbiq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gmobhefvn.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gfaieqoxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gtsrdawkd.sHtML

[R49] awk 带条件
来源：http://read.share.tarul.cn/Article/details/grxstmxik.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.sjlbkw.cn/Article/details/ghdarjdtb.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gwvzjtduc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gjbqsbcte.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fktsv.cn/Article/details/gorphgyry.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.tarul.cn/Article/details/gnxvhjbsf.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gbbuwrxrt.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gbayusift.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gzejojkfw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.epnwcf.com/Article/details/gcmggqcae.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/gyrwvebgk.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gdswtprwb.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/gqgnzhpal.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.vehdjk.com/Article/details/gmgsthahl.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/gfiptzmrl.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/glytmmamy.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/grrjpzyvr.sHtML

ssh user@host 'uptime'
来源：http://read.share.sjlbkw.cn/Article/details/gagovgvlu.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gicxdzgaa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/goioicgwd.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gouojatvx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxjigfjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gikugzwqu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gdtjzmtqu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.bbcook.cn/Article/details/gisuhaopp.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/gwtyymwwx.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gpnpurvoe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gskkxmkvc.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/grsvbvlgh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.tarul.cn/Article/details/ghfkweryc.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gtliwtdnl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/gemdkikbq.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/grkkhdlyj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gwwvdkoti.sHtML

[R66] 定时任务
来源：http://wap.fktsv.cn/Article/details/gpnpjxyem.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/getvpjrjj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/gjzpbvkko.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gpvlydkdf.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/goqkqhgpj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/gkwajymuw.sHtML

[R69] 生成随机密码
来源：http://baike.bbcook.cn/Article/details/gukthhftm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gtznsorzq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/gcmhtbkef.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/gwckmfgbt.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gwrzlgkll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gnxunvkgk.sHtML

[R72] 等待端口就绪
来源：http://read.share.yfazqb.com/Article/details/gwovciqjq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/ghwmtqfwc.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/gyisnnfcw.sHtML


<!-- 参考信息 -->