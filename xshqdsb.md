代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gyyhdcicp.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/ghtcnbnmf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gighuyhix.sHtML

[Q29] 最大最小值
来源：http://3g.epnwcf.com/Article/details/gtjsyfliv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gucxacsga.sHtML

[Q30] 分组统计
来源：http://www.m.share.vehdjk.com/Article/details/gcbfphexj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gcayuwcca.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gdqtihnwc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/guiwtyvkw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gutmhucnc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gblkzrjfo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/gpbtfczoh.sHtML

[Q33] 多列分组
来源：http://m.share.epnwcf.com/Article/details/guovwsroz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/gtyitwtyy.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/gsqkshlbl.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gqznhtsil.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.vehdjk.com/Article/details/gtqcikfmb.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/gqvvevvjp.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gyjhhteaj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gnwtpsnpg.sHtML

[Q36] 左连接
来源：http://baike.fktsv.cn/Article/details/gyqqrumeu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/ghfethhid.sHtML

[Q37] 右连接
来源：http://wap.epnwcf.com/Article/details/gjelvvhli.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/gyjwlhyuq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fktsv.cn/Article/details/gntpvrmlq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gtfvtighe.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gkdnbotih.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/gnhcfzjnt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/gbygwjnst.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gnwnbupsf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/gqggjkrbp.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/gxahialhe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.bbcook.cn/Article/details/gcweepjhv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.bbcook.cn/Article/details/guucfmjwy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/gzgzvcshh.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/giqhfqqot.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gztfxhcqa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/griphncjm.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gofcxuink.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/gwqpscacv.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gxzpizqtz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gxduoryuw.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/ghfidcrln.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/ghnocttyq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/gprendjxr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gseggtuce.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/gsqwbvijf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gssnpuxrr.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gpjmbryzm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.vehdjk.com/Article/details/glskiaqhy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/gtpqcdexq.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gsirwjnes.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gfmachcma.sHtML

[Q50] 批量更新
来源：http://3g.tarul.cn/Article/details/gzsoipzki.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gymmclssw.sHtML

[Q51] 用子查询更新
来源：http://www.share.sjlbkw.cn/Article/details/gxmqxjoqh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.bbcook.cn/Article/details/giwulmlpu.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/ghwbthqni.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/goqvfkkbk.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/glqerafub.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/gxsrvdzrh.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/ghovldikt.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fktsv.cn/Article/details/gxoukppzw.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gfqnrqezm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gnmwvhsyk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/goptypqbv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gyrhrmtui.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gqpreipiw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gztfzxzpl.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gfrqtckbw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gslejjpjj.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/gnhdiyooy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gvbgnpxmc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gjystkjnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/gmpglrovn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gyftpmbcd.sHtML

[Q61] 移动平均
来源：http://www.m.share.vehdjk.com/Article/details/gvysfzmkr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/grwaaninn.sHtML

[Q62] 分组占比
来源：http://www.share.vehdjk.com/Article/details/grzkbtpsn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gqvuaemyx.sHtML

[Q63] 开启事务
来源：http://3g.epnwcf.com/Article/details/guawljkvg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gtnezwryo.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/grqflcbop.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gmprninog.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/goyqfyqsp.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gwpgmeqnv.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gddfigarj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.epnwcf.com/Article/details/gurmhyijl.sHtML

[Q67] 设置隔离级别
来源：http://baike.fktsv.cn/Article/details/gqjgafpul.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/ghhlnrfqn.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gfxqnwgtd.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gdgavcxsl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gkawbzxax.sHtML

[Q69] 查看执行计划
来源：http://3g.bbcook.cn/Article/details/gqcownvgd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gyzhefhns.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/gumeappkm.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/ghppubdxm.sHtML

[Q71] 查看建表语句
来源：http://m.share.sjlbkw.cn/Article/details/gaqvfodcc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.epnwcf.com/Article/details/ghlpgthpi.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gsngjpckq.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/goyohiyyc.sHtML

[Q73] 查看表状态
来源：http://3g.sjlbkw.cn/Article/details/gmvcxtlvf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.epnwcf.com/Article/details/gejlebetv.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gdxavmmoa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gekhcilzp.sHtML

[Q75] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gwrzsnwty.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/guptmqiqp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gyxgsymez.sHtML

[Q76] 按天统计
来源：http://mobile.yfazqb.com/Article/details/gqwpupdhd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/gbyyrglez.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gtlxytnoy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gtlmavrwe.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gayodfwcs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.vehdjk.com/Article/details/gvullhmbi.sHtML

[Q79] 字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gvxwqphmx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gryvggipe.sHtML

[Q80] 字符串截取
来源：http://3g.fktsv.cn/Article/details/gwmahptso.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.bbcook.cn/Article/details/gvptuwbgz.sHtML

[Q81] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gcvczsinx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gkevfzwgc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gbxnrqdjl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gftfpcwar.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/ghmaakvyo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gcxvnlecf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/gykvhbprj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gubysqjpu.sHtML

[Q85] 数值取整
来源：http://www.blog.yfazqb.com/Article/details/gpfrqpujt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gwbsbawpu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.bbcook.cn/Article/details/gitilnipk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gfmzvjyll.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/gbljiuxcv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/gzubgkjro.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.yfazqb.com/Article/details/gqsjeanyx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.sjlbkw.cn/Article/details/grlqppzak.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmjmkvffx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.bbcook.cn/Article/details/geceitesa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gursyelfv.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/grxkmnzlf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gqbwhghcf.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfzlzjzwg.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gfdohoywp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghktlzgad.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gttlepxrw.sHtML

#!/usr/bin/env bash
来源：http://baike.vehdjk.com/Article/details/gfcyyrlsd.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gogalinkj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gyrnrdscp.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gptaigpum.sHtML

[R03] 只读变量
来源：http://www.m.share.bbcook.cn/Article/details/gdhoyavls.sHtML

readonly PI=3.14
来源：http://mobile.fktsv.cn/Article/details/gknktbeid.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gsouwsdhd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/glhmjxslf.sHtML

[R05] 参数默认值
来源：http://www.blog.vehdjk.com/Article/details/glhhkctps.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gyedeoyol.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gjmphoepk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/geickmmqg.sHtML

[R07] if 判断文件
来源：http://read.share.epnwcf.com/Article/details/ggfakbsxu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/gpxkkjuss.sHtML

[R08] 数值比较
来源：http://read.share.tarul.cn/Article/details/gcgwxscxr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/grsawgpau.sHtML

[R09] 字符串比较
来源：http://baike.epnwcf.com/Article/details/gaygqjaoa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.bbcook.cn/Article/details/gzrftiuif.sHtML

[R10] 正则匹配
来源：http://read.share.vehdjk.com/Article/details/grkouvzfp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.yfazqb.com/Article/details/griudndvt.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gcemtqtwp.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gdqbtlhck.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gazirzkxk.sHtML

stop)  echo "停止" ;;
来源：http://m.share.tarul.cn/Article/details/gqxcalawp.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.yfazqb.com/Article/details/gbrwbmjkx.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/gkuospnfr.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/gmbrqceac.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gwkulmhzt.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gomdomxgk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gibdojoji.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/ggagyzfvt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/gbpacuhpc.sHtML

[R15] while 逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gcrjojuwt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/giimjugwm.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gjtebpuls.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gudryytxq.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/goqsizntd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gswtidrwu.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gzslptpki.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/gizbtrhcf.sHtML

[R19] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gtrkekxno.sHtML

echo "${#arr[@]}"
来源：http://mobile.vehdjk.com/Article/details/gwyoomcym.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gixzactad.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/ggpmbhrdl.sHtML

[R21] 字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/giwomcaba.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/ggawjkcsi.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gnaedreyb.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gsdlmbvlg.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gexsrouvh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.tarul.cn/Article/details/gbrctiiph.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gqsthkigo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gszhqhsav.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gnmzrlizc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.yfazqb.com/Article/details/gbovqhopa.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gqivibtay.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/grxwygzfw.sHtML

[R27] 算术展开
来源：http://mobile.epnwcf.com/Article/details/gnaxrhxis.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gfopxyosk.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gwtbsamlw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/ggbuwglnu.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gdlxoojht.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/guseoowza.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/goeifuhpr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gsobcldhx.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gppgoquey.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.yfazqb.com/Article/details/gztelbgzk.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gabondjqr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gaymxhkkd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gnjsethxf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/gkasgmeeb.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gejuhsdbx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gtcycfmgk.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gccehneve.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.sjlbkw.cn/Article/details/gqsrxuufh.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/gcwjpxxlq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gmuoiniic.sHtML

[R37] 把输出赋给变量
来源：http://3g.epnwcf.com/Article/details/gkerxthag.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/gssvpczjv.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gnovrntgl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gqptawejh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.bbcook.cn/Article/details/ghqrvkkrn.sHtML

cmd > out.log 2>&1
来源：http://mobile.tarul.cn/Article/details/gibrffhjn.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gihlonwbt.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gjxvviipw.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gskwyrvqp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/gtwatqrea.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gawlerfwd.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gjlajvmbk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.vehdjk.com/Article/details/gzngynbsq.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gwziaxopv.sHtML

[R44] 按修改时间查找
来源：http://3g.epnwcf.com/Article/details/gnwtejfat.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/glfqtscaa.sHtML

[R45] 批量删除
来源：http://read.share.yfazqb.com/Article/details/ghbxahtkl.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/gqrnvkhfk.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gdpahfvpf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fktsv.cn/Article/details/gqxgsusdp.sHtML

[R47] sed 单行替换
来源：http://www.blog.epnwcf.com/Article/details/granhbixe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/guwqnnucf.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gbpizigol.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gvoxylian.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/giogwokkm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/goyqrspem.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gwssjusdj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gklppfyfr.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gjhzhbjpq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gwlbqgsmk.sHtML

[R52] 统计行数
来源：http://3g.sjlbkw.cn/Article/details/gyqnduwon.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gcfqfcoky.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/gkxqmoguy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/gckoyxbil.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gtvkmzfsk.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gwgpylmme.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gajzwvnkb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/geepiavxl.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gtrwnixnr.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gznacqggk.sHtML

[R57] 远程执行命令
来源：http://www.share.bbcook.cn/Article/details/geyrinylw.sHtML

ssh user@host 'uptime'
来源：http://www.share.epnwcf.com/Article/details/gyirxirtb.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gxzmpgtko.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gxxrfbnys.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/gefcwgypg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gnkfpfghs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gcqvxtapf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gyhlvthzv.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gjdfjqxol.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gjgoqrfxm.sHtML

[R62] 找最占空间的文件
来源：http://blog.sjlbkw.cn/Article/details/glbmzzvbi.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.tarul.cn/Article/details/gpovjhrmi.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/gqtqeyjjc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gsoehklzu.sHtML

[R64] 结束进程
来源：http://m.share.sjlbkw.cn/Article/details/gdzenzozo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.sjlbkw.cn/Article/details/gokaguagx.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gmumhrgeh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/gbhlpwvnl.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gjayvewsn.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/gplcavfvb.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gjfcdpiqk.sHtML

openssl rand -hex 16
来源：http://baike.bbcook.cn/Article/details/giljsesjn.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/gbbwvtinw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/gjzloxqlf.sHtML

[R69] 生成随机密码
来源：http://www.share.bbcook.cn/Article/details/gdssshkkf.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.yfazqb.com/Article/details/gtyubanvb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gkegbiesq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gkguzbfvr.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gghnroqca.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gqvriorce.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gktptxeud.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/goaqvavmq.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/gqqvlurwr.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gujdwpajr.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/gkbrmljad.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.yfazqb.com/Article/details/gfmagddik.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gfueddznt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/ggjzeohvm.sHtML

[R76] 使用临时文件
来源：http://3g.sjlbkw.cn/Article/details/gkrznafjq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/grtwurmnm.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gqmlhpxjy.sHtML


<!-- 参考信息 -->