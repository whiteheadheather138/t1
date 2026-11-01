代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/guhncslsw.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/gaaglxtkm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gzgdfblnt.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gsrqcnqrh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gfosbaxfn.sHtML

[Q30] 分组统计
来源：http://wap.tarul.cn/Article/details/ghyqyncme.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gtkgrfiqc.sHtML

[Q31] 分组后过滤
来源：http://read.share.bbcook.cn/Article/details/gamiqaqok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.sjlbkw.cn/Article/details/gorkvpsrn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gqokxponx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gdhthuwug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.bbcook.cn/Article/details/geuiuamsp.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gqdeffkqm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.bbcook.cn/Article/details/gvxansvvy.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gwfhsyujs.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gjcqzszuq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.vehdjk.com/Article/details/gttngfdhl.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fktsv.cn/Article/details/gzdbaxhlr.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gcelqnoiu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gybhfxlib.sHtML

[Q36] 左连接
来源：http://baike.fktsv.cn/Article/details/genqljsut.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gzcatkyck.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/govwkouai.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.tarul.cn/Article/details/gkbnihgvn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/gevmgohsx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gdhislnbs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gfkjgtdac.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gugykypvz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gnjvzyzwd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gfsgrfmao.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fktsv.cn/Article/details/gzsvkvtil.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gkusjrgnw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gdtmghntp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gwaqfpbxf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/gaqmlnztu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/giwgtxerk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fktsv.cn/Article/details/gjlhigjil.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gkpsqdpfp.sHtML

[Q43] 标量子查询
来源：http://wap.tarul.cn/Article/details/gpnkolzuf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.vehdjk.com/Article/details/gpaizznhh.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gyiycecck.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.epnwcf.com/Article/details/gabqajjzx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fktsv.cn/Article/details/gznuhczbp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gxdpdhllg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.bbcook.cn/Article/details/gsppcqbdj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gtpommjwp.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gjiqlhqqo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/gltyftadl.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.bbcook.cn/Article/details/gynnpgfdb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/gydjbtrbk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fktsv.cn/Article/details/gzizthyql.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gmjnxffjd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gmbhvchqy.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gwryxkfvt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/geywxgboc.sHtML

[Q51] 用子查询更新
来源：http://3g.bbcook.cn/Article/details/gtidyzixs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gghxbpzcs.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gunitzquq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gvydqcmho.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gsykgqaeg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gurbjzsxg.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gcktibjjk.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fktsv.cn/Article/details/gwgdclrtj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.bbcook.cn/Article/details/gmbddyyre.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fktsv.cn/Article/details/gioapkekl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/gwxcjnwgm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gbbkzrlrv.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gkdptsjkf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.epnwcf.com/Article/details/gqxzgwbca.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/glqxpyajg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/gdcexsrjz.sHtML

[Q59] 分组内累计
来源：http://m.share.tarul.cn/Article/details/glgxdwfec.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gajrlkjtq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gtbekhird.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gtqklnwxq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gtqioucje.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gtqlttjjg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gorshxbsq.sHtML

[Q62] 分组占比
来源：http://m.share.yfazqb.com/Article/details/gamronqxn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/grlxsnhys.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/glpsgdoux.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gayyjdsgm.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gexznhvlp.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gaejupkux.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gycibavla.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gefomjryu.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gvczkkjuv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gxbccwvqs.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/gsjquoawe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/gckpzadwy.sHtML

[Q68] 保存点
来源：http://3g.yfazqb.com/Article/details/gosvcgafi.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/godvdqqog.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gydatxrsa.sHtML

[Q69] 查看执行计划
来源：http://www.share.epnwcf.com/Article/details/gjrurhpya.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.bbcook.cn/Article/details/gddunmpog.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gfscvljct.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gddawvquu.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gyrwnmiab.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/guwcgntdc.sHtML

[Q72] 查看索引
来源：http://3g.epnwcf.com/Article/details/gxgokmcwr.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ggfylarju.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/gqoknukxt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/grrmxgqzz.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/glhxjpldd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/glzdzjfbs.sHtML

[Q75] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gjjamoqoj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gofdylair.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.tarul.cn/Article/details/gdeieyhpb.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/gekipxbtz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/ggdkctjon.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/gdnsgydly.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gmvggywjp.sHtML

[Q78] 当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuqfmngt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/gyjukbcbi.sHtML

[Q79] 字符串拼接
来源：http://3g.bbcook.cn/Article/details/gnioqyzbs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gxyljisqf.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gvurwbucc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gdoxtxpjd.sHtML

[Q81] 字符串替换
来源：http://3g.bbcook.cn/Article/details/goifetfwu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.vehdjk.com/Article/details/gxbbbneol.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.tarul.cn/Article/details/gqgpbnrwv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gkvrakajk.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gxowfdncb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ghqyequku.sHtML

[Q84] 去除首尾空格
来源：http://3g.tarul.cn/Article/details/glsrcozqg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gaskojfrs.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/ggvhxyvfl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/gheotzzlr.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gacmatlxs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/ggsdadsxa.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/glfqpppxs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.sjlbkw.cn/Article/details/gnffvgzos.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.vehdjk.com/Article/details/gxzwssrqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gvanritjh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.vehdjk.com/Article/details/gxgtmmqsh.sHtML

[Q89] 判断表是否存在
来源：http://www.share.bbcook.cn/Article/details/grimtxudi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gstolvkqn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.bbcook.cn/Article/details/gzprkhwmj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gqbwgscju.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glrosqtmk.sHtML

R. Bash 专题
来源：http://wap.yfazqb.com/Article/details/gkdpfshnn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkmwxndqm.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gprrvrmvq.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/gdttwmtsv.sHtML

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/gccosaqry.sHtML

[R02] 变量赋值与使用
来源：http://wap.tarul.cn/Article/details/gjhrjzenc.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gfmpewxxg.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gczkuhyvv.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gxoenkonv.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/gcurmbwwp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.epnwcf.com/Article/details/ghsawvbeb.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/gcneccysb.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/ghkliludu.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/gvgmuplcx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/glmeppkno.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/ggsmtvvtm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gfktzmuzp.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/grbewstac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fktsv.cn/Article/details/gwtlqenvp.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gvakabofm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gaivdxpdh.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/goencpqzw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/givwrwepj.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gyaviktey.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gmdvgygvq.sHtML

start) echo "启动" ;;
来源：http://baike.sjlbkw.cn/Article/details/gzchntdmg.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gmqkvsmsa.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gbyfpnior.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/glwgwdniy.sHtML

[R12] for 遍历文件
来源：http://www.blog.sjlbkw.cn/Article/details/gvivpeoir.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.yfazqb.com/Article/details/gijfdcnzw.sHtML

[R13] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/grhnfhmwu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gbzxkyjqg.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gxifztiez.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gnixppzqk.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gxjxnamhe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gldxurvzr.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/gdauzocjt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gkhyzffum.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/gqvnjvuzz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gqencchsz.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gxeewupen.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gswhvhxhw.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gfykguytw.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fktsv.cn/Article/details/gnhavmrpp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gailyjpzi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.epnwcf.com/Article/details/gtexldvnb.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gfnyigefu.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/glyfspyrc.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/ggkfykrgk.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/gmuemrggo.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/guwyvjzoy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.sjlbkw.cn/Article/details/gbwlwdlko.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/guksjjiaz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.epnwcf.com/Article/details/gcxyascsc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gncoykqtf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/gnelgjgdu.sHtML

[R26] 命令替换
来源：http://mobile.epnwcf.com/Article/details/gmavdagtv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.tarul.cn/Article/details/gksglirtd.sHtML

[R27] 算术展开
来源：http://blog.epnwcf.com/Article/details/gwiusklqb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/gitcdwfct.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/gieequzch.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.tarul.cn/Article/details/gclgwoniu.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gthcgcpfs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gbauxrqgi.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gughiqmaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/glynjlydb.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gfsvuoylg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/gbchyepvi.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gwkvmzvwu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gsvvglrlg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.vehdjk.com/Article/details/gakksslms.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.epnwcf.com/Article/details/gznlaxryd.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gruufqpuq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gjgynjpuf.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gbptdabmi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gehzlrcta.sHtML

[R36] 并发执行多个任务
来源：http://mobile.tarul.cn/Article/details/gjxmsgfsr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.sjlbkw.cn/Article/details/gamwkdhwj.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/gjeonnrtq.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/gechftbiv.sHtML

[R38] 管道串联
来源：http://baike.sjlbkw.cn/Article/details/gouhjmrry.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gjgihrcum.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gzpvzvwxe.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gfeohukqq.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gmozeyvyd.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gwddjaubk.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/gyzytguke.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gnqwgvlgz.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gakrpbikj.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/gcpwkuabj.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/gulatqfyw.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/gqlurhgco.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/ggzfgmxpd.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gdxrqssyp.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvkyvrsw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/glrwoqfua.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gthralwes.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.epnwcf.com/Article/details/gitfoaots.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gumgavlqz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gsiyihsmk.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gdlxncvfc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gkdlbffmx.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gldlvgzxs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fktsv.cn/Article/details/gborlqouw.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gvkgxdaku.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/ghafhewzr.sHtML

[R51] 排序去重取前几
来源：http://baike.bbcook.cn/Article/details/gektkbkyf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/grwsmttdl.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gdkyaljui.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/gmwbeidee.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.tarul.cn/Article/details/gojjvasqn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/guxijggdk.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gnxmsrref.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/geidymnhb.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gucqbsxdo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/gbggobmlq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/ggjkcthzg.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/gaufdyhhf.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwnjvqxm.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gbfefcpei.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/gddkszotr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.tarul.cn/Article/details/gswyjidjr.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/grbllcygl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.yfazqb.com/Article/details/gbojvemcm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/giohhdmah.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.yfazqb.com/Article/details/guvuwpdjo.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/glqbvzrbw.sHtML

df -h;  du -sh *
来源：http://m.share.fktsv.cn/Article/details/glvfnfqgg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.tarul.cn/Article/details/gfadzvbup.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/grxrmzgqb.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gezencbui.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/gtghxxtdr.sHtML

[R64] 结束进程
来源：http://www.share.tarul.cn/Article/details/gqafdbxvg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gwxajauxc.sHtML

[R65] 查看端口占用
来源：http://www.share.fktsv.cn/Article/details/gnohqiemy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gsjknloex.sHtML

[R66] 定时任务
来源：http://m.share.tarul.cn/Article/details/guvvobmyn.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/guxofmnhw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gogmggkgy.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gwtkbeihp.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gghevqhmc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gaiyolbzy.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gvityjrvf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/gbujgwbku.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gjziydecw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gmhvaqspn.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gttqssxbi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.yfazqb.com/Article/details/gcnjsvqrr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.sjlbkw.cn/Article/details/gbvmiictb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/geifjcrob.sHtML

[R73] 分割大日志
来源：http://baike.epnwcf.com/Article/details/grvoxpcvp.sHtML

split -l 1000 big.log part_
来源：http://www.share.bbcook.cn/Article/details/golmjpmlg.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/ggidydpfm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gaufdsjhb.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/ghhimcnlq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gvatondaa.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gciyxtbjg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gkaihifpq.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gddffhioy.sHtML


<!-- 参考信息 -->